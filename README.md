📌 Overview
This repository presents a machine learning–based voice pathology detection system using a novel Progressive Acoustic Stacking (PAS) framework. The approach incrementally fuses multiple acoustic feature families to improve classification performance over traditional single-feature or flat-fusion methods.

🧠 Key Idea: Progressive Acoustic Stacking (PAS)
Instead of concatenating all features at once, PAS adds feature groups step-by-step and evaluates their contribution:
PAS Level	Features Used:
i.Level-1:	MFCC
ii.Level-2:	MFCC + LPC
iii.Level-3:	MFCC + LPC + Formants
iv.Level-4:	MFCC + LPC + Formants + Phase
v.Each stage demonstrates measurable performance improvement.

🗂 Dataset
Dataset: German Voice Disorder Dataset
Classes: Healthy vs Pathological
🔗 Download link:https://www.kaggle.com/datasets/sree14hari/svd-dataset/data

⚙️ Feature Extraction
i.MFCC (Mel-Frequency Cepstral Coefficients)
ii.LPC (Linear Predictive Coding)
iii.Formant Frequencies (F1–F3)
iv.Phase-based Features

🤖 Models Used
i.Support Vector Machine (SVM)
ii.Random Forest
iii.Naive Bayes
iv.Logistic Regression

📊 Evaluation Metrics
i.Accuracy
ii.Sensitivity (Recall)
iii.Specificity
iv.G-Mean
v.Confusion Matrix

🧪 Results Summary
S.NO.         Model	       Best PAS Level	          Accuracy
  1.          SVM	           Level-4	              Highest
  2.          RF	           Level-4	               High
  3.          KNN	           Level-3	             Moderate
  4.          LR	           Level-2	              Lower

Progressive feature stacking consistently outperformed single-feature models.
