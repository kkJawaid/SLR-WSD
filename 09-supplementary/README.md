# Replication Package

Materials needed to replicate or build on this systematic literature review. Per PRISMA 2020 item 27, this package will be deposited on Zenodo with a DOI before manuscript submission.

## Contents

- `S1-search-strings/` — Full search strings for IEEE Xplore and Google Scholar
- `S2-prisma-checklist.pdf` — Completed PRISMA 2020 27-item checklist
- `S3-excluded-studies.xlsx` — Studies excluded at full-text with reasons (item 16b)
- `S4-risk-of-bias-details.xlsx` — Per-study, per-domain risk of bias detail (Lexical Resource Quality focus)
- `S5-data-extraction.xlsx` — Complete data extraction from all 33 studies
- `S6-included-studies.bib` — BibTeX of all included studies

## Why a replication package matters

PRISMA 2020 item 27 requires reporting which materials are publicly available. Reviewers and future researchers should be able to:
1. Verify any number reported in the manuscript (e.g., the 33 included studies)
2. Re-run the search to extend the review to newer Urdu LLM developments
3. Apply our WSD extraction form to their own NLP systematic reviews

## DOI

To be assigned at Zenodo deposit before submission.
Placeholder: 10.5281/zenodo.XXXXXXX

## Supplementary Files Manifest

| ID | Title | Source File | Description |
| :--- | :--- | :--- | :--- |
| S1 | Database search strings (2 databases) | `../02-searches/*-2026-04-02.txt` | All canonical and per-database adapted Boolean strings for IEEE Xplore and Google Scholar |
| S2 | Completed PRISMA 2020 checklist | `../08-manuscript/prisma-2020-checklist-completed.xlsx` | All 27 items mapped to manuscript pages, adapted for ML/NLP reviews |
| S3 | Excluded studies with reasons | `../03-screening/full-text-screening.xlsx` | Per item 16b, the 63 full-text exclusions with specific reasons (e.g., wrong script, no WSD focus) |
| S4 | Risk of bias details | `../06-risk-of-bias/risk-of-bias-assessment.xlsx` | Per-study, per-domain assessments focusing on D2 Lexical Resource Quality |
| S5 | Complete data extraction | `../05-data-extraction/data-extraction.xlsx` | All extraction columns (Base LLM, Lexical Resource Used, Architectures) for all 33 included studies |
| S6 | Included studies BibTeX | `included-studies.bib` | BibTeX of all 33 included studies for citation reuse (present in final draft) |