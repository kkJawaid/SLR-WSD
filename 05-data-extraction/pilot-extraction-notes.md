edit pilot-extraction-notes.md and copy paste this:

# Pilot Extraction Notes

## Pilot conducted: 2026-04-23

**Studies piloted:** S001, S002, S009, S010, S018 (selected to span varying domains including digital literacy, Urdu LLM pre-training, and zero-shot evaluations).

**Reviewers:** R1 (Student 1) and R2 (Student 2) independently extracted a subset of the dataset to standardize the process.

## Issues identified during pilot

### Issue 1: Task Heterogeneity (WSD vs. General NLP)
**Problem:** Very few papers exclusively use the exact term "Word Sense Disambiguation" for Urdu. Many group context-sensitive language into broader tasks such as idiom translation (S013), sentiment polarity disambiguation (S025), or general reasoning (S014).
**Resolution:** Broadened the operational definition of WSD during extraction. Relevant semantic tasks (idioms, context-dependent sentiment, code-switching) are now explicitly captured under the "Key Issue" and "Key Finding" columns to ensure no relevant architectural data is missed.

### Issue 2: Disentangling Generic vs. Fine-tuned Models
**Problem:** Many papers evaluate a massive suite of models (e.g., comparing zero-shot GPT-4 against fine-tuned LLaMA or specialist models). Extracting all of this cluttered the "Key Findings".
**Resolution:** Extraction instructions updated to prioritize findings that directly compare generalist (zero-shot) models against specialist (fine-tuned/QLoRA) models, as this directly informs our project's methodology involving Alif-1.0-8B-Instruct and Qwen 2.5.

### Issue 3: Defining the "Key Issue" for Non-Technical Papers
**Problem:** Papers focusing on the socio-technical aspects of Urdu (e.g., S001, S002 on digital literacy and immigrant reading habits) lacked traditional machine learning problem statements.
**Resolution:** For socio-technical papers, the "Key Issue" is extracted based on how the linguistic divide or comprehension barriers justify the need for AI-assisted reading applications, grounding our project's user-facing objectives.

## Form changes after pilot

The extraction form template was updated and split into two distinct reviewer assignments on 2026-04-23. The initial 21 fully-populated studies from the CSV were re-extracted into these new forms to verify completeness and consistency.

## Time per study (Preliminary Extraction Phase)

Varied and Untracked.