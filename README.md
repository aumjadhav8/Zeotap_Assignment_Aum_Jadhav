# Zeotap Assignment

This project focuses on customer segmentation, lookalike modeling, and clustering analysis using eCommerce transaction data. The dataset consists of three primary CSV files: `Customers.csv`, `Products.csv`, and `Transactions.csv`. The tasks aim to derive business insights, predict similar customers based on their profiles and transaction history, and segment customers using clustering techniques.

## Table of Contents

1. [Task 1: Exploratory Data Analysis (EDA) and Business Insights](#task-1-exploratory-data-analysis-eda-and-business-insights)
2. [Task 2: Lookalike Model](#task-2-lookalike-model)
3. [Task 3: Customer Segmentation / Clustering](#task-3-customer-segmentation--clustering)
4. [Dependencies](#dependencies)
5. [Usage](#usage)
6. [Evaluation Criteria](#evaluation-criteria)

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

---

## Task 3: Customer Segmentation / Clustering

In this task, we used clustering techniques to segment customers into distinct groups based on both their profile and transaction information.

### Steps Involved:
1. **Data Preparation**:
   - Combine the `Customers.csv` and `Transactions.csv` data to generate customer features, such as total purchases, total spending, and the frequency of purchasing each product category.

2. **Clustering Algorithm**:
   - Applied a clustering algorithm (e.g., K-means) to segment customers into clusters based on the features.
   - The number of clusters chosen was between 2 and 10 based on data characteristics and clustering metrics.

3. **Evaluation**:
   - Calculated the **DB Index** and other relevant clustering metrics to evaluate the effectiveness of the clustering.
   - Visualized the clusters to provide insights into customer behavior patterns.

### Deliverables:
- **Jupyter Notebook/Python Script** containing the clustering code.
- **Clustering Report**:
  - Number of clusters formed.
  - DB Index value.
  - Other relevant clustering metrics and visualizations.

---

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
