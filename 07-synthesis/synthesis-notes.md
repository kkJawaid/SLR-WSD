# Synthesis Notes

Working drafts of the narrative synthesis for each research question, to be
refined into the Results section of the manuscript.

## RQ1: Architectural patterns and Machine Learning Techniques

Among the 21 included studies, the following taxonomy of Urdu NLP and WSD architectures emerges:

### Top-level branches

1. **Parameter-Efficient Fine-Tuning (PEFT/QLoRA) Approaches** (5 studies)
   - Adapt pre-trained LLMs to Urdu semantics using LoRA/QLoRA on specialized datasets.
   - Examples: S010 (Qalb), S020 (Alif-1.0-8B), S033 (QLoRA foundation)
   - Strength: Achieves SOTA contextual understanding; highly resource-efficient.
   - Weakness: Requires high-quality, native instruction datasets to prevent catastrophic forgetting.

2. **Zero-Shot / Few-Shot Generalist Prompting** (4 studies)
   - Utilize massive multilingual models (GPT-4, LLaMA-3) using targeted prompt engineering (e.g., Chain-of-Thought, cultural prompts).
   - Examples: S017 (Zero-shot NLP benchmark), S018 (Cross-lingual QA), S019
   - Strength: No training cost; leverages massive pre-existing knowledge.
   - Weakness: Severe performance drops in Urdu compared to English; fails on complex boundary detection and cultural idioms.

3. **Unsupervised Semantic Similarity & Context-Aware Embeddings** (3 studies)
   - Calculate cosine similarity between context embeddings (e.g., BERT) and dictionary glosses to bypass annotated data scarcity.
   - Examples: S024 (CASS with BERT), S027 (All-words N-gram similarity)
   - Strength: Does not require massive labeled training data.
   - Weakness: Hits a hard accuracy ceiling (~57-77%); fails when sentence context is sparse.

4. **Rule-Based Lexicons & Semantic Web Ontologies (Traditional KBS)** (2 studies)
   - Manually constructed RDF/XML ontologies or heuristic sentiment rules.
   - Examples: S025 (Rule-based polarity), S031 (Semantic Web IR)
   - Strength: High precision within strictly bounded, domain-specific tasks.
   - Weakness: Labor-intensive; lacks scalability to general open-domain reading tasks.

5. **Traditional ML + Feature Extraction** (1 study)
   - Use classical classifiers (Naive Bayes, SVM) with Bag of Words (BoW) or Word2Vec.
   - Examples: S026 (ULS-WSD-18 baseline)
   - Strength: Computationally cheap; establishes historical baseline.
   - Weakness: Cannot capture deep, multi-word semantic relationships.

### Trends over time

- **2018-2022:** Foundational WSD work relies on traditional ML (BoW), unsupervised similarity, and manual rule-based KBS.
- **2023:** Introduction of QLoRA (S033) changes the paradigm for low-resource hardware constraints.
- **2024-2025:** Benchmarking reveals generic LLMs (GPT-4) fail at Urdu WSD and idioms (S015, S018). Focus shifts to specialized vs. generalist comparisons (S019).
- **2026:** SOTA is dominated by natively fine-tuned, parameter-efficient Urdu LLMs (Qalb, UrduLM, Alif) utilizing synthetic/distilled instruction data.

## RQ2: Lexical Resources and Integration Mechanisms

### Structured Datasets & Lexical Sources Used

| Dataset / Lexical Source | Studies | Notes |
|---|---|---|
| Native Urdu WSD Corpora (ULS-WSD-18, UAW-WSD-18) | 2 | Crucial ground-truth WSD data |
| Synthetic/Distilled Multilingual Instruct Data | 3 | Used for SFT (e.g., Urdu-Instruct) |
| Human-validated Translated Benchmarks | 1 | UrduBench (S014) |
| Machine-Translated QA/Text Corpora | 3 | Prone to semantic fragmentation |
| Native Urdu Dictionaries (Urdu Lughat) | 2 | Used for unsupervised gloss matching |
| Custom Domain Ontologies / Sentiment Lexicons | 2 | Domain-specific (State Aid acts, polarity) |

### Knowledge Integration Mechanisms

| Mechanism | Studies |
|---|---|
| Supervised Fine-Tuning (SFT) via LoRA/QLoRA | 5 |
| Context-Aware Prompting (CoT, Cultural Rules) | 4 |
| Unsupervised Cosine/N-gram Similarity Matching | 2 |
| Heuristic Lexical Rules (If/Then context triggers) | 1 |
| RDF/SPARQL Graph Queries | 1 |

## RQ3: Evaluation methodologies

### Benchmarks used

| Benchmark/Task | Studies |
|---|---|
| General NLP / Translation (MMLU, BLEU/COMET tasks) | 6 |
| Custom QA (UQuAD1.0, SQuAD 2.0) | 2 |
| Reasoning (UrduBench, MGSM, MATH) | 2 |
| Lexical Sample WSD (ULS-WSD-18, CoarseWSD-20) | 2 |
| All-Words WSD (UAW-WSD-18) | 1 |

### Comparative baselines

- 7 studies compared specialist (fine-tuned) models against generalist LLMs (GPT-4, LLaMA base).
- 4 studies compared WSD models against the "Most Frequent Sense" (MFS) baseline.
- 3 studies compared LLMs against traditional Neural Machine Translation (NMT) systems.
- 1 study compared Semantic Web IR against generic search engines (Google/Bing).

### Reported performance ranges (Contextual Understanding & WSD)

- **Unsupervised / N-gram WSD:** 57.7% (All-words) – 77.7% (Lexical sample)
- **Traditional ML (Naive Bayes + BoW):** ~81.4%
- **Specialist/Fine-tuned Urdu LLMs (Alif, Qalb):** 85% – 90%+ weighted scores on standard tasks.
- **Zero-shot Generalist LLMs (GPT-4 on Urdu):** Often suffer a 10-15% performance drop compared to English baselines.

*Note: Absolute cross-study numerical comparison is invalid due to the shift from strict classification WSD metrics (Accuracy) to generative LLM metrics (BERTScore, COMET, LLM-as-a-judge).*

## RQ4: Open challenges (thematic synthesis)

1. **The "Tokenizer Tax" and Script Issues** (5 studies) — Multilingual LLM tokenizers are highly inefficient for the Perso-Arabic Nastaliq script, leading to boundary detection errors and high compute costs.
2. **Translation Artifact Contamination** (4 studies) — Relying on English-to-Urdu translated datasets destroys cultural nuance and semantic integrity, yielding poor training data.
3. **Idiom and Cultural Nuance Failure** (3 studies) — Even state-of-the-art LLMs systematically fail at translating or disambiguating figurative language, puns, and idioms without explicit native fine-tuning.
4. **Lack of Large-Scale Annotated Data** (3 studies) — While lexical sample corpora (ULS-WSD-18) exist, large-scale "All-Words" WSD datasets are too small for robust deep learning training without synthetic augmentation.
5. **Hardware and Compute Constraints** (3 studies) — Despite QLoRA, running effective 8B+ parameter models for native WSD tasks remains computationally expensive for low-resource regional deployment.

## Cross-cutting observations

- **The Paradigm Shift:** The field has definitively moved away from manually constructed semantic ontologies and rigid rule-based lexicons toward parameter-efficient fine-tuning (QLoRA) of generative LLMs.
- **Specialists over Generalists:** For a complex, culturally bounded task like Urdu WSD, natively fine-tuned models (Alif, UrduLM) consistently outperform much larger, proprietary generalist models (GPT-4) in accuracy and cultural alignment.
- **Data Quality Trumps Scale:** As established by the QLoRA foundation and polyglot teacher studies, a small, highly curated native Urdu dataset yields vastly superior disambiguation results compared to scraping massive, noisy, machine-translated web corpora.