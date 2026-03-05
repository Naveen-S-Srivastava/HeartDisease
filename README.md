# ❤️ Heart Disease Prediction (Machine Learning)

This project builds a **machine learning model to predict heart disease** using patient health data.
The dataset is analyzed, visualized, processed, and then used to train a **Logistic Regression classifier** that predicts whether a person is likely to have heart disease.

The model achieves **~86.8% accuracy** on the test dataset.

---

# 📊 Dataset

The dataset used in this project is publicly available:

https://raw.githubusercontent.com/amankharwal/Website-data/master/heart.csv

It contains **303 patient records** with multiple medical attributes.

### Features in the dataset

| Feature  | Description                                    |
| -------- | ---------------------------------------------- |
| age      | Age of the patient                             |
| sex      | Gender (1 = male, 0 = female)                  |
| cp       | Chest pain type                                |
| trestbps | Resting blood pressure                         |
| chol     | Serum cholesterol                              |
| fbs      | Fasting blood sugar                            |
| restecg  | Resting ECG results                            |
| thalach  | Maximum heart rate achieved                    |
| exang    | Exercise induced angina                        |
| oldpeak  | ST depression induced by exercise              |
| slope    | Slope of peak exercise ST segment              |
| ca       | Number of major vessels colored by fluoroscopy |
| thal     | Thalassemia                                    |
| target   | Heart disease presence (1 = yes, 0 = no)       |

---

# 🔍 Project Workflow

The project follows a typical **machine learning pipeline**:

1. Data loading
2. Data exploration
3. Data visualization
4. Feature preprocessing
5. Feature scaling
6. Train/Test split
7. Model training
8. Model evaluation

---

# 📈 Exploratory Data Analysis

Some key steps performed during EDA:

* Checking dataset structure
* Handling missing values
* Summary statistics
* Correlation analysis
* Feature distribution analysis

### Correlation Matrix

A heatmap is generated to understand relationships between features.

This helps identify which variables influence the **target variable (heart disease)**.

---

# ⚙️ Data Preprocessing

Several preprocessing steps were applied:

### 1. Categorical Encoding

Categorical variables were converted using **one-hot encoding**.

```
pd.get_dummies()
```

### 2. Feature Scaling

Continuous variables were standardized using **StandardScaler**.

```
StandardScaler()
```

Scaled columns:

* age
* trestbps
* chol
* thalach
* oldpeak

---

# 🤖 Machine Learning Model

The model used:

### Logistic Regression

Logistic Regression is commonly used for **binary classification problems** like predicting disease presence.

```
LogisticRegression(solver='liblinear')
```

---

# 📊 Model Evaluation

The model performance was evaluated using:

* Accuracy Score
* Classification Report
* Confusion Matrix

### Training Results

Accuracy: **86.79%**

Confusion Matrix

```
[[80 17]
 [11 104]]
```

---

### Testing Results

Accuracy: **86.81%**

Confusion Matrix

```
[[34 7]
 [5 45]]
```

The similar train and test accuracy suggests **minimal overfitting**.

---

# 📉 Model Performance Summary

| Model               | Training Accuracy | Testing Accuracy |
| ------------------- | ----------------- | ---------------- |
| Logistic Regression | 86.79%            | 86.81%           |

---

# 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

# 🚀 How to Run the Project

1. Clone the repository

```
git clone https://github.com/yourusername/heart-disease-prediction.git
```

2. Install dependencies

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. Run the Python script

```
python heart_disease_prediction.py
```

---

# 📌 Future Improvements

Possible improvements for the project:

* Try additional ML models

  * Random Forest
  * Support Vector Machine
  * XGBoost

* Perform hyperparameter tuning

* Build a web interface using **Flask or Streamlit**

* Deploy the model

---

# 📚 Learning Outcomes

This project demonstrates:

* Data preprocessing
* Exploratory data analysis
* Feature scaling
* Logistic regression for classification
* Model evaluation using confusion matrix and classification reports

---

# ⭐ If you found this project useful

Give the repo a ⭐ and feel free to contribute!
