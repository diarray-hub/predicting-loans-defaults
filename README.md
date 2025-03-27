# Predicting Loan Defaults with Machine Learning

This repository contains the code, resources, and final report of my undergraduate thesis: **"Conception d’un Modèle de Prédiction des Défauts de Paiement sur les Prêts : Approches, Algorithmes et Évaluation comparative"**.  
The project was completed in 2024 as part of my Bachelor's studies in Mali, and explores various machine learning techniques to predict loan defaults using real-world data.

## 🔍 Project Overview

This work investigates the use of **machine learning algorithms** to assess the risk of **loan default** based on data provided by [Home Credit Group](https://www.homecredit.net/), through a public Kaggle competition. The goal is to compare traditional and advanced approaches for credit risk assessment and explore how **data-driven methods** can improve loan allocation decisions.

Key components of the project include:
- **Data cleaning and preprocessing**
- **Automatic feature engineering using Deep Feature Synthesis (DFS)**
- **Feature selection using statistical methods**
- **Model training and evaluation** on various algorithms

## 🧠 Models Implemented

The following machine learning models were trained and compared:
- Logistic Regression
- Random Forest
- Gradient Boosting
- Artificial Neural Networks
- Anomaly Detection using Support Vector Machines (SVM)

Each model was trained using a consistent pipeline and evaluated on the same dataset.

## 📁 Repository Structure

```
├── images/                # Visualizations and illustrations used in the report
├── literature/            # Some Research papers referenced in the study
├── notebooks/             # Jupyter notebooks for each modeling and preprocessing task
├── texFiles/              # LaTeX source files for the thesis report
├── UndergraduateFinal.pdf # Final thesis document (in French)
└── README.md              # You're here!
```

## 📊 Dataset

The dataset was derived from the **Home Credit Default Risk** Kaggle competition. After preprocessing, the final dataset contained:
- **1,526,659 samples**
- **100 selected features**
- **Binary target**: loan repaid (0) or default (1)

⚠️ **Important Note on Licensing**:  
The **code** in this repository is released under the MIT License. However, the data (available on Kaggle) are derived from a Kaggle competition and may be subject to different licensing terms as specified by the competition organizers. Please refer to the [original dataset page](https://www.kaggle.com/competitions/home-credit-default-risk) for more information.

## 🛠 Feature Engineering

One highlight of the project is the use of **automated feature engineering** via [Featuretools](https://www.featuretools.com/) and **parallelization** using [Dask](https://www.dask.org/). The raw relational data was transformed into meaningful predictors through a scalable pipeline that processed millions of rows in under 24 hours on Kaggle VMs (accessed through kaggle notebooks).

## 📈 Evaluation

Models were evaluated using:
- Accuracy
- Precision
- Recall
- ROC AUC

A comparative study is provided in the final chapter of the [thesis PDF](./UndergraduateFinal.pdf).

## 📚 References

See the `literature/` folder for some key references and academic papers consulted during this project.

## 💡 Potential future Works

Some perspectives explored include:
- Incorporating fairness-aware ML to reduce bias
- Extending the pipeline to other types of credit products

## 🤝 Acknowledgments

Thanks to:
- **Dr. Maïga Oumar**, my thesis supervisor
- The **Kaggle community** and **Home Credit Group** for the data
