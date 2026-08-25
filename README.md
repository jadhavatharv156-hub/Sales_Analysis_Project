# 📊 Sales Data Analysis

An end-to-end **Exploratory Data Analysis (EDA)** project analyzing customer purchase behavior across India. The project explores customer demographics, sector-wise revenue, zone and state performance, product categories, and customer spending patterns using **Python, Pandas, NumPy, Matplotlib, and Seaborn**.

---

## 📁 Dataset

The dataset contains:

- **11,239 cleaned records**
- **16 States**
- **15 Sectors**
- **18 Product Categories**

### Key Columns

| Column | Description |
|---|---|
| `User_ID` | Unique customer ID |
| `Cust_name` | Customer name |
| `Product_ID` | Product identifier |
| `Gender` | Customer gender |
| `Age Group` | Customer age group |
| `Age` | Customer age |
| `Marital_Status` | Customer marital status |
| `State` | Customer state |
| `Zone` | Geographic zone |
| `Sector` | Customer occupation/sector |
| `Product_Category` | Product category |
| `Orders` | Number of orders |
| `Amount` | Purchase amount |

---

## 🧹 Data Cleaning

The following data preprocessing steps were performed:

- Renamed `Occupation` to `Sector` for better clarity.
- Converted `Marital_Status` values from `0/1` into **Single/Married**.
- Removed completely empty columns such as `Status` and `Unnamed: 1`.
- Removed records with missing values in the `Amount` column.
- Checked and handled duplicate records.
- Standardized the dataset for further analysis.
- Exported the cleaned dataset as `cleaned_project_Data.xlsx`.

---

## 📈 Key Insights

### 👥 Age Group & Gender Analysis

The **26–35 age group** represents the largest customer segment, with **4,541 customers**, followed by the **36–45 age group** with 2,283 customers.

Female customers account for **7,832 customers**, compared with **3,407 male customers**, showing that female customers represent more than twice the male customer base.

Overall, customers between **18 and 45 years** contribute the majority of the orders.

### 📊 Sector Revenue Analysis

The **IT sector** generates the highest revenue at approximately **₹1.47 Cr**, followed by:

1. Healthcare — ₹1.30 Cr
2. Aviation — ₹1.26 Cr

The **Agriculture sector** generates the lowest revenue at approximately **₹25.9 Lakhs**.

The analysis also shows differences between total revenue and average order value, indicating that some sectors may generate higher-value purchases despite having fewer orders.

### 🌍 Zone Performance

The **Central Zone** is the strongest-performing zone, contributing approximately **39.2% of total revenue**.

Performance by zone:

- Central — **39.2%**
- Southern — **25.0%**
- Western — **17.3%**
- Eastern — **6.6%**

The Eastern Zone has significant potential for business expansion and targeted marketing.

### 🗺️ State Performance

**Uttar Pradesh** is the highest-revenue-generating state with approximately **₹1.94 Cr**, followed by **Maharashtra** with approximately **₹1.44 Cr**.

States such as **Telangana, Punjab, and Rajasthan** have comparatively lower revenue, indicating potential opportunities for targeted sales and marketing strategies.

### 💍 Marital Status

The customer distribution is approximately:

- **Single — 58%**
- **Married — 42%**

This indicates a moderate dominance of single customers within the dataset.

### 🛍️ Product Category Analysis

The leading product categories by order volume are:

1. **Clothing & Apparel** — 6,634 orders
2. **Food** — 6,110 orders
3. **Electronics & Gadgets** — 5,226 orders

These categories represent the strongest contributors to order volume.

On the other hand, **Hand & Power Tools** and **Tupperware** have relatively low order volumes and may require further analysis to understand their lower demand.

### 👤 Customer Spending Analysis

The analysis indicates that the **top 10% of customers contribute approximately 33.3% of total revenue**.

This customer concentration highlights the importance of:

- Customer retention
- Loyalty programs
- Personalized offers
- High-value customer targeting

### 💰 Average Order Value

The overall average order value is approximately **₹3,797**.

This value can be used as a benchmark to compare purchasing behavior across:

- Sectors
- Zones
- States
- Product categories
- Customer segments

---

## 📊 Visualizations

The project includes multiple visualizations covering:

- Age Group-wise Gender Count
- Sector-wise Total Revenue
- Sector-wise Average Orders
- Zone-wise Revenue
- Zone-wise Total Orders
- State-wise Revenue
- State-wise Total Orders
- Married vs Single Customers
- Product Category-wise Orders
- Top Customers by Spending

All visualization files are available in the `Visuals/` folder.

---

## 🛠️ Technologies & Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📂 Project Structure

```text
Sales-Data-Analysis/
│
├── Sales_Analysis.ipynb
├── cleaned_project_Data.xlsx
├── Total_States.csv
├── Total_Sectors.csv
├── Product_Category.csv
│
├── Visuals/
│   ├── Age Group Wise Gender Count.png
│   ├── Sector Wise Total Revenue.png
│   ├── Sector Wise Avg Orders.png
│   ├── Zone Wise Revenue.png
│   ├── Zone Wise Total Orders.png
│   ├── Total Revenue By Top 10 State.png
│   ├── Total Orders State.png
│   ├── Married And Single Users.png
│   ├── Top 10 Product Category Wise Total Orders.png
│   └── Spending Wise Top 10 Users.png
│
└── README.md
