# Customer Intelligence / Country Segmentation System

## Project Overview

This project applies **Unsupervised Machine Learning** techniques to segment countries based on socio-economic and health indicators. The objective is to identify groups of countries with similar characteristics and generate insights that can support policy-making, resource allocation, and international aid planning.

The project follows a complete clustering workflow including data preprocessing, feature scaling, K-Means clustering, DBSCAN clustering, PCA visualization, and cluster profiling.

---

## Dataset

**Dataset:** Country Data (Kaggle)

### Features

* country
* child_mort
* exports
* health
* imports
* income
* inflation
* life_expec
* total_fer
* gdpp

These features represent various economic, demographic, and healthcare indicators for countries around the world.

---

## Project Workflow

### 1. Data Inspection

* Load dataset
* Explore dataset structure
* Review summary statistics

### 2. Data Cleaning

* Remove duplicate records
* Handle missing values
* Convert columns to appropriate numeric types

### 3. Exploratory Data Analysis (EDA)

* Correlation heatmap
* Distribution analysis
* Boxplots for outlier detection

### 4. Feature Scaling

* StandardScaler used to normalize all numerical features

### 5. K-Means Clustering

* Elbow Method used to determine optimal cluster count
* Silhouette Score used to evaluate cluster quality

### 6. DBSCAN Clustering

* Density-based clustering for identifying alternative cluster structures and outliers

### 7. PCA Visualization

* Principal Component Analysis (PCA) used to reduce dimensions
* Cluster visualization in two-dimensional space

### 8. Cluster Profiling

* Average feature values analyzed for each cluster
* Comparison of economic and healthcare indicators across clusters

---

## Results & Insights

### Cluster 0 – Developed Countries

* Highest income levels
* Highest GDP per capita
* Lowest child mortality
* Highest life expectancy

### Cluster 1 – Underdeveloped Countries

* Highest child mortality
* Lowest income levels
* Lowest GDP per capita
* Lowest life expectancy
* Highest fertility rates

### Cluster 2 – Developing Countries

* Moderate income and GDP levels
* Moderate healthcare indicators
* Transitional stage between developed and underdeveloped economies

### Key Findings

* Cluster 1 countries should be prioritized for international aid and development programs.
* Income, GDP per capita, life expectancy, and child mortality are major drivers of country segmentation.
* K-Means successfully identified meaningful country groups based on socio-economic conditions.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

## Machine Learning Techniques

* K-Means Clustering
* DBSCAN
* Principal Component Analysis (PCA)
* StandardScaler
* Silhouette Score Evaluation

---

## How to Run

1. Clone the repository

```bash
git clone <repository-url>
```

2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. Open the notebook in Google Colab or Jupyter Notebook.

4. Upload the `Country-data.csv` dataset when prompted.

5. Run all notebook cells sequentially.

---

## Learning Outcomes

* Data Preprocessing
* Exploratory Data Analysis
* Feature Scaling
* Unsupervised Learning
* K-Means Clustering
* DBSCAN Clustering
* PCA Visualization
* Cluster Interpretation
* Data-Driven Decision Making

---

## Author

Developed as part of a Machine Learning Internship project on Country Segmentation and Customer Intelligence using Unsupervised Learning.
