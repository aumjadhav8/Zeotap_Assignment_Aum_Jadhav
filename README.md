# Zeotap Assignment

This project focuses on customer segmentation, lookalike modeling, and clustering analysis using eCommerce transaction data. The dataset consists of three primary CSV files: `Customers.csv`, `Products.csv`, and `Transactions.csv`. The tasks aim to derive business insights, predict similar customers based on their profiles and transaction history, and segment customers using clustering techniques.

## Table of Contents

1. [Task 1: Exploratory Data Analysis (EDA) and Business Insights](#task-1-exploratory-data-analysis-eda-and-business-insights)
2. [Task 2: Lookalike Model](#task-2-lookalike-model)
3. [Task 3: Customer Segmentation / Clustering](#task-3-customer-segmentation--clustering)
4. [Dependencies](#dependencies)

---

## Task 1: Exploratory Data Analysis (EDA) and Business Insights

In this task, we performed EDA to understand the data and uncover useful insights about customer and transaction patterns.

### Steps Involved:
1. **Data Cleaning and Preprocessing**:
   - Load and merge the `Customers.csv`, `Products.csv`, and `Transactions.csv` files.
   - Handle missing values, convert date columns to appropriate formats, and encode categorical variables.
   
2. **Exploratory Data Analysis**:
   - Visualized distributions of customer demographics (e.g., region).
   - Analyzed product sales across various categories and regions.
   - Studied transaction trends such as total spending, average transaction value, and frequency of purchases.
   
3. **Business Insights**:
   - Derived at least five actionable business insights based on the analysis of customer behavior, product preferences, and transaction trends.

### Deliverables:
- **Jupyter Notebook/Python Script** containing the EDA code.
- **PDF Report** summarizing the business insights.

### Outputs (Graphs)
![image](https://github.com/user-attachments/assets/a97929b4-0eea-4a9e-9250-67ad7292bb2b)
![image](https://github.com/user-attachments/assets/ea2da73d-73bb-40d8-ab0b-452539504c24)
![image](https://github.com/user-attachments/assets/05d2e48f-1f52-414f-a9fd-f0f9eca36a46)

**PDF Of Insights** 
![image](https://github.com/user-attachments/assets/62d0ed51-0ef6-4b53-a25e-019fa3e21055)

---

## Task 2: Lookalike Model

The objective of Task 2 was to build a Lookalike Model that recommends similar customers based on their profiles and transaction history.

### Steps Involved:
1. **Customer Profile Creation**:
   - Combine customer data and transaction data to create a profile for each customer, including features like region, days since signup, total purchases, and spending habits.
   
2. **Similarity Calculation**:
   - Implemented a similarity calculation mechanism using customer features (e.g., demographic info) and transaction-related features (e.g., total spending, frequent categories).
   
3. **Recommendation**:
   - For each customer (CustomerID: C0001 to C0020), recommend the top 3 similar customers based on their profile and transaction history.
   - Assign a similarity score to each recommendation.

4. **Output**:
   - A **Lookalike.csv** file containing a map of customer IDs to their top 3 lookalikes and their corresponding similarity scores.

### Deliverables:
- **Jupyter Notebook/Python Script** explaining the model development.
- **Lookalike.csv** containing the recommendations.

##Outputs:
**Lookalike.csv**
![image](https://github.com/user-attachments/assets/9d91e49a-b1df-404e-8d1a-6379e00f37c1)


**Top 3 Lookalikes with Similarity**
![image](https://github.com/user-attachments/assets/ae1ee45e-7d8a-4c03-a30e-80fdd3a143a4)

---

## Task 3: Customer Segmentation / Clustering

In this task, we used clustering techniques to segment customers into distinct groups based on both their profile and transaction information.

### Steps Involved:
To perform customer segmentation using clustering, we will:

1.Preprocess the data by aggregating transactions to form customer profiles.
2.Combine profile information with transaction data.
3.Apply a clustering algorithm.
4.Calculate metrics, including the Davies-Bouldin Index (DB Index).
5.Visualize clusters.

### Deliverables:
- **Jupyter Notebook/Python Script** containing the clustering code.
- **Clustering Report**:
  - Number of clusters formed.
  - DB Index value.
  - Other relevant clustering metrics and visualizations.

##Outputs:
![image](https://github.com/user-attachments/assets/ba5e345a-de8a-4f1b-903a-af89c6f31ec8)

![image](https://github.com/user-attachments/assets/1bc62d80-13c0-4721-b032-f1f648d42e94)
![image](https://github.com/user-attachments/assets/f4d5d0d2-0291-49b1-9cbf-b0c280cac2f4)

##Customer Segmentation (csv file)
![image](https://github.com/user-attachments/assets/057174f9-40f8-4b7e-9c2c-10e24adc9bc0)

---
## Warning : Inorder to run the ipynb files (notebooks) please copy the dataset csv in the same directory as the notebook files.

## Dependencies

The following libraries are required to run the project:

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- scipy
- sklearn

### Installation
```bash
pip install pandas numpy scikit-learn matplotlib seaborn scipy
