# 🚀 CausalCareNet

An uncertainty-aware causal Bayesian framework for multi-disease risk prediction, counterfactual intervention analysis, bootstrap uncertainty estimation, and optimization-driven clinical recommendations using Bayesian Networks and DAG learning.

---

##  Overview

CausalCareNet is a healthcare AI framework that combines:

- Bayesian Networks
- Directed Acyclic Graphs (DAGs)
- Causal Inference
- Bootstrap Uncertainty Estimation
- Counterfactual Intervention Analysis
- Optimization-Based Risk Reduction

to create an interpretable and uncertainty-aware clinical decision support system.

Unlike traditional black-box ML systems that only focus on prediction accuracy, this framework provides:

- Explainable probabilistic reasoning  
- Patient-level risk inference  
- Confidence interval estimation  
- Counterfactual “what-if” analysis  
- Optimization-driven intervention suggestions  

---

#  Supported Disease Pipelines

The framework currently supports:

| Notebook | Disease |
|---|---|
| ILPD | Liver Disease Prediction |
| Thyroid | Hypothyroid Risk Prediction |
| Heart | Heart Attack Risk Prediction |

---

#  Pipeline Architecture

```text
Dataset Preprocessing
        ↓
Feature Discretization
        ↓
DAG Learning
        ↓
Bayesian Network Training
        ↓
Risk Prediction
        ↓
Bootstrap Uncertainty
        ↓
Counterfactual Intervention
        ↓
Optimization Engine
        ↓
Clinical Recommendation
```

---

#  Features

##  Dataset Preprocessing
- Missing value handling
- Feature engineering
- Target standardization
- Categorical encoding
- Clinical feature discretization

---

##  DAG Learning
- Hill Climb Search
- Bayesian Information Criterion (BIC)
- Expert-guided edge constraints
- Structural Hamming Distance (SHD) evaluation

---

##  Bayesian Network Modeling
- Discrete Bayesian Networks
- Conditional Probability Tables
- Variable Elimination inference

---

##  Risk Prediction
- Patient-level posterior probability estimation
- Evidence-based disease prediction

---

##  Bootstrap Uncertainty
- Confidence interval estimation
- Prediction stability analysis
- Resampling-based uncertainty quantification

---

##  Counterfactual Intervention

Evaluate:

```math
P(Y | do(X = x))
```

Examples:
- Normalize TSH
- Reduce bilirubin
- Improve LDL levels
- Stop smoking

---

##  Optimization Engine

Finds minimum-change interventions that reduce disease risk below a desired threshold.

Objective:

```math
min ||x − x₀|| subject to P(Y = 1) < τ
```

---

##  Clinical Recommendation Engine
Provides:
- Risk-sensitive recommendations
- Intervention sensitivity analysis
- Explainable decision support

---

#  Tech Stack

## Languages
- Python

## Libraries
- pandas
- numpy
- scikit-learn
- pgmpy
- matplotlib
- seaborn
- catboost

---

#  Repository Structure

```bash
CausalCareNet/
│
├── datasets/
├── preprocessing/
├── dag_learning/
├── bayesian_network/
├── uncertainty/
├── intervention/
├── optimization/
├── recommendations/
├── notebooks/
├── visualizations/
├── results/
├── app/
│
├── ilpd-07.ipynb
├── thyroid-07.ipynb
├── heart-07.ipynb
│
├── requirements.txt
└── README.md
```

---

#  Experimental Results

## ILPD Dataset
- Bayesian Network Accuracy: **0.7136**
- Best F1 Score: **0.8328**
- Risk Reduction: **35.76%**

---

## Thyroid Dataset
- Gradient Boosting Accuracy: **1.0000**
- Bayesian Network AUC: **0.9746**
- Risk Reduction: **100%**

---

## Heart Dataset
- Bayesian Network Accuracy: **0.6993**
- SHD Score: **18**

---

#  Core Equations

## Bayesian Information Criterion (BIC)

```math
BIC = \log P(D | G) - \frac{k}{2}\log n
```

---

## Posterior Risk Inference

```math
P(Y | X = x)
```

---

## Counterfactual Intervention

```math
P(Y | do(X=x))
```

---

#  Outputs

The framework generates:
- DAG visualizations
- Model comparison tables
- Bootstrap confidence interval plots
- Intervention heatmaps
- Risk optimization outputs
- Clinical sensitivity analysis

---

#  Limitations

- Observational healthcare datasets
- Discretization may lose information
- Not intended for real-world clinical deployment
- Requires external medical validation

---

#  Future Work

- Dynamic Bayesian Networks
- Temporal healthcare modeling
- Fairness-aware causal analysis
- External hospital validation
- Cross-validation and calibration studies

---

#  Disclaimer

This project is intended strictly for:
- Research
- Educational purposes
- Experimental healthcare analytics

It should **NOT** be used for real-world medical diagnosis or treatment decisions without professional validation.

---

#  Citation

If you use this work, please cite the associated research paper.

---

