# 🛒 Predict Customer's Future Purchases

**Author**: Tasnim Jahan  
**Repository**: `predict-customers-future-purchases`

This project focuses on predicting whether a customer will make a purchase within the next 90 days based on historical online retail data using machine learning and customer segmentation techniques.

---

## 📦 Files in This Repository

| File Name                                                | Description |
|----------------------------------------------------------|-------------|
| `_An_approach_to_Predict_Customer's_future_Purchases.ipynb`| Main Jupyter notebook for the entire analysis, visualization, and modeling pipeline |
| `README.md`                                                | Project overview and documentation |
| `Online_Retail.ipynb`                                      | Backup or initial draft version of the notebook |

---

## 🔍 Project Overview

Using the **Online Retail Dataset** from Kaggle, the project applies:

- **RFM analysis** (Recency, Frequency, Monetary Value)
- **KMeans clustering** for customer segmentation
- **Classification algorithms** to predict future purchases

---

## 📊 Workflow Summary

1. **Data Cleaning & Exploration**  
   - Remove nulls, convert dates, inspect country distributions.

2. **Feature Engineering**  
   - Add `Revenue` and `InvoiceYearMonth`.
   - Calculate RFM metrics and cluster customers using KMeans.

3. **Labeling Prediction Target**  
   - Define `NextPurchaseDayRange`:  
     `1` = Customer purchased within 90 days  
     `0` = No purchase within 90 days

4. **Segmentation**  
   - Cluster customers into **Low**, **Mid**, and **High-Value** groups.

5. **Modeling & Evaluation**  
   - Classifiers used: `LogisticRegression`, `DecisionTreeClassifier`, `RandomForestClassifier`, `GaussianNB`
   - Evaluation metrics: `Accuracy`, `F1 Score`, `Recall`, `Precision`

---

## 📈 Results Snapshot

| Model                   | Accuracy | F1 Score | Time (s) |
|------------------------|----------|----------|----------|
| Logistic Regression     | 98.71%   | 97.87%   | 0.18     |
| Decision Tree           | 98.52%   | 97.73%   | 0.03     |
| Random Forest           | 98.04%   | 96.96%   | 0.52     |
| Gaussian NB             | 97.07%   | 95.47%   | 0.04     |

✅ **Best Performer**: Logistic Regression  
⚡ **Fastest**: Decision Tree (with competitive performance)

---

## 📌 Key Visualizations

- Monthly revenue trends  
- Customer distribution by country  
- Revenue vs Frequency and Recency scatter plots  
- Cluster-based heatmaps and segmentations

---

## 🛠 Requirements

- Python 3.7+  
- pandas, numpy  
- scikit-learn  
- plotly, seaborn, matplotlib  
- xgboost (optional)  
- multiscorer

---

## 📁 Dataset

- Online Retail Dataset from UCI 
- Covers transactions between Dec 2009 – Dec 2011  
- Over 1 million rows

---

## 🙌 Acknowledgements

- Dataset by UCI  
- Inspired by real-world customer behavior modeling practices  
- Special thanks to Colab for notebook development

