# 🧠 Breast Cancer Classification using SVM

## 📌 Project Overview
This project implements a **Support Vector Machine (SVM)** model to classify breast cancer tumors as **malignant** or **benign**.  
The objective is to understand **kernel-based classification**, **feature scaling**, and **hyperparameter tuning** while achieving high predictive accuracy.

---

## 🧰 Tools & Technologies
- Python  
- Scikit-learn  
- Matplotlib  

**Alternative Tools (Conceptual):**
- Weka  
- R (caret)

---

## 📂 Dataset Information
- **Dataset:** Breast Cancer Dataset (Kaggle / Scikit-learn)
- **Total Samples:** 569
- **Number of Features:** 30
- **Target Classes:**
  - `0` → Malignant  
  - `1` → Benign  

---

## ⚙️ Dataset Split
The dataset was split using an **80:20 train–test ratio**:

| Split | Samples |
|------|---------|
| Training Set | 455 |
| Testing Set | 114 |

---

## ⚙️ Project Workflow
1. Loaded the dataset and inspected features and label distribution  
2. Applied **StandardScaler** to normalize feature values  
3. Split data into training and testing sets  
4. Trained a baseline SVM with **linear kernel**  
5. Trained SVM with **RBF kernel** and compared accuracy  
6. Tuned hyperparameters (`C`, `gamma`) using **GridSearchCV**  
7. Evaluated the best model using test accuracy and confusion matrix  
8. Plotted **ROC curve** and calculated **AUC score**  
9. Saved the tuned model pipeline (Scaler + SVM) for reuse  

---

## 📈 Model Performance
- **Test Accuracy:** **97%**
- The model demonstrates strong generalization on unseen data
- High accuracy indicates effective separation of malignant and benign tumors

---

## 📊 ROC Curve & AUC
- ROC curve visualizes classifier performance across different thresholds
- High AUC value indicates excellent discrimination capability

---

## 📦 Deliverables
✔ Jupyter Notebook  
✔ ROC Curve & AUC Plot  
✔ Saved Model File (`svm_breast_cancer_model.pkl`)  

---

## 🧠 Key Insights
- Feature scaling is essential for SVM models  
- RBF kernel captures non-linear patterns effectively  
- Hyperparameter tuning improves performance significantly  
- SVM is well-suited for medical diagnosis tasks  

---

## 📌 Conclusion
The Support Vector Machine model achieved **97% test accuracy**, showing excellent performance in breast cancer classification.  
This project highlights the importance of preprocessing, kernel selection, and model tuning in healthcare-related machine learning tasks.

---

## ▶️ How to Run the Project
1. Clone the repository  
2. Install required libraries  
   ```bash
   pip install numpy pandas scikit-learn matplotlib
