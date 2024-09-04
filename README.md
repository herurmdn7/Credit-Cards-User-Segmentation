
# Credit Cards User Segmentation

## Table of Contents
1. [Project Overview](#project-overview)
2. [Project Structure](#project-structure)
3. [Installation and Setup](#installation-and-setup)
4. [Data](#data)
5. [Segmentation Approach](#segmentation-approach)
6. [Modeling](#modeling)
7. [Results](#results)
8. [Conclusion](#conclusion)
9. [Future Work](#future-work)
10. [References](#references)

---

### 1. Project Overview
This project focuses on segmenting credit card users based on their purchasing behavior using clustering algorithms. The primary goal is to provide meaningful segmentation that helps identify user groups with similar spending patterns, which can be used for targeted marketing and improving customer satisfaction.

---

### 2. Project Structure
```bash
├── P1G6_Set_1_Heru.csv               # Cleaned dataset for analysis
├── P1G6_Set_1_Heru.ipynb             # Notebook for analysis and modeling
├── P1G6_Set_1_Heru_Inference.ipynb   # Notebook for inference
├── model.pkl                         # Trained model file for segmentation
├── README.md                         # Project README file
```

---

### 3. Installation and Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/herurmdn7/Credit-Cards-User-Segmentation.git
   ```
2. Ensure Python (version >=3.7) is installed.

---

### 4. Data
- **Source**: Credit card transaction data sourced from **BigQuery**.
- **Data Cleaning**: The dataset was cleaned to remove missing values and outliers. Unnecessary columns were dropped to improve model performance.
- **Structure**: The dataset contains information about credit card usage behavior, including transaction amounts, frequency, and various spending categories.

---

### 5. Segmentation Approach
- **Clustering Algorithm**: K-Means clustering was used for user segmentation. Different clusters were tested to optimize the segmentation process.
- **Feature Engineering**: Various features such as total spending, frequency of transactions, and types of purchases were used to identify distinct segments of users.

---

### 6. Modeling
- **K-Means Clustering**: K-Means was chosen as the primary clustering algorithm due to its simplicity and effectiveness for customer segmentation.
- **Model Evaluation**: Elbow method was used to determine the optimal number of clusters.
- **Inference**: Once the model was trained, predictions were made to assign users to specific segments.

---

### 7. Results
The segmentation process successfully identified different customer segments based on their credit card usage. Key insights include:
- **High Spenders**: Users with high transaction amounts but lower frequency.
- **Frequent Shoppers**: Users with a high frequency of smaller transactions.
- **Balanced Users**: Users with moderate spending and transaction frequency.

---

### 8. Conclusion
This project provides an effective way to segment credit card users based on their behavior. These segments can be used for targeted marketing strategies and improving customer service by personalizing offers according to user profiles.

---

### 9. Future Work
- **Explore Other Clustering Methods**: Consider using other algorithms like DBSCAN or Hierarchical Clustering for better segmentation.
- **Feature Expansion**: Incorporate additional features such as geographic location or time of purchase to enhance the segmentation process.
- **Real-Time Segmentation**: Implement a real-time system for continuously updating user segments as new transaction data becomes available.

---

### 10. References
- Tools: Python, Pandas, Jupyter, Scikit-learn
- Data Source: **BigQuery**
