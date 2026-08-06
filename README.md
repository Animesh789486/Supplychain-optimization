# Supply Chain Optimization & Analytics

<img width="1707" height="520" alt="image" src="https://github.com/user-attachments/assets/4de936cf-b78e-4ba7-b385-c676a7ee00ec" />
<img width="1714" height="529" alt="image" src="https://github.com/user-attachments/assets/c6f87dcb-ec95-4e3d-9da6-15a4e2c897db" />
<img width="1722" height="524" alt="image" src="https://github.com/user-attachments/assets/56929316-bf5d-4b53-b134-06762263b850" />
<img width="1727" height="534" alt="image" src="https://github.com/user-attachments/assets/a2a745af-81b2-4f9b-b05d-3e1fd513e013" />
<img width="1715" height="523" alt="image" src="https://github.com/user-attachments/assets/7883fc26-7fbc-47b4-b61a-92f70c489ccd" />
<img width="1713" height="512" alt="image" src="https://github.com/user-attachments/assets/4d1fc13d-0262-42d3-b552-2c899c947d36" />


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
  
  ## Dashboard
<img width="1372" height="780" alt="image" src="https://github.com/user-attachments/assets/b6966def-9d48-4b4f-bb4d-f92239684385" />
<img width="1312" height="774" alt="image" src="https://github.com/user-attachments/assets/e05a38be-4569-4eb6-826e-fe300bb98be7" />
<img width="1347" height="776" alt="image" src="https://github.com/user-attachments/assets/ea680a0d-2a2a-41a5-b967-8e3d9eb1aa46" />

