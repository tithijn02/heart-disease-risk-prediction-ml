# ❤️ Heart Disease Risk Prediction using Machine Learning

Early detection of heart disease can significantly improve outcomes — this project builds predictive models to identify high-risk individuals while balancing accuracy, interpretability, and real-world clinical priorities.

---

## 🚨 The Problem

Coronary heart disease is one of the leading causes of mortality, yet identifying high-risk individuals early remains challenging. Traditional approaches often struggle with noisy clinical data, class imbalance, and the need to balance predictive performance with interpretability.

This leads to:
- missed high-risk patients (false negatives)  
- over-reliance on black-box models in sensitive domains  
- difficulty translating model outputs into clinical decisions  

---

## 💡 The Solution

This project develops a structured machine learning pipeline to predict heart disease risk using patient data. Multiple models were evaluated, with a strong focus on selecting an approach that not only performs well but is also interpretable and clinically meaningful.

Instead of optimizing purely for accuracy, the solution prioritizes recall for high-risk cases, aligning with real-world medical decision-making where missing a diagnosis is more costly than over-predicting risk.

---

## 📊 Business Impact

The model supports early risk identification and can act as a decision-support tool in clinical environments.

This enables:
- improved screening of high-risk patients  
- better allocation of medical resources  
- reduced risk of undiagnosed heart disease  
- more explainable and trustworthy predictions in healthcare settings  

---

## 🛠️ How it was done

The analysis uses a clinical dataset of 462 patients with features such as age, cholesterol (LDL), blood pressure (SBP), tobacco usage, and family history.

Exploratory analysis revealed strong skewness and outliers in variables like tobacco and alcohol, which were retained to preserve real-world risk patterns. Feature relationships showed that age, tobacco, and LDL were key predictors of heart disease.

A ridge-regularized logistic regression model was used to handle multicollinearity and outliers, achieving an AUC of 0.80 with balanced performance. To improve detection of high-risk cases, class imbalance was addressed using weighted models, increasing recall for heart disease cases to 88%.

Multiple classifiers were evaluated, with Linear Discriminant Analysis (LDA) selected as the final model due to its strong performance, interpretability, and suitability for clinical use. It achieved ~73% accuracy and strong discriminative ability while remaining computationally efficient and explainable.

---

## 📄 Full Case Study

👉 [View Report](./Report.pdf)
