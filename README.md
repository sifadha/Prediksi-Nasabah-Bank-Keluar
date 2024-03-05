# Analisa-Prediksi-Nasabah-Bank-Keluar

## Final Project
Project ini merupakan persyaratan kelulusan pada bootcamp yang saya ikuti. Dengan judul "Analisa Prediksi Nasabah Bank Keluar", project ini saya mengerjakan model prediksi yang dapat mengidentifikasi faktor penting yang mempengaruhi nasabah bank keluar.

## Data
Data yang digunakan bersumber pada:
* Kaggle: https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn/code

Dataset ini mengandung 10000 baris dan 18 kolom dengan detail nama kolom:
CustomerID, Surname, CreditScore, Geography, Gender, Age, Tenure, Balance, NumOfProducts, HasCrCard, IsActiveMember, Estimated Salary, Exited, Complain, Satisfaction Score, Card Type, Point Earned.

## EDA Questions
1. Jumlah total customer keluar (Exited) dan mengajukan 'Complain'.
2. Jumlah customer yang keluar (Exited) berdasarkan 'Geography' dan 'Gender'.
3. Jumlah customer yang keluar (Exited) berdasarkan 'HasCrCard' dan 'Gender'.
4. Nilai rata-rata, median, maksimum, dan minimum dari kolom CreditScore, Age, Tenure, Balance, NumOfProducts, EstimatedSalary.
5. Distribusi customer yang keluar.
6. Distribusi customer berdasarkan 'Satisfaction Score'.
7. Rata-rata 'Tenure' dari customer yang keluar dan customer yang masih aktif.
8. Perbandingan jumlah customer yang complain berdasarkan 'Exited' dan 'Gender'.
9. Distribusi umur customer.

## Library

- import numpy as np
- import pandas as pd
- import seaborn as sns
- import matplotlib.pyplot as plt
- from sklearn.model_selection import GridSearchCV
- from sklearn.model_selection import KFold
- from sklearn.model_selection import cross_validate, StratifiedKFold, RandomizedSearchCV, cross_val_score
- from sklearn import svm,tree
- from sklearn import ensemble
- from sklearn.linear_model import LogisticRegression
- from sklearn.tree import DecisionTreeClassifier
- from sklearn.neighbors import KNeighborsClassifier
- from sklearn.naive_bayes import GaussianNB
- from sklearn.svm import SVC
- from sklearn.ensemble import RandomForestClassifier
- from sklearn import metrics
- from sklearn.metrics import confusion_matrix
- from sklearn.metrics import auc,roc_auc_score
- from sklearn.metrics import roc_auc_score, roc_curve, RocCurveDisplay, precision_recall_curve, PrecisionRecallDisplay
- from sklearn.model_selection import train_test_split as tts
- from sklearn import model_selection
