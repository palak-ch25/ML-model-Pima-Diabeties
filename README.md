# Diabetes Outcome Prediction using Logistic Regression

This repository contains a Data Science and Machine Learning workflow for analyzing patient health data and predicting the likelihood of diabetes using **Logistic Regression**. The project covers data loading, exploratory data analysis (EDA), missing value verification, target distribution visualization, feature scaling, and model evaluation.

---

## 📋 Table of Contents
- [Overview](#-overview)
- [Dataset Details](#-dataset-details)
- [Project Workflow](#-project-workflow)
- [Tech Stack](#%EF%B8%8F-tech-stack)
- [Project Structure](#-project-structure)
- [Setup & Installation](#%EF%B8%8F-setup--installation)
- [Results & Visualization](#-results--visualization)

---

## 🎯 Overview
The primary goal of this project is to build a classification model that predicts whether a patient has diabetes based on medical diagnostic measurements.

* **Task:** Binary Classification
* **Target Variable:** `Outcome` (`1` = Diabetic, `0` = Non-Diabetic)
* **Algorithm:** Logistic Regression

---

## 📊 Dataset Details
The dataset used in this project is the **PIMA Indian Diabetes Dataset** (768 rows, 9 columns).

### Features
| Column Name | Description | Data Type |
| :--- | :--- | :--- |
| `Pregnancies` | Number of times pregnant | `int64` |
| `Glucose` | Plasma glucose concentration (2 hours in an oral glucose tolerance test) | `int64` |
| `BloodPressure` | Diastolic blood pressure (mm Hg) | `float64` |
| `SkinThickness` | Triceps skinfold thickness (mm) | `int64` |
| `Insulin` | 2-Hour serum insulin (mu U/ml) | `float64` |
| `BMI` | Body mass index (weight in kg / (height in m)^2) | `float64` |
| `DiabetesPedigreeFunction` | Diabetes pedigree function (genetic score) | `float64` |
| `Age` | Age in years | `int64` |
| **`Outcome`** | Class variable (**0** or **1**) | `int64` |

---

## 🔄 Project Workflow
1. **Library Import:** Essential Python libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`) are imported.
2. **Data Ingestion:** Loads `diabetes.csv` into a Pandas DataFrame.
3. **Exploratory Data Analysis (EDA):**
   * Inspecting top rows (`head()`)
   * Dataset shape and variable types (`shape`, `info()`)
   * Statistical summary (`describe()`)
   * Null/Missing value checks (`isnull().sum()`)
   * Value counts of the target label (`value_counts()`)
4. **Data Visualization:** Distribution plot of diabetic vs. non-diabetic outcomes using Seaborn countplots.
5. **Model Building & Training:** 
   * Data splitting (`train_test_split`)
   * Feature Standardization (`StandardScaler`)
   * Fitting a `LogisticRegression` classifier
6. **Model Evaluation:** Performance assessment using Accuracy Score, Confusion Matrix, and Classification Report.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Environment:** Jupyter Notebook
* **Libraries:**
  * **Data Manipulation:** `pandas`, `numpy`
  * **Data Visualization:** `matplotlib`, `seaborn`
  * **Machine Learning:** `scikit-learn`

