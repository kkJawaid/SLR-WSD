# Manuscript Outline (v0.1)

**Target venue:** Knowledge-Based Systems (Elsevier) or ACM Transactions on Asian and Low-Resource Language Information Processing (TALLIP)

**Target submission:** 2026-06-30

**Reporting guideline:** PRISMA 2020 (mandatory in author guidelines)

## Title

Parameter-Efficient Fine-Tuning of Large Language Models for Urdu Word Sense Disambiguation: A Systematic Literature Review

## Abstract (PRISMA 2020 item 2 — structured)

- **Background:** [The linguistic divide, Nastaliq script challenges, and the failure of zero-shot multilingual LLMs on Urdu figurative language]
- **Objectives:** [The four RQs covering architectures, lexical resources, evaluation metrics, and open challenges]
- **Methods:** [IEEE Xplore & Google Scholar, 2018-2026, dual-blind screening via Rayyan, risk of bias via QUADAS-2 adaptation]
- **Results:** [33 included studies, paradigm shift to QLoRA, superiority of specialist vs. generalist models]
- **Conclusions:** [Necessity of native instruction datasets, limitations of machine-translated corpora, future directions]
- **Registration:** OSF Registries DOI (if applicable) or University repository

## 1. Introduction (PRISMA 2020 items 3-4)

- 1.1 Background: LLMs, low-resource language barriers, and the complexity of Urdu Word Sense Disambiguation (WSD)
- 1.2 The paradigm shift: From traditional Rule-Based/ML methods to Generative LLMs and QLoRA
- 1.3 Gap: Lack of rigorous systematic synthesis on Urdu-specific LLM fine-tuning and resource integration
- 1.4 Objectives and research questions (PCC framework)
- 1.5 Contributions

## 2. Methods (PRISMA 2020 items 5-15)

- 2.1 Protocol and registration (item 24a-c)
- 2.2 Eligibility criteria (item 5)
- 2.3 Information sources (item 6) — IEEE Xplore and Google Scholar
- 2.4 Search strategy (item 7) — Full Boolean strings in supplementary
- 2.5 Selection process with dual independent reviewers (Student 1 & Student 2) via Rayyan (item 8)
- 2.6 Data collection process (item 9)
- 2.7 Data items (item 10) — Architecture, LLM Base, Lexical Resources, Metrics
- 2.8 Risk of bias assessment (item 11) — Custom instrument focusing on Lexical Resource Quality
- 2.9 Effect measures (item 12) — N/A for narrative synthesis
- 2.10 Synthesis methods (item 13) — Thematic coding and comparative taxonomy
- 2.11 Reporting bias assessment (item 14)
- 2.12 Certainty assessment (item 15)

## 3. Results (PRISMA 2020 items 16-22)

- 3.1 Study selection
  - **Figure 1: PRISMA 2020 flow diagram** (1,040 initial -> 33 included)
  - 3.1.1 Numbers identified, screened, included (item 16a)
  - 3.1.2 Excluded studies with reasons (item 16b)
- 3.2 Study characteristics (item 17)
  - **Table 1: Characteristics of included studies**
- 3.3 Risk of bias in studies (item 18)
  - **Figure 2: Risk of bias summary**
- 3.4 Results of individual studies (item 19)
- 3.5 Results of syntheses (item 20)
  - 3.5.1 RQ1: Architectural patterns and ML techniques
    - **Figure 3: Urdu WSD architecture taxonomy** (Rule-based -> PEFT)
  - 3.5.2 RQ2: Lexical resources and knowledge integration
    - **Table 2: Corpora, dictionaries, and synthetic data sources**
  - 3.5.3 RQ3: Evaluation methodologies and baselines
    - **Table 3: Benchmarks, generative metrics, and specialist vs. generalist comparisons**
  - 3.5.4 RQ4: Open challenges
    - **Table 4: Thematic categories** (Tokenizer Tax, Translation Artifacts, Idiom Failures)
- 3.6 Reporting biases (item 21)
- 3.7 Certainty of evidence (item 22)

## 4. Discussion (PRISMA 2020 item 23)

- 4.1 Summary of evidence
- 4.2 The dominance of QLoRA and Specialist Models over Generalists (GPT-4)
- 4.3 The Native vs. Translated Dataset gap
- 4.4 Limitations of the evidence (e.g., small scale of All-Words WSD datasets)
- 4.5 Limitations of the review process
- 4.6 Implications for research and practice (Building the AI-assisted reading app)

## 5. Conclusions

## Other (PRISMA 2020 items 24-27)

- Registration and protocol (24a-c)
- Support / funding (25)
- Competing interests (26)
- Availability of data, code, materials (27) — Replication package (Search strings, Rayyan exports, Extraction sheets)

## References

## Supplementary Materials

- S1: Full database search strings
- S2: PRISMA 2020 checklist
- S3: List of excluded studies with reasons
- S4: Risk of bias details and instrument
- S5: Data extraction tables

---

**Status as of 2026-04-29:** Outline locked. Methods drafted by 2026-05-15.