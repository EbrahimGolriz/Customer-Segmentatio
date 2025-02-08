# Customer Personality Analysis & Segmentation

![Clustering Visualization](https://img.shields.io/badge/Analysis-Clustering-blueviolet) 
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)

Customer segmentation analysis using clustering algorithms to identify distinct customer groups for targeted marketing strategies.

## 📁 Dataset
**Source:** [Customer Personality Analysis Dataset](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis/data)  
**Context:** 2,240 customer records with 29 behavioral features  
**Attributes Include:**
- Demographics (Age, Education, Marital Status, Income)
- Purchasing Behavior (Wines, Fruits, Meat, Fish, Sweets)
- Campaign Responses (AcceptedCmp1-5)
- Engagement Metrics (Recency, Web Visits, Store Purchases)

## 🛠️ Key Steps(Full report in **Report.pdf**)
### 1. Data Preprocessing
- Handled missing values
- Feature engineering:
- Encoded categorical features:
- Removed outliers

### 2. Feature Standardization
- Scaled features using StandardScaler
- Ensured equal weight for income (high magnitude) vs binary features

### 3. Clustering & PCA
**Algorithms Tested:**
- K-Means
- BIRCH
- MiniBatchKMeans 
- Agglomerative Clustering
- Mean Shift
**Dimensionality Reduction:**
- PCA achieved 90% variance retention with 7 components
- Silhouette Score Comparison

### 4. Cluster Visualization
![Cluster Characteristics](reports/cluster_viz.png)

## 📊 Key Findings
**3 Distinct Customer Segments Identified:**
1. **Cluster 0 - Budget Families**  
   - Lowest income (price-sensitive)
   - Middle-aged with children
   - Prefers deals on Gold/Fish/Sweets

2. **Cluster 1 - Affluent Professionals**  
   - Highest income (top 15%)
   - Young, educated, no kids
   - Wine/Meat enthusiasts, catalog shoppers

3. **Cluster 2 - Conservative Seniors**  
   - Moderate income
   - Oldest demographic (many widowed)
   - Low campaign engagement
