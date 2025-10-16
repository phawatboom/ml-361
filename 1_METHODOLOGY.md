# Methodology

## 1. Data Acquisition
Data were imported via CSV or Excel using pandas. Initial inspection involved:
```python
df.head(), df.info(), df.describe()
```

## 2. Data Cleaning
- **Missing Values:** handled through imputation or row-wise removal.  
- **Outliers:** identified with inter-quartile range and winsorization (±10%).  
- **Type Normalization:** ensured consistent numeric, date, and categorical formats.  
- **Derived Features:** created rolling statistics (AR(1) correlation, volatility, momentum).

## 3. Exploratory Data Analysis (EDA)
Exploration combined summary statistics and visualization:
- Distribution plots for central tendency and skewness  
- Correlation heatmaps for multicollinearity checks  
- Boxplots and pairplots for variance and relationships  

## 4. Analytical Techniques
Depending on dataset type:
- **Descriptive Statistics:** mean, variance, z-scores  
- **Correlation & Regression:** to quantify relationships  
- **Visualization-Driven Insight:** trend and clustering identification  
- **Model Evaluation:** accuracy, error metrics, or probability calibration  

## 5. Reproducibility
Each step is encapsulated in Jupyter cells for easy rerun, parameter changes, and result exports.  
