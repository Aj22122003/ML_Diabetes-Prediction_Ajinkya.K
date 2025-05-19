# 🩺 Diabetes Prediction Project 📊

[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Aj22122003/ML_Diabetes-Prediction_Ajinkya.K/graphs/commit-activity)
[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Predicting whether a person has diabetes or not using machine learning.**

This project leverages a dataset containing various features like Pregnancies, Glucose, BloodPressure, SkinThickness, BMI, Insulin, DiabetesPedigreeFunction, and Age to build predictive models for diabetes.

## 🎯 Project Goal

The primary objective is to accurately predict if an individual has diabetes based on the provided health-related features. This involves:

- **Data Preprocessing:** Handling missing values and preparing the data for machine learning models.
- **Feature Engineering:** (Implicitly done by replacing 0 with the mean for specific features)
- **Model Implementation:** Training and evaluating several classification algorithms.
- **Performance Comparison:** Identifying the best-performing model for diabetes prediction.

## ✨ What I've Done

This project involved a comprehensive machine learning workflow:

1.  **Data Loading and Preprocessing:** Libraries were used to load and preprocess the dataset. A key step involved addressing missing values (represented as 0 in certain features) by replacing them with the mean of that particular feature, assuming a strong relationship between the variables.
2.  **Data Standardization:** Standardization was applied to the features to ensure they have a mean of 0 and a standard deviation of 1. This is crucial for algorithms sensitive to feature scaling.
3.  **Data Splitting:** The dataset was divided into training and testing sets (80% for training and 20% for testing) to evaluate the generalization ability of the models.
4.  **Classification Model Implementation:** Several popular classification algorithms were implemented:
    - Logistic Regression
    - Decision Tree Classifier
    - Support Vector Machine (SVM)
    - Random Forest Classifier
5.  **Model Training and Evaluation:** Each model was trained on the training data, and its performance was evaluated on the testing data. The accuracy of each model was calculated and recorded.
6.  **Confusion Matrix Analysis:** The confusion matrix was likely analyzed to gain deeper insights into the models' performance, including true positives, true negatives, false positives, and false negatives.
7.  **Model Persistence:** The trained and evaluated models were saved using the `pickle` library, allowing for easy loading and deployment in the future.

## ⚙️ Models Used

The following machine learning models were implemented and evaluated:

- **Logistic Regression**
- **Decision Tree Classifier**
- **Support Vector Machine (SVM)**
- **Random Forest Classifier**

## 📊 Results

The following accuracies were achieved on the testing dataset for each model:

- **Logistic Regression:** Training Accuracy: $\approx 0.7688$, Testing Accuracy: $\approx 0.8182$
- **Decision Tree Classifier:** Training Accuracy: $1.00$, Testing Accuracy: $\approx 0.7597$
- **Support Vector Machine (SVM):** Training Accuracy: $\approx 0.8143$, Testing Accuracy: $\approx 0.7727$
- **Random Forest Classifier:** Training Accuracy: $1.00$, Testing Accuracy: $\approx 0.8182$

**Analysis:** Both the Random Forest and Logistic Regression models demonstrated the highest testing accuracy ($\approx 0.8182$). While the Decision Tree and Random Forest models achieved perfect accuracy on the training data, their testing accuracies suggest that Logistic Regression and Random Forest generalize slightly better to unseen data in this case. The Support Vector Machine also shows competitive performance.

Considering the high training accuracy and slightly lower testing accuracy of the Decision Tree and Random Forest, there might be a slight indication of overfitting. However, the Random Forest still maintains a strong testing accuracy.

**Conclusion:** The **Support Vector Machine (SVM)** algorithm is considered to have achieved relatively good scores compared to the Decision Tree and Logistic Regression.

## 🚀 Deployment

The trained models have been saved using the `pickle` library, making them ready for deployment in a real-world application.

## 🛠️ Technologies Used

- Python
- Libraries (likely including):
    - pandas
    - scikit-learn
    - pickle

## 📂 Repository Contents

(You can add more details here if you have other files in your repository, like data files, notebooks, etc.)

- `requirements.txt`: Lists the project dependencies.
- `README.md`: This file, providing an overview of the project.
- (Potentially other files like `.py` scripts, data files, notebooks, etc.)

## ⚙️ Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Aj22122003/ML_Diabetes-Prediction_Ajinkya.K.git](https://github.com/Aj22122003/ML_Diabetes-Prediction_Ajinkya.K.git)
    cd ML_Diabetes-Prediction_Ajinkya.K
    ```
2.  **Create a virtual environment (recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Linux/macOS
    venv\Scripts\activate  # On Windows
    ```
3.  **Install the required dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## 🚀 Usage

(Provide instructions on how to run your code or use the deployed model, if applicable.)

## 🙏 Acknowledgements

(You can acknowledge any datasets, libraries, or individuals that helped with this project.)

- The diabetes dataset used in this project.
- The developers and contributors of the Python libraries used (pandas, scikit-learn).

## 📄 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## ✍️ Author

[Ajinkya Kutarmare] ([https://github.com/Aj22122003/ML_Diabetes-Prediction_Ajinkya.K])
