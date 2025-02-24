# Customer Segmentation  

## Overview  
This project aims to segment customers based on purchasing behavior using unsupervised learning techniques. By identifying distinct customer groups, businesses can tailor marketing strategies and improve customer engagement.  

## Dataset  
The dataset comprises customer data with the following attributes:  
- **CustomerID**: Unique identifier for each customer  
- **Gender**: Customer's gender  
- **Age**: Customer's age  
- **Annual Income (k$)**: Yearly income of the customer in thousand dollars  
- **Spending Score (1-100)**: Score assigned by the mall based on customer behavior and spending nature  

## Objectives  
- Perform Exploratory Data Analysis (EDA) to understand customer demographics and spending patterns.  
- Apply clustering algorithms to segment customers into distinct groups.  
- Visualize the clusters to interpret and profile each customer segment.  

## Methodology  

### 1. Data Exploration & Preprocessing  
- **Data Cleaning**: Checked for missing values and handled them appropriately.  
- **Feature Selection**: Focused on 'Age', 'Annual Income (k$)', and 'Spending Score (1-100)' for clustering.  
- **Data Visualization**: Used histograms and box plots to understand the distribution and detect outliers.  

### 2. Clustering Models  
- **K-Means Clustering**:  
  - Applied the **Elbow Method** to determine the optimal number of clusters.  
  - Segmented customers based on their purchasing behavior.  
  - Cluster visualization was performed using **scatter plots**.  
- **Hierarchical Clustering**:  
  - Used **dendrograms** to decide the number of clusters.  
  - Visualized customer groups using hierarchical clustering techniques.  

## Findings  
- **Optimal Number of Clusters**: The **Elbow Method** suggested 5 as the optimal number of clusters.  
- **Cluster Profiles**:  
  - **Cluster 1**: High income, high spending  
  - **Cluster 2**: High income, low spending  
  - **Cluster 3**: Low income, high spending  
  - **Cluster 4**: Low income, low spending  
  - **Cluster 5**: Average income, average spending  

## Performance Evaluation  
The clustering results were validated using **visual methods**, such as the **Elbow Method graph** and **cluster scatter plots**. However, quantitative metrics like **Silhouette Score and Davies-Bouldin Index** were **not computed** in this project.  

## Technologies Used  
- **Python**: Programming language  
- **Pandas & NumPy**: Data manipulation and analysis  
- **Matplotlib & Seaborn**: Data visualization  
- **Scikit-learn**: Machine learning algorithms  
- **Jupyter Notebook**: Interactive computing environment  

## Conclusion  
The project successfully segmented customers into distinct groups based on their purchasing behavior. These segments provide valuable insights that can drive targeted marketing and personalized customer experiences.  

## Future Enhancements  
- **Compute Clustering Metrics**: Include **Silhouette Score and Davies-Bouldin Index** for performance evaluation.  
- **Incorporate Additional Features**: Use more attributes like **purchase history** for deeper segmentation.  
- **Explore Other Clustering Algorithms**: Evaluate **DBSCAN** or **Gaussian Mixture Models** for better clustering.  
