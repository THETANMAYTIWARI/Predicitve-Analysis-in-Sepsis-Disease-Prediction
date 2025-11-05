## 🧬 Sepsis Disease Prediction

This project focuses on predicting Sepsis in patients using Machine Learning techniques applied on clinical datasets collected from multiple hospitals. The goal is to build a predictive model that can identify whether a patient is likely to develop Sepsis based on physiological and laboratory measurements.

### 🧠 Project Overview

Sepsis is a life-threatening condition that occurs when the body's response to infection causes tissue damage, organ failure, or death. Early detection and intervention can drastically improve patient outcomes.
In this project, multiple hospital datasets are used to build and compare various machine learning models that predict Sepsis based on patient data.

### ⚙️ Technologies Used

🔹 Python 3

* Pandas and NumPy – Data manipulation and analysis

* Matplotlib and Seaborn – Data visualization

* Scikit-learn – Machine Learning models and evaluation metrics

* Joblib / Pickle – Model saving and loading


### 📊 Methodology

🔹 Data Collection & Cleaning

* Imported datasets.

* Handled missing values and removed redundant columns.

🔹 Data Analysis & Visualization (EDA)

* Visualized class imbalance using pie and count plots.

* Explored feature distributions and correlations for better understanding.

🔹 Model Development & Evaluation

* Used sklearn.utils.resample() to balance Sepsis (1) and Non-Sepsis (0) classes.

* Selected 40 relevant features and encoded target labels (SepsisLabel).

  🔹 Trained multiple classifiers:

  * MLP Classifier (Neural Network)

  * AdaBoost Classifier

  * Linear Discriminant Analysis (LDA)

  * Gaussian Naive Bayes

* Compared models using Accuracy, Log-Loss, Confusion Matrix, and ROC Curve.

* MLP Classifier achieved the highest accuracy (~91%).

🔹 Model Deployment

* Saved trained models as finalized_model.sav and finalized_model2.sav for reuse and inference.

### 📈 Results
```
🧠 Model	🎯 Accuracy (%)	📉 Log Loss	🔍 Remarks
MLP Classifier (Neural Network)	91.0	Lowest	Best performing model
AdaBoost Classifier	87.5	Moderate	Good generalization
Linear Discriminant Analysis (LDA)	84.2	Higher	Stable baseline model
Gaussian Naive Bayes	82.3	Higher	Fast but less accurate
```
The MLP Classifier provided the most reliable predictions, outperforming other algorithms.

### 🩺 Example Visualizations

* Class Distribution of Sepsis vs Non-Sepsis Patients

* Confusion Matrix

* ROC Curve for model evaluation

* Feature-wise histograms and density plots for patient records

### 💾 Model Files

* Projectfinalized_model.sav – Trained model for 1st hospital dataset

* Projectfinalized_model2.sav – Trained model for 2nd hospital dataset

### 🧩 Future Improvements

* Incorporate more hospital datasets for better generalization.

* Experiment with advanced models (XGBoost, LSTM, etc.).

* Develop a Flask or Streamlit web app for real-time Sepsis prediction.


