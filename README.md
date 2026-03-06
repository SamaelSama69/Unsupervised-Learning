# AllLife Bank Customer Segmentation using Unsupervised Machine Learning

![Python](https://img.shields.io/badge/Python-3.9-blue) ![Machine
Learning](https://img.shields.io/badge/Machine%20Learning-Clustering-orange)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-green)
![Status](https://img.shields.io/badge/Project-Completed-success)

------------------------------------------------------------------------

# Project Overview

This project focuses on **customer segmentation for AllLife Bank** using
**unsupervised machine learning techniques**. The goal is to analyze
customer financial behavior and group similar customers together based
on their credit card usage patterns.

Customer segmentation enables banks to better understand their customer
base and design **targeted marketing strategies, improved services, and
personalized financial products**.

Using clustering algorithms such as **K-Means and Hierarchical
Clustering**, the project identifies distinct customer groups based on
attributes such as credit limits, credit card ownership, and banking
interaction channels.

------------------------------------------------------------------------

# Problem Statement

Banks serve customers with diverse financial behaviors and needs.
Treating all customers the same limits opportunities for targeted
services and marketing.

The objective of this project is to:

-   Segment customers into meaningful groups
-   Identify behavioral patterns among customers
-   Enable the bank to create targeted strategies for different customer
    segments

------------------------------------------------------------------------

# Dataset Description

The dataset contains financial and behavioral information about **660
bank customers**.

### Dataset Shape

660 rows × 7 columns

### Features

  Feature               Description
  --------------------- -------------------------------------------
  Sl_No                 Serial number
  Customer_Key          Unique customer identifier
  Avg_Credit_Limit      Average credit limit assigned to customer
  Total_Credit_Cards    Total number of credit cards owned
  Total_visits_bank     Number of visits made to the bank
  Total_visits_online   Number of online banking visits
  Total_calls_made      Number of customer service calls

All variables in the dataset are numerical and contain no missing
values.

------------------------------------------------------------------------

# Project Workflow

The project follows a structured data science workflow:

1.  Data Understanding
2.  Exploratory Data Analysis
3.  Data Preprocessing
4.  Feature Scaling
5.  Clustering Model Development
6.  Model Evaluation
7.  Cluster Profiling
8.  Business Recommendations

------------------------------------------------------------------------

# Data Preprocessing

Key preprocessing steps performed:

-   Checked for missing values and duplicates
-   Treated outliers using IQR capping
-   Scaled numerical features before clustering
-   Removed unnecessary identifiers

Feature scaling is essential because clustering algorithms rely on
distance calculations.

------------------------------------------------------------------------

# Machine Learning Techniques Used

Two unsupervised learning techniques were implemented and compared:

### K-Means Clustering

-   Used Elbow Method to determine optimal cluster count
-   Evaluated clusters using Silhouette Score

### Hierarchical Clustering

-   Tested multiple linkage methods
-   Selected optimal clusters using dendrogram analysis and cophenetic
    correlation

------------------------------------------------------------------------

# Optimal Number of Clusters

Using Elbow Method and Silhouette Score, the optimal number of clusters
was determined to be:

K = 3

------------------------------------------------------------------------

# Customer Segments Identified

## Platinum Customers

-   Very high credit limits
-   Large number of credit cards
-   Prefer online banking
-   Very few bank visits and calls

## Gold Customers

-   Medium credit limits
-   Moderate credit card ownership
-   Prefer in-person bank visits

## Silver Customers

-   Low credit limits
-   Few credit cards
-   High number of customer service calls

------------------------------------------------------------------------

# Model Comparison

  Method                                     Result
  ------------------------------------------ -----------------------------
  K-Means Clustering                         Clear and balanced clusters
  Hierarchical Clustering (Ward Linkage)     Similar segmentation
  Hierarchical Clustering (Single Linkage)   Less stable clusters

**Final Conclusion:** K-Means performed best for this dataset.

------------------------------------------------------------------------

# Key Insights

-   Higher credit limits correlate with owning more credit cards
-   High-value customers prefer online banking
-   Low-value customers rely more on customer service calls
-   Different customer groups require different engagement strategies

------------------------------------------------------------------------

# Technologies Used

Programming: - Python

Libraries: - Pandas - NumPy - Scikit-learn - Matplotlib - Seaborn -
SciPy

Environment: - Jupyter Notebook - Google Colab

------------------------------------------------------------------------

# Repository Structure

AllLife-Bank-Customer-Segmentation │ ├── data │ └── bank_customers.csv │
├── notebooks │ └── Customer_Segmentation.ipynb │ ├── reports │ └──
Project_Report.pdf │ └── README.md

------------------------------------------------------------------------

# How to Run the Project

Clone the repository:

git clone
https://github.com/yourusername/alllife-customer-segmentation.git

Install dependencies:

pip install -r requirements.txt

Run the notebook:

Customer_Segmentation.ipynb

------------------------------------------------------------------------

# Future Improvements

-   Deploy segmentation model using Streamlit or Dash
-   Build real-time segmentation pipeline
-   Test advanced clustering algorithms like DBSCAN and Gaussian Mixture
    Models
-   Create interactive dashboards for business users

------------------------------------------------------------------------

# Author

Sham Solanki\
Master's in Data Science -- Deakin University

------------------------------------------------------------------------

# License

MIT License
