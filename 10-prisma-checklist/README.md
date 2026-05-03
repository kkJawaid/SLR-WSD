# PRISMA 2020 Compliance

This folder is the central location for everything related to PRISMA 2020 compliance for the Systematic Literature Review on Urdu Word Sense Disambiguation (WSD) and LLM Fine-Tuning.

## Files

- `prisma-2020-checklist.xlsx` — A copy of the checklist for ongoing tracking
- `prisma-2020-statement-citation.txt` — Citation information for PRISMA 2020
- This README

The completed, page-mapped checklist for the final manuscript lives at `../08-manuscript/prisma-2020-checklist-completed.xlsx`.

## What is PRISMA 2020?

PRISMA 2020 (Preferred Reporting Items for Systematic Reviews and Meta-Analyses, 2020 update) is the most widely adopted reporting guideline for systematic reviews. It consists of:

1. A 27-item checklist (with sub-items, 42 total reporting items)
2. A flow diagram template
3. An abstract checklist
4. Explanation and elaboration document

PRISMA 2020 is endorsed by:
- BMJ, JAMA, The Lancet, NEJM, PLOS Medicine
- Knowledge-Based Systems (Elsevier)
- ACM Transactions on Asian and Low-Resource Language Information Processing (TALLIP)
- Information Fusion
- Most Cochrane and Campbell collaborations
- Many other journals across disciplines

## Why PRISMA 2020 alone (not Kitchenham, not Wohlin)?

This review uses PRISMA 2020 as the sole reporting guideline because:

1. It is the most widely accepted standard across disciplines, ensuring broad academic validity.
2. The target venues for this NLP/AI research (e.g., Knowledge-Based Systems, TALLIP) explicitly recommend it.
3. PRISMA 2020 is sufficient for methodological rigor when applied thoroughly, especially for tracking database searches (IEEE Xplore, Google Scholar) and screening phases (Rayyan).
4. Adding multiple guidelines creates ambiguity about which takes precedence when they differ.
5. PRISMA 2020 is more recent (2020) than Kitchenham (2007) and reflects current best practices in managing risk of bias and dataset construction quality.

For other valid options in CS/SE reviews, see:
- Kitchenham & Charters 2007/2015 — preferred strictly in software engineering
- Wohlin 2014 — snowballing procedure when database coverage is uncertain (our review explicitly relies on strict database identification, avoiding snowballing)
- ROSES — environmental sciences

These were considered and explicitly not adopted for this review.

## How to use this checklist

1. **At protocol stage:** Use the checklist as a planning aid — every item should be addressable in your protocol or planned for the manuscript.
2. **During the review:** Refer back to relevant items as you complete each methodological step (e.g., extracting LLM Base architectures, assessing Lexical Resource Quality).
3. **At manuscript drafting:** Map every item to a specific page or section.
4. **At submission:** Submit the completed checklist as a supplementary file alongside the manuscript via the replication package (Zenodo/GitHub).

Reviewers will check that every item has either a page number or a clear "Not applicable" justification (e.g., Item 12 "Effect measures" is N/A due to the narrative synthesis approach).