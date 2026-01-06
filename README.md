# 🫀 Heart Disease Prediction using Machine Learning (KNN)

This project focuses on building a **Heart Disease Prediction System** using a **K-Nearest Neighbors (KNN)** classification model.  
The workflow follows a complete **machine learning pipeline**, starting from data cleaning and preprocessing, handling class imbalance, model training, evaluation, and finally deploying an interactive prediction interface using **Gradio**.

---

## 📂 Dataset

- **File name:** `Heart_Disease dataset.csv`
- **Target variable:** `HeartDisease` (Yes / No)
- **Problem type:** Binary Classification

### 🔑 Features Include:
- BMI  
- Physical Health  
- Mental Health  
- Sleep Time  
- Smoking  
- Alcohol Drinking  
- Stroke  
- Difficulty Walking  
- Sex  
- Age Category  
- Race  
- Diabetic  
- Physical Activity  
- General Health  
- Asthma  
- Kidney Disease  
- Skin Cancer  

---

## 🛠️ Data Preprocessing

The following preprocessing steps were applied:

1. **Handling Missing Values**
   - Numerical features → filled using **Median**
   - Categorical features → filled using **Mode**

2. **Removing Duplicates**
   - Duplicate rows were detected and removed to ensure data quality.

3. **Encoding**
   - Categorical features were encoded using **One-Hot Encoding**
   - Target variable:
     - `Yes → 1`
     - `No → 0`

4. **Feature Scaling**
   - Applied **StandardScaler** to normalize numerical values before model training.

---

## ⚖️ Handling Class Imbalance

- The dataset was imbalanced.
- **SMOTE (Synthetic Minority Oversampling Technique)** was applied to balance the classes before training.

---

## 🤖 Model Used

- **Algorithm:** K-Nearest Neighbors (KNN)
- **Number of neighbors (k):** 5
- **Distance-based classification**
- Trained on scaled features for better performance.

---

## 📊 Model Evaluation

The model was evaluated using:

- **Confusion Matrix**
- **Accuracy Score**
- **Classification Report**
  - Precision
  - Recall
  - F1-score

A heatmap visualization was used to clearly display the confusion matrix results.

---

## 🧪 Libraries Used

- `pandas`
- `numpy`
- `scikit-learn`
- `imblearn`
- `matplotlib`
- `seaborn`
- `gradio`

---

## 🌐 Interactive Web Application (Gradio)

An interactive **Gradio web interface** was developed that allows users to:

- Enter patient medical and lifestyle data
- Receive:
  - Heart disease prediction (Yes / No)
  - Estimated probability of heart disease

### 🖥️ Features of the UI:
- User-friendly sliders and dropdowns
- Input validation (ranges for numerical values)
- Real-time prediction
- Clean and modern interface

---

##👨‍🎓 Author
Heart Disease Prediction Project Built for learning and academic purposes in Data Science & Machine Learning.

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/heart-disease-prediction.git
