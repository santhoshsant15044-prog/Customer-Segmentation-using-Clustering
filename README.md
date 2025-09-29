# Customer Segmentation using K-Means Clustering

 Introduction
This project focuses on customer segmentation, a critical practice in modern marketing. By understanding different customer groups, businesses can tailor their strategies to meet specific needs, leading to increased customer satisfaction and profitability.

This repository contains a complete data science pipeline that uses **unsupervised learning** to group customers of a mall based on their annual income and spending scores. The project covers data preprocessing, finding the optimal number of clusters using the Elbow Method, training a K-Means model, and interpreting the final customer segments for actionable business insights.

 🎯 Problem Statement
The primary goal is to identify distinct customer segments within a mall's clientele. By grouping customers with similar behaviors, the marketing team can develop targeted campaigns and promotions that are more effective and resource-efficient than a one-size-fits-all approach.


📊 Dataset
The project utilizes the "Mall Customers" dataset, which is publicly available on Kaggle. It contains basic information about the mall's customers.

* **Dataset Link:** [Mall Customer Segmentation Data - Kaggle](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
* **Key Features Used:**
    * `Annual Income (k$)`
    * `Spending Score (1-100)`


  Project Workflow
1.  **Data Preparation:** Selected the `Annual Income` and `Spending Score` features for clustering. As K-Means is a distance-based algorithm, the data was scaled using **StandardScaler** from Scikit-learn to ensure that both features were given equal importance.
2.  **Finding Optimal Clusters:** The **Elbow Method** was implemented to determine the optimal number of clusters (k). By plotting the Within-Cluster Sum of Squares (WCSS) for a range of k values, the "elbow" was identified at **k=5**, indicating that five distinct clusters are present in the data.
3.  **Model Training:** A **K-Means** model was trained on the scaled data with `n_clusters=5`. The model then assigned each customer to one of the five identified segments.
4.  **Cluster Visualization:** The final customer segments were visualized using a **Matplotlib** scatter plot to clearly show the distinct groups and their characteristics.


 💡 Results & Business Insights
The model successfully segmented customers into five distinct groups. These groups can be interpreted as customer personas for targeted marketing:



* **Cluster 1: Target Group (High Income, High Spending)**
    * **Insight:** Ideal customers. They should be targeted with premium product promotions and loyalty programs.
* **Cluster 2: Careful Spenders (High Income, Low Spending)**
    * **Insight:** Cautious buyers. Marketing should focus on quality, value, and high-end discounts to encourage purchases.
* **Cluster 3: Standard (Average Income, Average Spending)**
    * **Insight:** The general customer base. Standard marketing campaigns can be directed at this large segment.
* **Cluster 4: Careless Spenders (Low Income, High Spending)**
    * **Insight:** Likely younger, impulsive buyers. Target with trendy, budget-friendly items and promotions.
* **Cluster 5: Sensible (Low Income, Low Spending)**
    * **Insight:** Price-sensitive customers. Focus on essential products and special offers.

---
 💻 Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Scikit-learn, Matplotlib
* **Environment:** Jupyter Notebook

---
 🚀 How to Use
To run this project on your local machine, follow these steps:
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/santhoshsant15044-prog/Customer-Segmentation-using-Clustering.git](https://github.com/santhoshsant15044-prog/Customer-Segmentation-using-Clustering.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd Customer-Segmentation-using-Clustering
    ```
3.  **Install the required libraries:**
    ```bash
    pip install -r requirements.txt
    ```
    *(Note: You will need to create a `requirements.txt` file by running `pip freeze > requirements.txt` in your terminal)*
4.  **Run the Jupyter Notebook:**
    ```bash
    jupyter notebook "Customer Segmentation using Clustering.ipynb"
    ```
