# Evaluation

## Standard F1

Token-level precision and recall over {C, E, O} labels.

---

## F1ₚₕᵣₐₛₑ (proposed)

A phrase-aware F1 metric that:

- uses dependency parsing
- maps tokens to their noun-phrase head
- credits partial phrase detection as correct

This reflects downstream usability better than strict token matching.

---

## Why F1ₚₕᵣₐₛₑ matters

- Penalizes models less for annotation style mismatch
- Better reflects phrase localization ability
- Enables fair transfer comparison

Across datasets, F1ₚₕᵣₐₛₑ improves scores by up to **40%**.
