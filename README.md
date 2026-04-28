# MLflow Experimentation on Iris Dataset

## Overview

This project demonstrates the end-to-end usage of MLflow for experiment tracking, model management, and reproducibility using the Iris classification problem.

The objective is not the dataset itself, but to validate and understand MLflow’s capabilities in managing machine learning workflows in a structured and scalable manner.

---

## Objectives

* Track machine learning experiments systematically
* Log parameters, metrics, and artifacts
* Compare multiple model configurations
* Register and version models
* Understand reproducibility in ML pipelines

---

## Dataset

The project uses the Iris dataset, a standard multi-class classification dataset with:

* 150 samples
* 3 classes (Setosa, Versicolor, Virginica)
* 4 numerical features

This dataset is intentionally simple to isolate MLflow functionality without introducing data complexity.

---

## Tech Stack

* Python
* Scikit-learn
* MLflow
* Pandas / NumPy
* Matplotlib / Seaborn (for visualization)

---



---

## MLflow Implementation

### Experiment Tracking

* Logged parameters:

  * Model type (e.g., Logistic Regression, Random Forest)
  * Hyperparameters (C, max_depth, n_estimators, etc.)

* Logged metrics:

  * Accuracy
  * Precision
  * Recall
  * F1-score

* Logged artifacts:

  * Confusion matrix
  * Model files
  * Plots

---

### Model Comparison

Multiple models were trained and tracked under a single experiment:

* Logistic Regression
* Random Forest
* Decision Tree

MLflow UI enables comparison across runs based on metrics and parameters.

---

### Model Registry

* Registered best-performing model
* Versioned models for traceability
* Prepared for staging/production transition (conceptual stage)

---

## How to Run

### 1. Clone the repository

```
git clone https://github.com/your-username/mlflow-iris.git
cd mlflow-iris
```

### 2. Create environment

```
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
```

### 3. Install dependencies

```
pip install -r requirements.txt
```


### 5. Launch MLflow UI

```
mlflow ui
```

Open:

```
http://127.0.0.1:5000
```

---

## Key Learnings

* MLflow provides a structured way to manage experiments beyond notebooks
* Tracking parameters and metrics improves reproducibility
* Model registry introduces version control for ML models
* Even simple datasets are sufficient to validate MLOps concepts

---

## Limitations

* Dataset is small and not representative of production-scale problems
* No deployment pipeline integrated
* No CI/CD or automated retraining

---

## Next Steps

* Integrate MLflow with a REST API (FastAPI)
* Add Docker for containerization
* Introduce CI/CD pipeline (GitHub Actions)
* Extend to larger, real-world datasets
* Add model monitoring and drift detection

---

## Author

Naga Dheeraj S
Master’s in Advanced Data Analytics
Focus: MLOps, Machine Learning Systems, Data Engineering

---
