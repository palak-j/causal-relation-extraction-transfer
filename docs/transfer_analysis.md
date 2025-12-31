# Transfer Learning Analysis

## Pairwise transfer

Models trained on one dataset and evaluated on another show:

- MedCaus transfers best despite domain mismatch
- CauseNet-only training underperforms on implicit datasets

---

## Combined data transfer

Training on **multiple datasets simultaneously**:

- improves transfer in all cases
- regardless of domain or size

---

## Key insight

> Training data **composition** matters more than training data **volume**.

Longer annotations and implicit causality improve generalization.
