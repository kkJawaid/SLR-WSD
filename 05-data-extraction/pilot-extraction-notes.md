# Pilot Extraction Notes

## Pilot conducted: 2026-06-26

**Studies piloted:** S001, S002, S003, S006, S010 (selected to span venue
types, KG sources, and clinical/general domains)

**Reviewers:** R1 and R2 independently extracted each study, then compared
results in a 90-minute session.

## Issues identified during pilot

### Issue 1: KG size measurement
**Problem:** Some papers report node count, some report triple count, some
report disk size. Original form had a single "KG size" column.
**Resolution:** Split into two columns: "KG Size (entities)" and "KG Size
(relations)". When only one is reported, the other is left blank with a
note.

### Issue 2: LLM parameter ranges
**Problem:** Studies often use multiple LLMs for ablation (e.g., 7B, 13B, 70B
of LLaMA). How to capture?
**Resolution:** Record range as "8B-1.7T" in the "LLM Parameters" column;
list all models in the "Base LLM(s)" column separated by commas.

### Issue 3: Multi-task evaluation
**Problem:** Several papers evaluate on 3-5 different benchmarks. The
extraction form had only one "Primary Metric" cell.
**Resolution:** Allow comma-separated listing in "Datasets" and "Result"
fields, but record only the *primary* metric per the paper's stated focus.
Additional results captured in RQ3 notes.

### Issue 4: KG source ambiguity
**Problem:** Several papers mix pre-existing KGs (Wikidata, UMLS) with custom
augmentation. Single "KG Source" column was insufficient.
**Resolution:** Allow combined entries like "Wikidata + custom" with
clarification in "Graph Construction Method" column.

### Issue 5: Verbatim limitation quotes
**Problem:** Reviewers paraphrased differently, losing nuance for synthesis.
**Resolution:** Added "Verbatim limitation quotes" column to RQ Notes sheet
requiring at least one direct quote per study.

## Form changes after pilot

The extraction form template was updated 2026-06-29. The 5 piloted studies
were re-extracted using the new form to verify completeness.

## Time per study (pilot)

- S001: 38 minutes
- S002: 52 minutes (complex multi-level architecture)
- S003: 41 minutes
- S006: 35 minutes
- S010: 28 minutes

**Average:** 39 minutes per study. Estimated total for 23 studies: ~15 hours.
