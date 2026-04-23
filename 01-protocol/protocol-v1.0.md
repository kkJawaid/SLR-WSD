# Systematic Review Protocol (PRISMA-P 2015 + PRISMA 2020 alignment)

**Title:** Knowledge-Augmented Urdu Reading System for Context-Sensitive Word Sense Disambiguation: Design, Fine-Tuning, and Integration of Lexical Resources

**Version:** 1.0

**Date:** 2026-04-01

**Registered at:** OSF Registries (DOI placeholder: 10.17605/OSF.IO/XXXXX) [N/A IN THIS PROJECT]

**Reporting guideline followed:** PRISMA 2020 (Page et al., BMJ 2021;372:n71)

This protocol follows the PRISMA-P 2015 reporting checklist for systematic
review protocols (Moher et al., Syst Rev 2015;4:1).

## 1. Administrative information

### 1.1 Title
See above.

### 1.2 Registration
OSF Registries, DOI to be assigned at registration. [N/A IN THIS PROJECT]

### 1.3 Authors
- Khadija Kausar Jawaid, Software Engineering Undergraduate, NED-UET
- Syed Haider Shahid, Software Engineering Undergraduate, NED-UET

### 1.4 Amendments
None as of v1.0. Future amendments will be documented in the decision log
with justification, date, and impact.

### 1.5 Support
[Funding source] [N/A IN THIS PROJECT]

## 2. Introduction

### 2.1 Rationale (PRISMA-P item 6a)

Large language models struggle with severe lexical ambiguity, particularly in low-resource languages like Urdu where 17–20% of the vocabulary is highly context-sensitive. Generic, zero-shot LLMs attempt to process this language but consistently fail to capture deep cultural and semantic nuances, while traditional unsupervised methods hit a hard accuracy ceiling when sentence context is sparse. Knowledge-augmented fine-tuning—integrating structured lexical databases like WordNet into parameter-efficient training pipelines (QLoRA)—has emerged as a powerful paradigm to embed precise, context-aware reasoning directly into a model's weights. However, the Urdu NLP landscape remains fragmented and lacks cohesive, user-facing applications that leverage these specialized architectures to provide real-time disambiguation and drive digital literacy.
### 2.2 Objectives (PRISMA-P item 6b)

To systematically synthesize peer-reviewed primary literature on Knowledge-Based Systems (KBS), large language model (LLM) fine-tuning, and Word Sense Disambiguation (WSD) in low-resource environments in order to:
1. Catalog architectural patterns for integrating structured lexical resources (e.g., WordNet, domain corpora) with LLMs.
2. Map the machine learning techniques and fine-tuning paradigms utilized for WSD in Urdu and comparable low-resource languages.
3. Characterize evaluation methodologies, metrics, and reported performance for these hybrid architectures.
4. Identify open challenges and research gaps regarding fragmented architectures, resource constraints, and system explainability.

## 3. Methods

### 3.1 Eligibility criteria (PRISMA-P item 8 / PRISMA 2020 item 5)

**Inclusion criteria:**
- Peer-reviewed journal articles or peer-reviewed conference papers.
- Published between January 2018 and June 2026.
- Written in English.
- Focuses on Word Sense Disambiguation (WSD), Natural Language Processing (NLP), Knowledge-Based Systems (KBS), LLM fine-tuning, or Urdu lexical processing.
- Demonstrates the use of structured datasets (e.g., WordNet, ULS-WSD-18, or other linguistic corpora).
- Clearly describes the system architecture, integration methodology, or fine-tuning pipeline.

**Exclusion criteria:**
- Non-English papers.
- Surveys, reviews, mappings, pure opinion pieces, or editorial articles.
- Papers lacking technical or methodological detail to support extraction.
- Duplicate or redundant studies.
- Studies focusing purely on data-driven generation without the integration of structured knowledge resources.

### 3.2 Information sources (PRISMA-P item 9 / PRISMA 2020 item 6)

Four primary bibliographic databases will be searched on a single date. 

1. Google Scholar
2. IEEE Xplore
3. Springer Nature Link
4. ACM Digital Library

### 3.3 Search strategy (PRISMA-P item 10 / PRISMA 2020 item 7)

A canonical Boolean search string will be developed iteratively, targeting three conceptual blocks combined with AND:

- **Block 1 (Context/Language):** Urdu, low-resource language, NLP
- **Block 2 (Concept/Task):** Word Sense Disambiguation, WSD, lexical ambiguity, semantic understanding
- **Block 3 (Technology/Architecture):** Knowledge-Based Systems, LLM, fine-tuning, WordNet, structured lexical resources

Keywords include: *Urdu, Word Sense Disambiguation, WSD, Knowledge-Based Systems, LLM, Fine-tuning, Architecture, Word Sense Disambiguation Urdu, Knowledge-based WSD, Low-resource language WSD, WordNet WSD techniques, Knowledge-augmented language models.* The full canonical string and database-specific adaptations will be documented prior to execution.

### 3.4 Study records (PRISMA-P item 11 / PRISMA 2020 item 8)

**Data management:** Records will be exported in BibTeX or RIS format, and imported into the *Rayyan* web tool for deduplication and systematic screening.

**Selection process:** Two reviewers (R1, R2) will independently screen all records at the title/abstract and full-text stages, with reviewer blinding enabled in Rayyan. Disagreements will be resolved through discussion; unresolved disagreements will be adjudicated by a third reviewer.

**Data collection process:** Two reviewers will independently extract data from all included studies into a shared structured form. Disagreements will be resolved through consensus.

### 3.5 Data items (PRISMA-P item 12 / PRISMA 2020 item 10)

The structured data extraction form captures: bibliographic data, KBS architectural paradigms, characteristics of the structured lexical datasets used (e.g., WordNet, ULS-WSD-18), fine-tuning methodologies (e.g., QLoRA), base LLMs utilized (e.g., Alif, LLaMA), evaluation metrics (e.g., Accuracy, F1, BERTScore, COMET), comparative baselines, reported performance, and stated limitations regarding structural cohesion or explainability.

### 3.6 Outcomes and prioritization (PRISMA-P item 13 / PRISMA 2020 item 9)

**Primary outcomes:**
- Reported task performance for WSD and semantic interpretation tasks.
- Reported performance of comparative baselines (e.g., generic vs. fine-tuned, or data-driven vs. knowledge-augmented).

**Secondary outcomes:**
- System explainability and structural cohesion.
- Computational cost/efficiency of the fine-tuning approach in low-resource environments.
- Effort and methodologies required for lexical dataset integration.

### 3.7 Risk of bias (PRISMA-P item 14 / PRISMA 2020 item 11)
[N/A IN THIS PROJECT, THE FOLLOWING PARA. LEFT INTACT]

A custom risk of bias assessment instrument, adapted from QUADAS-2 principles for methodological NLP and Machine Learning studies, will be applied to each included study by two independent reviewers. This will assess potential biases in dataset selection, model evaluation transparency, and baseline fairness.

### 3.8 Data synthesis (PRISMA-P item 15 / PRISMA 2020 item 13)

Narrative synthesis is planned. Quantitative synthesis (meta-analysis) is **not** planned because primary studies in low-resource NLP utilize highly heterogeneous benchmarks, base models, and custom evaluation metrics, making numerical pooling inappropriate.

Synthesis will be organized by the predefined research questions:
- **RQ1:** Mapping of machine learning techniques and knowledge representation paradigms (e.g., ontologies, WordNet).
- **RQ2:** Thematic analysis of architectural patterns, reasoning flows, and KBS components in NLP.
- **RQ3:** Methodologies for integrating structured lexical datasets with LLMs.
- **RQ4:** Identification of primary limitations, focusing on fragmented architectures and the lack of explainability.

### 3.9 Meta-bias and certainty (PRISMA 2020 items 14, 15)
[N/A IN THIS PROJECT, THE FOLLOWING PARA. LEFT INTACT]
Reporting bias will be assessed by examining whether studies report negative results, checking for selective outcome reporting against standardized NLP benchmarks, and noting publication patterns in low-resource language research. Certainty in the synthesis will be discussed narratively, considering the risk of bias, consistency of architectural approaches, and directness of evidence.

## 4. Reporting

The completed review will be reported strictly per the PRISMA 2020 guidelines, with the 27-item checklist completed and a PRISMA 2020 flow diagram included detailing the record screening process.

## 5. Replication package

A replication package containing the final search strings, *Rayyan* screening decisions, extraction data, risk of bias assessments, and the completed PRISMA checklist will be deposited on a public github repo with a DOI prior to submission.