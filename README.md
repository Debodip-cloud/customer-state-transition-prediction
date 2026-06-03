# Customer State Transition Prediction

A temporal state-aware machine learning framework for customer behavioural state transition prediction, purchase propensity modelling, and marketing analytics.

## Overview

Understanding customer behaviour is one of the most important challenges in modern marketing analytics. Traditional customer segmentation methods often treat customers as static groups, even though customer behaviour changes continuously over time.

This project introduces **TS-Hybrid++**, a Temporal State-Aware Hybrid Framework designed to model customer behavioural state transitions and predict future purchasing behaviour. The framework combines behavioural state discovery, temporal feature engineering, Markov transition modelling, machine learning, purchase propensity prediction, robustness testing, and explainable artificial intelligence within a unified analytical system.

The goal is to help businesses better understand how customers evolve over time and support more informed decisions related to customer retention, campaign targeting, lifecycle management, and future sales opportunities.

---

## Research Motivation

Many organisations collect large amounts of customer data but struggle to transform that information into actionable insights. Traditional approaches often focus only on a customer's current behaviour and fail to consider how customer behaviour changes over time.

For example:

* Active customers may become inactive.
* Inactive customers may return.
* Customer engagement may increase or decrease gradually.
* Purchasing patterns may change across different periods.

By modelling customer behaviour as a sequence of behavioural states rather than fixed customer segments, businesses can gain a deeper understanding of customer lifecycle dynamics and future customer actions.

---

## Proposed Framework

The TS-Hybrid++ framework consists of the following components:

1. Customer behavioural state discovery
2. Temporal feature engineering
3. Markov state transition modelling
4. Machine learning prediction models
5. Hyperparameter optimisation using Optuna
6. Transition-calibrated hybrid ensemble learning
7. Purchase propensity prediction
8. Robustness testing
9. Explainable AI and feature importance analysis
10. External validation

The framework is designed to capture both current customer behaviour and behavioural evolution over time.

---

## Datasets

### Olist Brazilian E-Commerce Dataset

The primary dataset used in this project is the Olist Brazilian E-Commerce dataset, which contains customer transactions, reviews, payments, product information, and delivery records.

### UCI Online Retail II Dataset

An external validation experiment was conducted using the UCI Online Retail II dataset to evaluate the generalisability of the framework.

---

## Methodology

The project follows the following workflow:

Raw Transaction Data

↓

Data Cleaning and Preparation

↓

Monthly Customer Aggregation

↓

Temporal Feature Engineering

↓

Behavioural State Discovery

↓

Markov Transition Matrix Construction

↓

Machine Learning Model Training

↓

Hyperparameter Optimisation

↓

Transition-Calibrated Ensemble

↓

Purchase Propensity Prediction

↓

Explainability and Robustness Analysis

---

## Machine Learning Models

The following models were evaluated:

* Logistic Regression
* Random Forest
* Extra Trees
* XGBoost
* LightGBM

Model performance was evaluated using rolling temporal validation to better simulate real-world deployment conditions.

---

## Key Features

### Behavioural State Modelling

Customers are represented as dynamic behavioural states rather than static customer segments.

### Temporal Analytics

Historical customer behaviour is incorporated through lagged features and state memory.

### Transition Modelling

Markov transition probabilities are used to model behavioural evolution.

### Purchase Propensity Prediction

The framework predicts whether customers are likely to make future purchases.

### Explainability

Permutation importance and feature importance analysis help explain model predictions.

### Robustness Testing

The framework is evaluated under multiple data perturbation scenarios to assess reliability.

---

## Key Findings

The results suggest that:

* Customer behaviour is highly dynamic and evolves over time.
* Temporal behavioural information improves predictive performance.
* Behavioural state transitions provide valuable predictive signals.
* Purchase propensity can be predicted using temporal customer information.
* Explainability techniques help identify the drivers of customer behaviour.
* The framework generalises reasonably well across multiple retail datasets.

---

## Business Applications

Potential applications include:

* Customer retention strategies
* Churn prevention
* Customer lifecycle management
* Marketing campaign targeting
* Customer reactivation campaigns
* Customer value optimisation
* Personalised marketing

---

## Repository Structure

```text
├── notebooks/
│   └── TS_Hybrid_PlusPlus.ipynb
│
├── data/
│   ├── olist/
│   └── online_retail_ii/
│
├── figures/
│
├── results/
│
├── paper/
│   ├── main.tex
│   └── references.bib
│
└── README.md
```

---

## Future Work

Future extensions may include:

* Deep learning sequence models
* Transformer-based architectures
* Real-time customer analytics
* Recommendation systems
* Multi-channel customer behaviour modelling
* Industry-specific implementations

---

## Author

**Debodip Chowdhury**

MSc Financial Technology with Data Science 
University of Bristol

---

## Citation

If you use this work in your research, please cite the accompanying paper:

**A Temporal State-Aware Hybrid Framework for Customer Behavioural State Transition and Purchase Propensity Prediction**

