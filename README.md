# IRP

## About this template

We generated this repository for you to work in during your IRP. Please note that if your code is confidential, you do not need to submit your code here.

- For project information updates, please refer to `README.md` in [`info/`](./info) directory.
- For details on deliverable submissions, please refer to `README.md` in [`reports/`](./reports) directory.

If you have any questions or experience any difficulties, please get in touch with Marijan (m.beg@imperial.ac.uk).

# Explainable AI: understand the black box of predictive models with chemical engineering applications

This project will focus on the explainability of machine learning predictive models for drop coalescence conducted in microfludics device and use initial experimental conditions as input. In the first stage, the student will construct different ML predictive models, including random forest, XGboost and deep neural networks. The second stage consists of extensive analysis of model results/parameters. SHAP and LIME will be used for model interpretbility.

# Getting Started

Programming language: Python 3.8
# Software Requirement
## Environment Installation
First of all, please set up a conda environment
```
conda env create -n XAI 
conda activate XAI
pip install numpy pandas scikit-learn xgboost matplotlib seaborn shap tensorflow lime
```

# Dataset
We use min-max normlazation to rescale the raw dataset, and split it into two for training and testing repectively. Validation step is evaluated by using 5-fold cross validation.
The experimental data can be available upon reasonable request to Dr. Nina Kovalchuk (n.kovalchuk@bham.ac.uk)

|  | Coalescence | Non-Coalescence | Total |
| :-----| :----: | :----: | :----: |
| Total Dataset | 782 | 719 | 1501 |
| Training Dataset | 625 | 575 | 1200 |
| Testing Dataset | 157 | 144 | 301 |

# Implementation
# Generating Predictive Results

We trains random forest, XGBoost and MLP classifier to get predictions. The corresponding implementation code are shown in code folder.

# Interpret predictive models

We use SHAP and LIME to get model interpetbility. Feature ablation testing is also used to analyse feature importance. The feature ablation results is shown in code/ablation_test.ipynb


