# Causal Relation Extraction Transfer: Design and Data

This repository accompanies the paper:
[Paper](https://arxiv.org/abs/2503.06076)


**An Empirical Study of Causal Relation Extraction Transfer: Design and Data**

The project presents a large-scale empirical analysis of **model architectures, embeddings, and data transfer strategies** for sentence-level causal relation extraction across diverse domains and annotation styles.

---

## Problem

Causal relation extraction models are often trained and evaluated on a **single dataset**, leading to poor generalization. Differences in:
- domain (medical, financial, news, general)
- annotation style
- implicit vs explicit causality
- phrase length

It make transfer learning particularly challenging.

---

## Contributions

This work shows that:

- **BioBERT + BiGRU** consistently generalizes better than more complex architectures
- **CRF layers and BiLSTMs are unnecessary** for open-domain causal extraction
- **Data diversity matters more than data size**
- **Implicit causality improves transfer**
- A new evaluation metric, **F1ₚₕᵣₐₛₑ**, better measures transfer performance

---

## Core idea

> Transferable causal extraction depends more on **noun-phrase localization and dataset composition** than architectural complexity.

---

## Repository status

✅ Full technical documentation  
✅ Dataset descriptions & evaluation protocol  

---

## Contents

- `docs/method.md` — model architectures & labeling scheme  
- `docs/experiments.md` — embedding, RNN, CRF ablations  
- `docs/evaluation.md` — F1 vs F1ₚₕᵣₐₛₑ  
- `docs/transfer_analysis.md` — cross-dataset transfer results  
- `docs/reproduction.md` — reproducibility protocol  

