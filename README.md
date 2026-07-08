# Supply Chain Optimization & Analytics

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow.svg)](https://pandas.pydata.org/)
[![Scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange.svg)](https://scikit-learn.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep%20Learning-orange.svg)](https://tensorflow.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Viz-green.svg)](https://plotly.com/)

An end-to-end **Supply Chain Analytics** project focused on risk assessment, inventory optimization, customer segmentation, lead time optimization, and predictive modeling using Machine Learning and Deep Learning.

---

## 📋 Project Overview

This project analyzes a comprehensive supply chain dataset to extract actionable business insights and build predictive models for better decision-making.

**Key Objectives:**
- Identify high-risk SKUs using custom risk scoring
- Optimize inventory using Economic Order Quantity (EOQ)
- Segment customers for targeted strategies
- Optimize transportation lead times
- Predict product demand and manufacturing costs

---

## 📊 Dataset

- **File**: `supply_chain_data.csv`
- **Rows**: 100
- **Columns**: 24
- **Domains**: Product, Sales, Inventory, Logistics, Manufacturing, Quality

**Key Features:**
- Product Type, SKU, Price, Availability
- Sales & Revenue
- Stock Levels, Lead Times
- Manufacturing Costs & Defect Rates
- Transportation Modes & Routes

---

## 🔍 Key Analyses & Insights

### 1. Risk Assessment
- Created a custom **Risk Score** = Lead Time + (1 - Stock Level)
- Identified top 30 highest-risk SKUs using interactive Plotly visualizations

### 2. Economic Order Quantity (EOQ)
- Implemented EOQ formula to recommend optimal order quantities
- Compared recommended vs actual order quantities

### 3. Customer Segmentation
- Segmented customers by **Demographics** and **Product Type**
- Analyzed average and total revenue per segment

### 4. Lead Time Optimization
- Compared average lead times across **Transportation Modes** (Road, Air, Rail, Sea)
- Identified best routes for faster delivery

### 5. Defect Rate Analysis
- Compared defect rates across **Product Types** (Haircare, Skincare, Cosmetics)

---

## 🤖 Machine Learning Models

### LightGBM (Demand Prediction)
- **Target**: `Number of products sold`
- **Features**: Price, Availability, Stock Levels, Lead Times, Order Quantities
- Used **10-Fold Cross Validation**
- Evaluated using MSE, RMSE, MAE, and R² Score

### Neural Network (Manufacturing Cost Prediction)
- **Target**: `Manufacturing costs`
- **Input**: `Production volumes`
- Built using **TensorFlow/Keras**
- Trained with Early Stopping and Model Checkpointing
- Used 5-Fold Cross Validation

---

## 🛠 Technologies Used

- **Python 3.12**
- **Pandas, NumPy** – Data Manipulation
- **Matplotlib, Seaborn, Plotly** – Visualization
- **Scikit-learn** – Preprocessing & Modeling
- **LightGBM** – Gradient Boosting
- **TensorFlow / Keras** – Deep Learning
- **Joblib** – Model Saving

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/supply-chain-optimization.git
   cd supply-chain-optimization
