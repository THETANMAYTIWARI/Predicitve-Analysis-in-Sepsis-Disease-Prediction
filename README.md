## 🧬 Sepsis Disease Prediction

This project focuses on predicting Sepsis in patients using Machine Learning techniques applied on clinical datasets collected from multiple hospitals. The goal is to build a predictive model that can identify whether a patient is likely to develop Sepsis based on physiological and laboratory measurements.

### 🧠 Project Overview

Sepsis is a life-threatening condition that occurs when the body's response to infection causes tissue damage, organ failure, or death. Early detection and intervention can drastically improve patient outcomes.
In this project, multiple hospital datasets are used to build and compare various machine learning models that predict Sepsis based on patient data.

### ⚙️ Technologies Used
```
Python 3

Pandas and NumPy – Data manipulation and analysis

Matplotlib and Seaborn – Data visualization

Scikit-learn – Machine Learning models and evaluation metrics

Joblib / Pickle – Model saving and loading
```

### 📊 Methodology
1.	Data Collection & Cleaning
o	Imported datasets from multiple hospitals.
o	Handled missing values and removed redundant columns.
2.	Exploratory Data Analysis (EDA)
o	Visualized class imbalance using pie and count plots.
o	Studied feature distributions and correlations.
3.	Resampling
o	Used sklearn.utils.resample() to balance Sepsis (1) and Non-Sepsis (0) classes.
4.	Feature Selection
o	Selected 40 relevant features as predictors.
o	Encoded target labels (SepsisLabel).
5.	Model Building
o	Trained multiple classifiers:
	MLP Classifier (Neural Network)
	AdaBoost Classifier
	Linear Discriminant Analysis (LDA)
	Gaussian Naive Bayes
o	Compared accuracy and log-loss metrics.
6.	Model Evaluation
o	Evaluated using Confusion Matrix, Accuracy, Log-Loss, ROC Curve.
o	MLPClassifier achieved the highest accuracy (~91%).
7.	Model Deployment
o	Trained model saved as finalized_model.sav and finalized_model2.sav.
