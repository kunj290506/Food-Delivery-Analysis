## Food Delivery Analysis  
### Customer Segmentation for Personalized Marketing using Clustering and PCA  
**Author:** Kunj Kiran Chauhan  
**Student ID:** D24AIML082

---

## Introduction  
In today’s competitive food delivery market, companies face the challenge of catering to a diverse user base. Customers differ in age, spending habits, app usage time, and order behavior. Without understanding these differences, businesses risk missing out on key opportunities for personalization and retention.

This project uses unsupervised machine learning techniques to identify **distinct customer segments** that can help food delivery services improve marketing strategies, increase engagement, and boost customer satisfaction.

---

## Project Objective  
Segment customers based on behavior and demographic features using clustering algorithms and PCA, so that businesses can:
- Personalize marketing campaigns
- Optimize service offerings
- Increase user retention and satisfaction

---

## Dataset Overview  
The dataset contains information about food delivery app users, including:
- Age  
- Total Orders  
- Average Spend  
- App Usage Time  
- Favorite Cuisine (categorical)  
- Delivery Ratings  
- And other behavioral metrics

---

## Tools & Libraries Used  
- `Pandas`, `NumPy` – Data manipulation  
- `Matplotlib`, `Seaborn` – Visualizations  
- `Scikit-learn` – Clustering, PCA, preprocessing  
- `SciPy` – Hierarchical clustering

---

## Operations Performed

### 1. Problem Understanding & Goal Setting  
- Defined the problem of customer diversity in food delivery services.  
- Set the goal to segment customers using clustering and PCA for targeted marketing.

### 2. Data Loading & Initial Inspection  
- Loaded the dataset from CSV file using `pandas`.  
- Performed summary statistics with `.describe(include='all')`.

### 3. Data Analysis & Interpretation  
- Discovered spending behavior, engagement time, cuisine preferences, age group distributions, and rating biases.  
- Identified insights to guide clustering.

### 4. Missing Value Check  
- Used `.isnull().sum()` to ensure data quality and identify gaps.

### 5. Data Preprocessing  
- Dropped irrelevant columns like `UserID`, `FavoriteCuisine`.  
- Scaled numerical features using `StandardScaler`.

### 6. Data Visualization  
- Plotted:
  - Histograms
  - Boxplots
  - Pair plots
  - Correlation matrix

### 7. Dimensionality Reduction with PCA  
- Reduced dimensions using PCA for better cluster visualization.  
- Interpreted principal components to understand feature influence.  
- Created scatter plots of PCA-transformed data.

### 8. Clustering - Unsupervised Learning  
- **K-Means Clustering**:
  - Ran the algorithm on standardized data.  
  - Used Elbow Method & Silhouette Score to determine optimal clusters.
- **Hierarchical Clustering**:
  - Created dendrograms with Agglomerative clustering.  
  - Compared results with K-Means.

### 9. Cluster Evaluation & Profiling  
- Assigned cluster labels to PCA plots.  
- Calculated average statistics per cluster.  
- Created business-friendly profiles (e.g., "young frequent users", "older high spenders").

### 10. Business Implications & Limitations  
- Demonstrated how results could support marketing and recommendation systems.  
- Discussed limitations (e.g., sensitivity to scaling, assumption of spherical clusters).  
- Suggested future enhancements (e.g., DBSCAN, richer behavioral data).

---

## Insights  
- Strong segment of premium high-spending users  
- High app engagement from younger users  
- Opportunities for cuisine-based promotions  
- Potential rating inflation that may need alternate metrics

---

## How to Run  
1. Install required libraries:  
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn scipy
