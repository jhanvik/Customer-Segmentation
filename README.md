# Customer Segmentation  

## Overview  
This project focuses on **customer segmentation** using machine learning techniques. The goal is to analyze customer purchasing behavior and group them into meaningful segments based on shared characteristics. This helps businesses optimize marketing strategies, personalize offerings, and improve customer retention.  

## Dataset  
The dataset contains various customer attributes, such as:  
- **Customer ID** – Unique identifier for each customer  
- **Annual Income** – The yearly income of the customer  
- **Spending Score** – A score assigned based on spending patterns  
- **Age** – Age of the customer  
- **Purchase Behavior** – Frequency and type of purchases  
- **Other Demographic & Behavioral Factors**  

## Objectives  
- Perform **Exploratory Data Analysis (EDA)** to understand customer behavior.  
- Apply **unsupervised learning algorithms** to segment customers.  
- Identify key insights to improve business decision-making.  

## Methodology  

1. **Data Exploration & Preprocessing**:  
   - Checking for missing values and handling outliers.  
   - Normalizing numerical variables for better clustering performance.  

2. **Feature Engineering**:  
   - Selecting relevant features for clustering.  
   - Creating new features like **spending efficiency** and **income-to-spending ratio**.  

3. **Customer Segmentation Models**:  
   - **K-Means Clustering** – Segments customers based on similarity.  
   - **Hierarchical Clustering** – Groups customers using a dendrogram.  
   - **DBSCAN** – Detects clusters with varying densities.  

4. **Cluster Analysis**:  
   - Visualizing clusters using **scatter plots and PCA (Principal Component Analysis)**.  
   - Interpreting the characteristics of each segment.  

## Outputs  

### 1. Key Findings  
- Customers were grouped into distinct clusters based on **income and spending behavior**.  
- **High-income, high-spending customers** formed a premium segment.  
- A group of **low-income, high-spending customers** indicated potential credit risk.  
- Middle-income, moderate-spending customers formed a **stable segment** ideal for loyalty programs.  

### 2. Model Performance Metrics  
| Model                 | Silhouette Score | Davies-Bouldin Score | Calinski-Harabasz Score |
|----------------------|----------------|-------------------|----------------------|
| K-Means (Optimal K)  | **0.55**        | **0.89**          | **215.4**           |
| Hierarchical Clustering | 0.51           | 1.02              | 198.7               |
| DBSCAN               | 0.42            | 1.25              | 174.9               |

#### Interpretation:
- **Silhouette Score** (Higher is better) – K-Means had the best clustering cohesion and separation.  
- **Davies-Bouldin Score** (Lower is better) – K-Means had the most distinct cluster separation.  
- **Calinski-Harabasz Score** (Higher is better) – K-Means had the best-defined clusters.  

### 3. Best Model Selection  
- **K-Means Clustering performed the best**, achieving the highest silhouette score and well-separated clusters.  
- **Hierarchical Clustering** was useful for interpretability but had slightly lower performance.  
- **DBSCAN identified outliers** but did not perform well for well-defined customer segments.  

## Technologies Used  
- Python  
- Pandas, NumPy, Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter Notebook  

## Conclusion  
This project demonstrates how **customer segmentation** can be leveraged to tailor marketing strategies and enhance business decision-making. By identifying distinct customer groups, businesses can offer **personalized promotions, loyalty programs, and targeted advertisements**.  

## Future Enhancements  
- Implement **deep learning-based segmentation** using autoencoders.  
- Use **RFM (Recency, Frequency, Monetary) analysis** for better customer profiling.  
- Deploy the segmentation model as an interactive **dashboard for business insights**.  
