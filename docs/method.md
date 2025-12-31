# Method

This study focuses on **sentence-level causal relation extraction** framed as a
**sequence labeling task**.

---

## Task formulation

Each token in a sentence is labeled as:
- `C` — Cause
- `E` — Effect
- `O` — Other

Contiguous `C` or `E` tokens form causal phrases.

---

## Model architecture (general form)

All evaluated models follow:

Embedding → Recurrent Layer → Linear / CRF → Token Labels

---

## Embeddings evaluated

- BERT (base)
- BioBERT
- RoBERTa
- Flair (general, news, fine-tuned)

**Finding:** BioBERT performs best overall due to biomedical pretraining, while RoBERTa excels in some general-domain datasets.

---

## Recurrent units

- BiGRU
- BiLSTM

**Key result:**  
BiGRU matches or outperforms BiLSTM while being simpler and faster.

---

## CRF layer

Conditional Random Fields were evaluated but showed **no statistically significant benefit** in most settings and were excluded from final models.

---

## Final recommended architecture

> **BioBERT + BiGRU + Linear classifier**

This model balances performance, speed, and transferability.
