# Grocery Sales EDA Project 🛒📊

This project is an **Exploratory Data Analysis (EDA)** on a grocery retail sales dataset.  
The goal was to clean the dataset, understand the data distributions, and analyze how different item and outlet features relate to **Item_Outlet_Sales**.

---

## 📌 Objective
- Perform complete EDA (cleaning + visualization + insights)
- Identify important patterns and trends in sales
- Understand which factors are most associated with sales

---

## 🗂️ Dataset Information
The dataset contains item and outlet details such as:
- Item Type, Item Weight, Item MRP
- Outlet Type, Outlet Size, Outlet Location Type
- Target column: **Item_Outlet_Sales** (Total revenue of an item in a particular outlet)

---

## ✅ Steps Performed

### 1️⃣ Data Cleaning
- Checked missing values
- Filled missing `Item_Weight` using **median-based imputation**
- Filled missing `Outlet_Size` using **mode per Outlet_Type**
- Verified column types and data quality

### 2️⃣ Univariate Analysis
- Analyzed distributions of key numeric features (Sales, MRP, Weight)
- Analyzed frequency distribution of categorical features (Outlet Type/Size/Location, Item Type)

### 3️⃣ Bivariate Analysis
Studied relationships between:
- **Item_MRP vs Item_Outlet_Sales**
- **Item_Weight vs Item_Outlet_Sales**
- **Outlet_Type / Outlet_Size / Outlet_Location_Type / Item_Type vs Sales**

### 4️⃣ Multivariate Analysis
- Combined Outlet_Type + Outlet_Size vs Sales
- Combined Location Tier + Outlet_Type vs Sales
- Correlation heatmap for numeric features

---

## 🔍 Key Insights
- `Item_Outlet_Sales` is **right-skewed**, meaning most items generate low-to-moderate sales while a few generate very high sales.
- `Item_MRP` shows a **multimodal pattern** (price bands) and has the strongest relationship with sales.
- `Item_Weight` shows **near-zero correlation** with sales, meaning weight alone does not explain sales.
- **Outlet_Type** plays a major role in sales distribution: Grocery stores show much lower median sales compared to supermarkets.
- Medium-sized outlets show higher median sales compared to small outlets.

---

## 🛠️ Tech Stack / Tools Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

---

## ▶️ How to Run
1. Clone the repository:
   ```bash
   git clone <repo-link>
