
# EBM Eval Harness: LLM Benchmarking for Evidence Synthesis

A rigorous, gold-standard evaluation harness for testing the accuracy, hallucination rate, and structural compliance of Large Language Models (LLMs) in Evidence-Based Medicine (EBM).

## The Bottleneck
Everyone is trying to use GPT-4, Claude 3, and Llama to extract PICO (Population, Intervention, Comparator, Outcome) data from clinical trial PDFs. However, there is no standardized way to measure if an LLM is actually safe to use for meta-analyses, leading to dangerous hallucinations in pooled effect sizes.

## The Solution
This harness provides:
1. **The Gold Standard Dataset:** A curated set of open-access RCTs paired with human-verified, double-adjudicated extraction JSONs.
2. **The Evaluator:** An automated Python engine that scores LLM outputs on exact matching, semantic equivalence (for text fields), and numerical precision (for 2x2 tables and hazard ratios).
3. **The Hallucination Penalty:** Strictly penalizes models that generate data not present in the source text.

Part of the E156 Ecosystem's quality assurance layer.

