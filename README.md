# Data Warehouse Implementation on Daraz Dataset

## 📌 Project Overview

This project focuses on building a centralized **Data Warehouse** for the Daraz dataset.  
The objective is to collect, transform, store, and analyze data from multiple CSV sources to support better business intelligence and decision-making.

The project includes:
- ETL (Extract, Transform, Load) Pipeline
- Data Cleaning & Transformation
- Data Denormalization
- SQLite Database Storage
- Data Visualization using Python & Power BI

---


# 🏗️ Architecture Overview

![Architecture](./dwh_readme_assets/slide_1.png)

---

# ⚙️ Technologies Used

- **Python**
- **Pandas**
- **SQLite**
- **Matplotlib**
- **Power BI**

---

# 📂 Dataset Files

### Sales.csv
Contains:
- Sales transactions
- Sale amounts
- Sales regions
- Quantities sold

### Product.csv
Contains:
- Product titles
- Categories
- Product attributes

### Reviews.csv
Contains:
- Customer reviews
- Ratings
- Product identifiers

**![Extract](./dwh_readme_assets/slide_2.1.jpg)
![Extract](./dwh_readme_assets/slide_2.2.jpg)
![Extract](./dwh_readme_assets/slide_2.3.jpg)
**---

# 🔄 ETL Process

## 1️⃣ Extract

Data was extracted from CSV files using **Python Pandas**.

![Extract](./dwh_readme_assets/slide_3.png)

---

## 2️⃣ Transform

The transformation phase included:
- Handling missing values
- Removing duplicates
- Formatting date/time fields
- Creating new columns
- Data validation

![Transform](./dwh_readme_assets/slide_6.png)
![Transform](./dwh_readme_assets/slide_6.2.png)
![Transform](./dwh_readme_assets/slide_6.3.png)
![Removing Duplicates](./dwh_readme_assets/slide_6.4.png)
![Create new columns & date time format](./dwh_readme_assets/slide_6.5.png)
![Storing Cleaned Data in new files](./dwh_readme_assets/slide_6.6.png)



---

## 3️⃣ Denormalization

Sales and Product data were merged into:
- Product-Sales Table
- Product-Reviews Table

This improved query performance and reporting efficiency.

![Denormalization](./dwh_readme_assets/slide_11.png)

---

## 4️⃣ Load

The transformed data was loaded into:
- `project_database.db`

using **SQLite** for structured storage and fast querying.

![Load](./dwh_readme_assets/slide_16.png)

---

# 📊 Data Visualization

The project includes:
- KPI dashboards
- Sales performance analysis
- Category-wise sales breakdown
- Regional sales insights
- Trend analysis

### Power BI Dashboard Features
- Total Sales Metrics
- Units Sold by Category
- Region-wise Sales
- Product Demand Analysis
- Delivery Type Analysis

![Dashboard](./dwh_readme_assets/slide_21.jpg)

---

# 📈 Key Insights

- Improved accessibility to centralized business data
- Faster analytical queries
- Enhanced reporting capabilities
- Better trend identification
- Data-driven business decision support

---

# 🚀 Future Improvements

- Real-time data integration
- Cloud data warehouse deployment
- Automated ETL scheduling
- Advanced predictive analytics

---

# 🙌 Conclusion

This project successfully demonstrates the implementation of a **Data Warehouse** using Daraz sales data, integrating ETL processes, database storage, and visual analytics to support efficient business intelligence operations.

---

# ⭐ Thank You
