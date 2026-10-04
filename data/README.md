# Dataset

This project uses the Criteo Attribution Modeling for Bidding Dataset.

Dataset source:
https://www.kaggle.com/datasets/sharatsachin/criteo-attribution-modeling

The raw dataset is not stored in this GitHub repository because of its large file size.

It can be downloaded programmatically using KaggleHub:

```python
import kagglehub

path = kagglehub.dataset_download(
    "sharatsachin/criteo-attribution-modeling"
)

print(path)
