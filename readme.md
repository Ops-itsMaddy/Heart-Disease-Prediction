# Heart Disease Prediction using Logistic Regression

This project implements a machine learning model to predict the presence of heart disease in patients based on various medical attributes. It uses a **Logistic Regression** approach, achieving high accuracy on both training and testing datasets.

## 📌 Project Overview

The goal of this project is to provide a predictive tool that can assist medical professionals in identifying potential heart conditions. The notebook covers the entire machine learning pipeline, including data loading, exploratory data analysis (EDA), model training, and a functional inference system.

## 📊 Dataset Description

The model is trained on a dataset containing 303 instances with 14 attributes:
* **age**: Age in years
* **sex**: (1 = male; 0 = female)
* **cp**: Chest pain type
* **trestbps**: Resting blood pressure
* **chol**: Serum cholesterol in mg/dl
* **fbs**: Fasting blood sugar > 120 mg/dl
* **restecg**: Resting electrocardiographic results
* **thalach**: Maximum heart rate achieved
* **exang**: Exercise induced angina
* **oldpeak**: ST depression induced by exercise relative to rest
* **slope**: The slope of the peak exercise ST segment
* **ca**: Number of major vessels (0-3) colored by flourosopy
* **thal**: Thalassemia (categorical)
* **target**: Diagnosis of heart disease (1 = Defective Heart, 0 = Healthy Heart)

## 🛠️ Project Workflow

1.  **Dependencies**: Importing libraries like `numpy`, `pandas`, and `scikit-learn`.
2.  **EDA**: Statistical analysis using `.describe()`, `.info()`, and `.groupby()` to understand feature distributions.
3.  **Preprocessing**: Splitting the data into features ($X$) and targets ($Y$), followed by a stratified train-test split.
4.  **Model Training**: Implementing a `LogisticRegression` model.
5.  **Evaluation**: Measuring performance using accuracy scores.
6.  **Predictive System**: A custom script to input raw medical data and receive a prediction.

## 📈 Performance

* **Training Accuracy**: ~85.12%
* **Testing Accuracy**: ~81.97%

## 🚀 How to Run
1.  Clone this repository.
2.  Ensure you have the dataset file `heart_disease_data.csv` in the root directory.
3.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4.  Run the Jupyter Notebook `Heart Disease Prediction.ipynb`.

## 🔮 Predictive System

The notebook includes a section to test individual cases. By providing a tuple of medical data, the system will output:
* `[1]` -> **The Person has Heart Disease**
* `[0]` -> **The Person does not have a Heart Disease**