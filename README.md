# 📦 Predictive Modeling and Optimization for Shipment Delay in Logistics

This repository presents a complete machine learning framework to **predict shipment delays** and **optimize logistics operations** using models like Logistic Regression, Random Forest, and Gradient Boosting. The project combines **predictive analytics** and **optimization strategies**, delivering actionable insights for real-world supply chain applications.

---

## 📚 Literature Review

This work builds upon the foundation of research in predictive supply chain analytics:

- **Wang et al. (2016)**: Introduced real-time transportation data in predictive logistics modeling.
- **Baryannis et al. (2018)**: Showed the integration of AI and machine learning for managing disruptions using structured/unstructured data.
- **De Santis et al. (2017)**: Used predictive models to optimize inventory and prevent backorders.
- **Winkenbach et al. (2020)**: Emphasized dynamic route optimization using real-time traffic and weather data.

> Key takeaway: **Machine learning models like Random Forest and Gradient Boosting outperform traditional methods in delay prediction accuracy and logistics optimization.**

---

## ⚙️ Methodology

### 🔸 Dataset
- Public logistics dataset with features:
  - Shipment weight
  - Delivery urgency
  - Shipping mode
  - Distance
  - Delay status (binary)

### 🔸 Preprocessing
- **Imputation**: Mean/median for numerical, mode for categorical
- **Outlier Removal**: Z-score and IQR method
- **Normalization**: Min-max scaling
- **Encoding**: One-hot for nominal, label encoding for ordinal features
- **Feature Engineering**:
  - Weight-to-Distance Ratio
  - Shipment Priority Score

### 🔸 Models Implemented
- **Logistic Regression**
- **Random Forest Classifier & Regressor**
- **Gradient Boosting Classifier & Regressor**

### 🔸 Optimization
- Hyperparameter tuning using **Grid Search** and **Genetic Algorithms**
- Evaluated on 80-20 train-test split with cross-validation

---

## 📊 Results

### 📈 Classification Performance

| Model              | Accuracy | Precision | Recall | F1-Score |
|--------------------|----------|-----------|--------|----------|
| Logistic Regression | 78%      | 72%       | 74%    | 73%      |
| Random Forest       | 88%      | 85%       | 87%    | 86%      |
| Gradient Boosting   | 86%      | 83%       | 85%    | 84%      |

### 🔍 Detailed Class-wise Metrics

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.46      | 0.60   | 0.52     | 45      |
| 1     | 0.56      | 0.42   | 0.48     | 55      |

**Accuracy**: 50% (on imbalanced subset)  
**Macro Avg F1-Score**: 0.50  
**Weighted Avg F1-Score**: 0.50

### 📉 Regression Metrics

| Model                  | MSE   | R² Score |
|------------------------|-------|----------|
| Random Forest Regressor | 25.56 | 0.71     |
| Gradient Boosting Regressor | 25.10 | 0.71     |

---

## 📌 Key Observations

- **Random Forest** showed the best classification and regression performance.
- **Gradient Boosting** handled imbalanced datasets better with slight trade-offs in accuracy.
- **Logistic Regression** is interpretable but underperforms with non-linear data.
- Genetic Algorithm tuning improved model performance significantly.

---

## 📷 Visualizations

- 📦 Box Plot of Weight by Shipment Mode  
- 📊 Count Plot for Shipment Modes  
- 💡 Feature Importances (RF vs GB)  
- 🔍 Logistic Regression Coefficients  
- 🔄 Comparison of Random Forest vs Gradient Boosting  

(All plots available in `/figures/` folder)

---

## 🏁 Conclusion

This project demonstrates the power of combining **domain-specific feature engineering**, **ensemble models**, and **hyperparameter optimization** to solve complex logistics problems like shipment delays.

By fusing predictive modeling with optimization, this framework supports **real-time decision making** and **operational resilience** in supply chain systems.

---

## 📂 Folder Structure

```
├── data/
│   └── shipment_data.csv
├── notebooks/
│   └── exploratory_analysis.ipynb
├── models/
│   └── trained_models.pkl
├── figures/
│   └── *.png
├── README.md
└── report/
    └── full_latex_report.pdf
```

---

## 📌 Technologies

- Python (NumPy, pandas, scikit-learn, matplotlib, seaborn)
- Jupyter Notebooks
- LaTeX (for report)
- Genetic Algorithm (from DEAP/TPOT or custom)

---

## 📬 Contact

For queries or collaborations, feel free to reach out:

**Name**: *Sayantan Mandal*  
**Email**: *msayantan05@gmail.com*  
**GitHub**: [your-username](https://github.com/sayantanmandal1)
