# Robustness-Bias-Analysis-of-NLI-Models-SNLI-

Link: https://colab.research.google.com/drive/1prrmnZfZOCpOZ8rtDC5D8yFaLPDrfnie?usp=sharing

## Overview

Fine-tuned a DistilBERT model on the SNLI dataset and analyzed how much the model relies on evidence vs. dataset bias.

Focus: robustness, hypothesis-only bias, and adversarial evaluation.

---

## Experiments

### 1. Normal Evaluation (Premise + Hypothesis)
Accuracy: **~75%**

Model performs strongly on entailment and contradiction.

---

### 2. Evidence Swapped (Adversarial Test)
Accuracy: **~46%**

- Entailment collapses (~12%)
- Contradiction spikes (~92%)

Shows model depends on premise-hypothesis interaction.

---

### 3. Claim-Only Baseline (Hypothesis Only)
Accuracy: **~60%**

Significantly above random (33%), indicating strong hypothesis bias in SNLI.

Neutral class shows highest hypothesis-only predictability.

---

## Key Insights

- Evidence adds ~15% performance over claim-only.
- SNLI contains annotation artifacts.
- Per-class analysis reveals bias patterns.
- Accuracy alone does not measure reasoning.

---

## Stack

Python • PyTorch • HuggingFace Transformers • Datasets • Scikit-learn

---

Author: Arshpreet




