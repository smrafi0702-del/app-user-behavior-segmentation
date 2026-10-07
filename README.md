# App User Behavior Segmentation

This project explores app user behavior and uses clustering to identify behavioral groups. The analysis is documented in a Jupyter notebook.

## Project structure

- `data/app_user_behavior_dataset.csv` — user behavior data
- `notebooks/app_user_behavior_segmentation.ipynb` — analysis notebook
- `README.md` — project overview and instructions

## Analysis overview

The notebook includes:

- Dataset inspection, missing-value checks, and duplicate checks.
- Median imputation for missing `rating_given` values.
- Exploratory analysis of behavioral features and their distributions.
- Standardization of selected behavioral features.
- K-Means experiments using inertia and silhouette scores, followed by a two-cluster model.
- Cluster profiling and visualizations, including PCA.
- Exploratory hierarchical clustering and DBSCAN analyses on samples.

The notebook notes that the K-Means groups overlap substantially and have a low silhouette score. Treat the clusters as exploratory; they do not necessarily represent clearly separated customer segments. Cluster numbers are labels, not rankings.

## Requirements

Install the libraries used by the notebook: `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `scipy`, and `jupyter`.

## Run the notebook

From the project root, start Jupyter with `jupyter notebook`, then open `notebooks/app_user_behavior_segmentation.ipynb`.

The notebook expects the dataset at `data/app_user_behavior_dataset.csv`.

## Data considerations

Review the dataset for sensitive or personal information before publishing it. Confirm that the sample sizes in the notebook are appropriate for the dataset you use.