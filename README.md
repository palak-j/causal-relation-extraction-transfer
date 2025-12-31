# Causal Relation Extraction Transfer: Design and Data

This repository accompanies the paper:
[Paper](https://arxiv.org/abs/2503.06076)


**An Empirical Study of Causal Relation Extraction Transfer: Design and Data**

The project presents a large-scale empirical analysis of **model architectures, embeddings, and data transfer strategies** for sentence-level causal relation extraction across diverse domains and annotation styles.

---
<img width="1124" height="257" alt="image" src="https://github.com/user-attachments/assets/000af721-3c5e-4c62-a470-97acafd41beb" />


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

- [Model architectures & labeling scheme](docs/method.md)  
- [Embedding, RNN, CRF ablations](docs/experiments.md)  
- [F1 vs F1ₚₕᵣₐₛₑ](docs/evaluation.md)  
- [Cross-dataset transfer results](docs/transfer_analysis.md)  
- [Reproducibility protocol](docs/reproduction.md)  

