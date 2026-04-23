#  Country Development Segmentation using K-Means & Hierarchical Clustering

##  Project Overview

This project applies unsupervised machine learning techniques to segment countries based on socio-economic and health indicators such as income, GDP per capita, life expectancy, child mortality, and fertility rate.

The goal is to group countries into meaningful categories like **Developed**, **Developing**, and **Underdeveloped**, enabling better understanding of global development patterns.

---

##  Objectives

* Perform Exploratory Data Analysis (EDA) to understand country-level data
* Apply clustering techniques to identify natural groupings
* Compare multiple clustering approaches
* Derive meaningful insights for country classification

---

##  Dataset Description

The dataset contains country-level features including:

* Income
* GDP per capita (gdpp)
* Inflation
* Imports & Exports
* Health expenditure
* Life expectancy
* Child mortality
* Total fertility rate

---

##  Exploratory Data Analysis (EDA)

Key observations:

* Income and GDP per capita show strong positive correlation
* Higher income countries tend to have higher life expectancy
* Child mortality is inversely related to income
* Fertility rates are higher in less developed countries
* Significant variation in feature scales required normalization

---

##  Methodology

### 1. Data Preprocessing

* Removed non-numeric columns (e.g., country names)
* Applied feature scaling using StandardScaler

---

### 2. Clustering Techniques

####  K-Means Clustering

* Used Elbow Method to determine optimal clusters
* Selected **K = 3** for better interpretability
* Segmented countries into:

  * Developed
  * Developing
  * Underdeveloped

---

####  Hierarchical Clustering

* Applied Agglomerative Clustering
* Used dendrogram to validate cluster structure
* Confirmed similar grouping patterns as K-Means

---

### 3. Model Evaluation

* Silhouette Score used for validation (~0.28)
* Slightly low due to overlapping real-world data
* Focus placed on interpretability and business meaning

---

##  Key Insights

* Developed countries exhibit:

  * High income
  * High life expectancy
  * Low child mortality

* Developing countries show moderate values across indicators

* Underdeveloped countries have:

  * Low income
  * High child mortality
  * Low life expectancy

* Strong inverse relationship between income and child mortality

---

##  Model Comparison

Both K-Means and Hierarchical Clustering produced **consistent segmentation patterns**, despite differences in cluster labels.

This validates the robustness of the clustering approach.

---

##  Visualization

* PCA used for dimensionality reduction
* Cluster visualization plotted using scatter plots

---

## 🧠 Conclusion

This project demonstrates how unsupervised learning can effectively identify hidden patterns in global data and classify countries based on development indicators.

---

##  Tech Stack

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn

---

##  Project Structure

```
country-segmentation/
│
├── notebook.ipynb
├── data/
├── README.md
└── requirements.txt
├──.gitignore

```

---

##  Future Improvements

* Add interactive dashboards (Power BI / Tableau)
* Include time-series analysis 
* Try advanced clustering techniques

---

## Author
Kusum Jangir

---
