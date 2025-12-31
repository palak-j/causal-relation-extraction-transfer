# Datasets

Six sentence-level causal relation datasets were used:

| Dataset | Domain | Implicit % | Notes |
|------|------|------|------|
| MedCaus | General/Medical | 17% | Long phrases |
| CauseNet-cause | General | 0% | Explicit markers |
| CauseNet-noncause | General | 0% | Non-cause markers |
| FinCausal2020 | Financial | 78.7% | Very long phrases |
| Causal-TimeBank | News | 54.7% | Temporal/implicit |
| SemEval 2010 Task 8 | General | 34% | Short phrases |

---

## Key observation

Datasets differ dramatically in:
- phrase length
- POS distribution
- annotation density
- implicit vs explicit causality

These differences drive transfer difficulty.
