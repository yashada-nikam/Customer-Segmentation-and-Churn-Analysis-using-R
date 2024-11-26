# Customer Segmentation Using K-Means Clustering

## Project Overview  
This project applies **K-means clustering** to perform customer segmentation, aiming to help businesses better strategize customer engagement and improve profitability. It uses a dataset from Kaggle representing customer attributes and spending behaviors, with the analysis conducted in **R**. The project identifies clusters of customers based on their characteristics and spending patterns.

## Methodology  

### 1. Data Collection and Preprocessing  
- Cleaned the data using **tidyverse**, removed null values, and created dummy variables with **fastDummies** for categorical features.  
- Scaled the data to ensure equal contribution of features using the formula:  
  `scaled_value = (original_value - mean) / standard_deviation`  

### 2. Exploratory Data Analysis (EDA)  
- Visualized customer spending behaviors and demographic trends using **ggplot2**.  
- Observed that:  
  - Unmarried customers generally have lower spending scores.  
  - Younger professionals (healthcare, marketing) spend more compared to older professionals in law.

### 3. Clustering Algorithm  
- Implemented **K-means clustering** with the number of clusters (**K**) determined using the **elbow method**.  
- Optimal number of clusters identified as **6**, based on the sum of squared distances (SSD).  
- Visualized the clusters using **clusplot()** from the cluster library.

### 4. Results  
- Successfully segmented customers into 6 distinct clusters based on spending behaviors and demographic attributes.  
- Generated a 2-D cluster plot showing major components that explain the clusters.  
- Cluster assignments saved for further analysis.

## Key Features  
- **Clustering Technique**: K-means  
- **Data Cleaning**: tidyverse, fastDummies  
- **Visualization**: ggplot2, clusplot  
- **Optimization**: Elbow method  

## Visuals  
### 1. Elbow Method Plot  
Shows the optimal number of clusters (K=6).  
### 2. Cluster Plot  
Visualizes the distinct customer clusters in 2-D space.  

## Tools & Libraries  
- **R**: Primary language used for the analysis.  
- **Packages**:  
  - `tidyverse`: Data manipulation  
  - `fastDummies`: Dummy variable creation  
  - `factoextra`: Visualization of clustering results  
  - `cluster`: Cluster visualization  
