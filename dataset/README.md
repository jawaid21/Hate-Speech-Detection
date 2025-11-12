# Dataset

This folder contains the CSV files used for the hate-speech detection experiments (English, Urdu and Sindhi).

Files

- [english_urdu_sindhi_curated_and_translated(full).csv](english_urdu_sindhi_curated_and_translated%28full%29.csv) — The full curated and translated dataset containing English, Urdu, and Sindhi examples (CSV).
- [train.csv](train.csv) — Training split used for model training.
- [val.csv](val.csv) — Validation split used for hyperparameter tuning and early stopping.
- [test.csv](test.csv) — Test split used for final evaluation.

Format

- Files are CSVs. Inspect the header to see the exact column names (for example: `id`, `text`, `label`, `language`).

How to load

```python
import pandas as pd

# load training split
train = pd.read_csv('train.csv')
print(train.shape)
print(train.columns)
print(train.head())
```

Notes

- The full dataset filename contains parentheses; links in this README use URL-encoded parentheses so they work on GitHub.
- If you need additional metadata (file sizes, number of rows per split, column descriptions), I can add a brief stats table.
