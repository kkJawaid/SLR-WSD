# Risk of Bias Assessment Instrument

A custom instrument addressing PRISMA 2020 item 11 (study risk of bias
assessment). Adapted from QUADAS-2 (Whiting et al., Ann Intern Med 2011)
principles for methodological NLP studies.

Each domain is rated:
- **Low risk** — Sufficient information; methodology sound
- **Some concerns** — Information incomplete or methodology has minor issues
- **High risk** — Significant methodological weakness or missing information

Studies with two or more "high risk" ratings are flagged for sensitivity
analysis but are NOT excluded from synthesis (per PRISMA 2020, risk of bias
informs interpretation, not inclusion).

## Domains

### D1. Selection of evaluation data
Are the evaluation benchmarks/datasets clearly described, appropriate for
the claimed task, and free from contamination with the LLM training corpus?

**Low risk:** Standard benchmarks, contamination addressed
**Some concerns:** Benchmark described but contamination not addressed
**High risk:** Custom dataset without sufficient description, or known
contamination

### D2. Corpus Quality
How rigorously did they construct their training dataset, lexicon, or corpus?

**Low risk:** Construction fully described, quality metrics reported
**Some concerns:** Construction described but no quality validation
**High risk:** Construction process unclear or undocumented

### D3. Comparative baselines
Are comparative baselines appropriate, current, and fairly implemented?

**Low risk:** Strong baselines including current SOTA, fair implementation
**Some concerns:** Limited or older baselines
**High risk:** No baselines or weak/unfairly-implemented baselines

### D4. Metric appropriateness
Are evaluation metrics appropriate for the task and reported with
sufficient detail (e.g., confidence intervals, multiple runs)?

**Low risk:** Appropriate metrics, statistical analysis present
**Some concerns:** Standard metrics without statistical analysis
**High risk:** Inappropriate metrics or single-run results without variance

### D5. Reproducibility
Is sufficient information provided to reproduce the results (code,
hyperparameters, random seeds, model versions)?

**Low risk:** Code released, hyperparameters and seeds reported
**Some concerns:** Some reproducibility info missing
**High risk:** No code, no hyperparameters, or LLM version unspecified

### D6. Conflict of interest
Are funding sources and competing interests disclosed? Is there a clear
relationship between the authors and any commercial product evaluated?

**Low risk:** Full disclosure, no apparent conflict
**Some concerns:** Disclosure present but commercial relationship exists
**High risk:** No disclosure, or evident undisclosed conflict

## Overall risk of bias

Studies with all domains "low risk" are rated **Low overall**.
Studies with one "high risk" or several "some concerns" are rated
**Some concerns overall**.
Studies with two or more "high risk" are rated **High overall**.

## Process

1. Both R1 and R2 divided the studies and evaluated them independently
2. Any disagreements were resolved via discussion