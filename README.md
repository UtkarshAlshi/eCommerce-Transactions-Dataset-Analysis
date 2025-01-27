# eCommerce Transactions Dataset Analysis

## Overview

This project aims to explore an eCommerce Transactions dataset and leverage data science techniques to derive meaningful business insights. The tasks involve performing **Exploratory Data Analysis (EDA)**, building a **Lookalike Model** to recommend similar customers, and conducting **Customer Segmentation** using clustering techniques. The ultimate goal is to assist businesses in improving their marketing strategies, customer acquisition, and retention.

The project includes:

- **Exploratory Data Analysis (EDA)** to understand the data and derive business insights.
- **Lookalike Model** to recommend similar customers based on transaction history and profile.
- **Customer Segmentation** using clustering techniques for targeted marketing.

---

## Table of Contents

- [Project Description](#project-description)
- [Tasks Overview](#tasks-overview)
  - [Task 1: Exploratory Data Analysis (EDA)](#task-1-exploratory-data-analysis-eda)
  - [Task 2: Lookalike Model](#task-2-lookalike-model)
  - [Task 3: Customer Segmentation / Clustering](#task-3-customer-segmentation--clustering)
- [Data Description](#data-description)
- [Methodologies Used](#methodologies-used)
  - [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Lookalike Model](#lookalike-model)
  - [Customer Segmentation](#customer-segmentation)
- [Installation Instructions](#installation-instructions)
- [File Naming and Submission](#file-naming-and-submission)
- [License](#license)

---

## Project Description

This project aims to uncover actionable insights from the eCommerce Transactions dataset consisting of three main files: `Customers.csv`, `Products.csv`, and `Transactions.csv`. These files contain customer profiles, product information, and transactional data, respectively.

By performing data analysis and applying machine learning techniques, the project develops a **Lookalike Model** to recommend similar customers and uses **clustering** to segment customers into meaningful groups. These techniques will help the company in better targeting marketing campaigns and improving business strategies.

---

## Tasks Overview

### Task 1: Exploratory Data Analysis (EDA)

The first task involves performing comprehensive exploratory data analysis (EDA) on the given dataset. Key operations include:
- Data cleaning and preprocessing.
- Exploring patterns and trends in customer behavior, products, and transactions.
- Generating key **business insights** that can help the company optimize their marketing strategies and customer engagement.

**Key Deliverables:**
- **EDA Code**: A Jupyter Notebook or Python script that performs the analysis.
- **Business Insights**: A PDF report containing actionable insights derived from the data.

### Task 2: Lookalike Model

The objective of Task 2 is to build a **Lookalike Model** that takes a customer's profile and transaction history as input, and recommends three similar customers. The model leverages both customer and product information to generate similarity scores, which are then used to identify customers with similar profiles.

**Key Deliverables:**
- **Lookalike.csv**: A file containing the top 3 lookalikes and their similarity scores for customers C0001 - C0020.
- **Model Code**: A Jupyter Notebook or Python script explaining the model development.

### Task 3: Customer Segmentation / Clustering

In this task, we perform customer segmentation using clustering techniques, utilizing both customer profile data and transactional data. The goal is to identify meaningful groups of customers that exhibit similar buying patterns.

**Key Deliverables:**
- **Clustering Results Report**: A detailed report including the number of clusters, DB Index value, and other relevant metrics.
- **Clustering Code**: A Jupyter Notebook or Python script containing the clustering logic and visualizations.

---

## Data Description

The dataset consists of the following files:

1. **Customers.csv**: Contains customer information.
   - `CustomerID`: Unique identifier for each customer.
   - `CustomerName`: Name of the customer.
   - `Region`: Continent where the customer resides.
   - `SignupDate`: Date when the customer signed up.

2. **Products.csv**: Contains product information.
   - `ProductID`: Unique identifier for each product.
   - `ProductName`: Name of the product.
   - `Category`: Product category.
   - `Price`: Product price in USD.

3. **Transactions.csv**: Contains transaction details.
   - `TransactionID`: Unique identifier for each transaction.
   - `CustomerID`: ID of the customer making the transaction.
   - `ProductID`: ID of the product sold.
   - `TransactionDate`: Date of the transaction.
   - `Quantity`: Quantity of the product purchased.
   - `TotalValue`: Total value of the transaction (Quantity * Price).

---

## Methodologies Used

### Exploratory Data Analysis

EDA was conducted to:
- Clean the data and handle any missing or inconsistent values.
- Visualize patterns like spending habits, frequency of transactions, product popularity, and regional trends.
- Identify outliers or anomalies in the dataset.

**Tools Used:**
- Pandas, Matplotlib, Seaborn for data processing and visualization.

### Lookalike Model

The Lookalike Model uses a **similarity scoring** mechanism to recommend customers with similar characteristics. The model takes into account:
- Customer demographic data (e.g., region, signup date).
- Transactional data (e.g., purchase frequency, total spending).

We used **cosine similarity** and **Euclidean distance** as metrics to compute customer similarity.

**Tools Used:**
- Pandas for data manipulation.
- Scikit-learn for building the similarity model.

### Customer Segmentation

For customer segmentation, we used **K-means clustering**, a widely used unsupervised learning algorithm, to group customers based on:
- Customer profile features (e.g., region, signup date).
- Transactional features (e.g., total value, frequency of purchase).

The quality of the clustering was evaluated using the **Davies-Bouldin Index (DBI)**, and the clusters were visualized using **2D scatter plots**.

**Tools Used:**
- Scikit-learn for clustering and DB Index calculation.
- Matplotlib/Seaborn for cluster visualization.

---

## Installation Instructions

To run the project, you need Python 3.x and several libraries. Follow these steps to set up the environment:

### Prerequisites
- Python 3.x
- pip (Python package installer)

### Installation Steps:
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ecommerce-transactions-analysis.git
   ```
   
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebooks for EDA, Lookalike Model, and Clustering:
   - `Utkarsh_Alshi_EDA.ipynb`
   - `Utkarsh_Alshi_Lookalike.ipynb`
   - `Utkarsh_Alshi_Clustering.ipynb`

---

## File Naming and Submission

Follow the naming convention for your files:
- **Utkarsh_Alshi_EDA.pdf**
- **Utkarsh_Alshi_EDA.ipynb**
- **Utkarsh_Alshi_Lookalike.csv**
- **Utkarsh_Alshi_Lookalike.ipynb**
- **Utkarsh_Alshi_Clustering.pdf**
- **Utkarsh_Alshi_Clustering.ipynb**

Upload all files to a public GitHub repository and share the link for submission.

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### Final Thoughts

This eCommerce Transactions Dataset analysis is designed to provide actionable insights that can be used to optimize marketing strategies, improve customer targeting, and enhance business operations. By leveraging advanced data science techniques such as exploratory data analysis, lookalike modeling, and customer segmentation, the project creates a comprehensive solution for real-world business challenges.
