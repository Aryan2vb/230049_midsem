# Dataset — partB/data/

## File: dataset.csv

**Source:** Synthetically generated via `sklearn.datasets.make_blobs`

**Parameters:**
- `n_samples = 300`
- `centers = 4`
- `n_features = 2`
- `cluster_std = 0.8`
- `random_state = 42`

**Columns:** `x1`, `x2`, `label`

**How to regenerate:** Run all cells in `../task_2_1.ipynb`. The dataset is generated and saved automatically.

**Why this dataset:** `make_blobs` generates isotropic Gaussian clusters, directly satisfying DP-means' spherical cluster assumption (Kulis & Jordan 2012, Section 4, Eq. 9). The 2D structure allows visual verification of cluster recovery.

**Limitations vs paper:** The paper's experiments use real-world datasets (image patches, speaker segmentation). `make_blobs` is idealized — no outliers, balanced classes, no high-dimensional structure.

## Failure Mode Dataset

The `task_3_2.ipynb` notebook uses `sklearn.datasets.make_moons` (generated inline, not saved to file):
- `n_samples = 300`, `noise = 0.1`, `random_state = 42`
- No download or manual step required.

**Notebooks that use it:** `task_2_2.ipynb`, `task_3_1.ipynb`
