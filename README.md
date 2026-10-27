Disease Prediction from Clinical Symptoms
Overview
This project explores the use of machine learning to predict diseases based on reported clinical symptoms. It focuses on data preprocessing, symptom representation, feature selection, model training, and evaluation.
The project compares four classification algorithms to investigate their performance in a multi-class disease prediction task.
Objectives
Clean and prepare the symptom dataset.
Represent symptoms as binary features.
Select the most informative symptoms using Mutual Information.
Train and compare different machine learning classifiers.
Evaluate model performance using multiple classification metrics.
Dataset
The project uses the Disease Symptom Prediction dataset published on Kaggle.
According to the project report, the original dataset contains 4,920 records, 131 distinct symptoms, and 41 disease classes. After removing duplicate records, 304 unique records remain.
The project also references supporting files containing symptom severity weights, disease descriptions, and recommended precautions.
Methodology
Data Preprocessing: Clean symptom and disease names, resolve formatting inconsistencies, and remove duplicate records.
Symptom Encoding: Convert symptom lists into binary features, where 1 indicates a present symptom and 0 indicates an absent symptom.
Feature Selection: Select the 30 most informative symptoms using Mutual Information.
Data Splitting: Split the data into 80% training and 20% testing sets using stratification.
Model Training: Tune model hyperparameters using GridSearchCV and stratified 3-fold cross-validation on the training set.
Model Evaluation: Compare the models using classification metrics and execution time.
Machine Learning Models
The following classifiers are compared:
Logistic Regression
Support Vector Machine (SVM)
Random Forest
Multi-Layer Perceptron (MLP)
Evaluation Metrics
Accuracy
Precision
Recall
F1-score
Confusion Matrix
Training and prediction time
Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Google Colab
Jupyter Notebook
Project Files
Disease_Prediction_Clean.ipynb — Notebook containing the data preparation, feature selection, model training, and evaluation workflow.
Disease_Prediction_Report_Combined.docx — Detailed project report documenting the methodology and analysis.
Important Limitation
This project is an academic machine learning experiment, not a clinically validated diagnostic system. The dataset contains substantial duplication and highly structured symptom patterns. Therefore, evaluation results should be interpreted cautiously and should not be considered evidence of real-world medical diagnostic accuracy.
Future Improvements
Dataset Source and License

The dataset was obtained from Disease Symptom Prediction on Kaggle.

The dataset page specifies the CC BY-SA 4.0 license. Please refer to the original source and license terms for attribution and redistribution requirements.
Evaluate the models on larger and more diverse datasets.
Test generalization using independent patient data.
Improve the reliability and clinical relevance of the prediction process.
Disclaimer
This project is intended for educational and research purposes only. It must not be used as a substitute for professional medical advice, diagnosis, or treatment.
