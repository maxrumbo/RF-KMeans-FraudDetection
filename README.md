# Machine Learning Clustering Classification

This repository contains an end-to-end machine learning project focused on two main tasks:

1. Clustering for transaction pattern segmentation.
2. Classification to predict target labels generated from clustering.

The entire pipeline is implemented in Python using Jupyter Notebook, and the models are saved as artifacts for evaluation and reuse.

## Project Goals

- Build a clustering model based on transaction features.
- Apply dimensionality reduction for further analysis.
- Generate a derived dataset that includes a Target column.
- Train a classification model using clustering output.
- Explore alternative models and perform hyperparameter tuning.

## Dataset

The main dataset is related to financial transaction patterns and is used for:

- Data exploration.
- Feature preprocessing.
- Cluster formation.
- Preparing a classification-ready dataset.

Available dataset files in this repository:

- data_clustering.csv
- data_clustering_inverse.csv

## Project Structure

- [Clustering]_Submission_Akhir_BMLP_Your_Name.ipynb
	Notebook for the clustering stage, including preprocessing, cluster modeling, and evaluation.

- [Klasifikasi]_Submission_Akhir_BMLP_Your_Name.ipynb
	Notebook for the classification stage using clustering output data.

- model_clustering.h5
	Saved clustering model.

- PCA_model_clustering.h5
	PCA artifact for dimensionality reduction.

- decision_tree_model.h5
	Decision Tree classification model.

- explore_random_forest_classification.h5
	Random Forest model for performance exploration.

- tuning_classification.h5
	Model artifact from the tuning process.

## Technologies and Libraries

Main libraries used in the notebooks:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- yellowbrick
- joblib

## How to Run

1. Clone this repository.
2. Make sure Python 3.10+ is installed.
3. Install the notebook dependencies.
4. Run the clustering notebook first.
5. Run the classification notebook after the clustering output dataset is ready.

Example dependency installation:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn yellowbrick joblib jupyter
```

Run Jupyter:

```bash
jupyter notebook
```

## Workflow Summary

1. Data loading and data understanding.
2. Data preprocessing and categorical feature encoding.
3. Scaling and cluster formation.
4. Cluster evaluation (including silhouette/elbow as defined in the notebooks).
5. Save clustering and PCA artifacts.
6. Split data for classification.
7. Train Decision Tree and alternative models.
8. Evaluate classification metrics and tuning results.
9. Save final models.

## Notes

- Model files use the .h5 extension, but the notebooks save models using joblib.
- For reproducibility, use the same random_state values as in the notebooks.


