# Results

Each experiment compares `regular` (no augmentation) against `augmented`, 5 seeds each.

| Experiment | Training | Augmentation |
|---|---|---|
| v1 | M1 | aug1 (Dawid's first) |
| v2 | M1 | aug2 (Dawid's updated) |
| v3 | M2 | aug1 |
| v4 | M2 | aug2 |

- **M1**: first training setup, augmentation saved as one extra copy per image (commit `4b75b17`).
- **M2**: label smoothing, lower learning rate for the pretrained layers, augmentation applied on the fly (current `training.ipynb`).
- v1/v2 share the same `regular` runs, as do v3/v4 (same training, no augmentation). They're copied into both folders.

Each folder has `seedN.json` (scores, training curve) and `seedN_test_predictions.csv`, plus `summary.csv`, `ensemble.csv` and `config.json`.
