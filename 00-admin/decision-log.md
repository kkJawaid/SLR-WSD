# Decision Log

Append-only record of all methodological decisions for transparency and
reproducibility per PRISMA 2020 item 24c (amendments to protocol).

---

## 2026-04-1 — Topic scope definition

**Decision:** Limit scope to knowledge-augmented systems for Urdu Word Sense Disambiguation (WSD) — defined as the integration of Knowledge-Based Systems (KBS), structured lexical resources (e.g., WordNet, domain-specific corpora), and fine-tuned Large Language Models (LLMs) to resolve context-sensitive meanings in Urdu text. Exclude generic LLM-based NLP systems without lexical grounding, and exclude multilingual WSD approaches that do not specifically address Urdu or low-resource settings.

**Rationale:** A scoping review of existing literature indicates that while a substantial body of work exists on WSD and LLMs broadly, only a limited subset focuses on Urdu and leverages structured lexical integration. Constraining the scope to this intersection enables a focused and meaningful synthesis aimed at improving disambiguation accuracy, explainability, and system design in low-resource NLP environments.

---

## 2026-04-1 — Date range

**Decision:** Restrict search to 2018-2026.

**Rationale:** Neural contextual models for WSD and NLP matured with the introduction of transformer-based architectures (e.g., BERT in 2018), marking a shift from traditional feature-engineered and knowledge-based methods to deep contextual representations. Subsequent years saw the emergence of large language models and knowledge-augmented approaches, enabling more effective integration of lexical resources such as WordNet and annotated corpora. Limiting the timeframe to 2018–2026 captures this modern paradigm while excluding earlier rule-based and classical machine learning work that has been extensively reviewed and is less aligned with current system design practices in low-resource settings like Urdu.

---

## 2026-04-1 — Language restriction

**Decision:** Include only papers written in English.

**Rationale:** Team has multi-language capability but is more comfortable with English text; risk of misinterpretation of methodological details exceeds value of our broader linguistic coverage. This
limitation will be acknowledged in the discussion.

---

## 2026-04-1 — Publication type

**Decision:** Include peer-reviewed journal articles; Exclude arXiv preprints, workshop papers, theses, and bodies of work without any citations. 

**Rationale:** This field moves rapidly through preprints, but peer review
provides a quality floor necessary for synthesis reliability. Citations in high quality journals add credibility to the body of work. 

---

## 22026-04-1 — Search string finalization

**Decision:** Final canonical search string locked after pilot search
returned manageable counts on Scopus (1,040 records). Saved in
`02-searches/search-string-canonical.txt`.

---

## 2026-04-1 — Screening tool

**Decision:** Use Rayyan for dual-independent screening with blinding enabled.

**Rationale:** Rayyan supports the dual-independent screening workflow with
reviewer blinding required by PRISMA 2020 item 8 (selection process).
