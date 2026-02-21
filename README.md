# 🛒 E-commerce Return Rate Reduction Analysis

**Internship:** Elevate Labs | **Domain:** Data Analytics & Machine Learning  

## 📝 Project Overview
[cite_start]Product returns are a significant profit-drainer in the e-commerce industry[cite: 71, 72]. [cite_start]The objective of this project is to analyze transactional retail data to identify why customers return products and how return rates vary across different categories and geographies[cite: 72]. Moving beyond historical analysis, this project utilizes a Machine Learning model to predict the probability of future returns, allowing the business to take proactive measures.

## 🛠️ Tools & Technologies
* [cite_start]**SQL (SQLite):** Data extraction, aggregation, and table joining[cite: 73].
* [cite_start]**Python:** Data preprocessing and predictive modeling[cite: 73].
    * *Libraries:* `pandas`, `numpy`, `scikit-learn`
* [cite_start]**Power BI:** Interactive dashboarding and data storytelling[cite: 73].

## 🔄 Project Workflow

### 1. Data Engineering (SQL)
* [cite_start]Imported and cleaned the raw `Orders` and `Returns` datasets[cite: 75].
* Executed a `LEFT JOIN` to combine the tables, creating a binary target variable (`Is_Returned`) to flag historical returns.
* [cite_start]Analyzed historical return percentages grouped by Product Category and Region[cite: 77].

### 2. Predictive Modeling (Python)
* **Preprocessing:** Handled missing values and applied `OneHotEncoder` to convert categorical text data (Category, Region) into numerical formats.
* [cite_start]**Model Training:** Built and trained a **Logistic Regression** classification model to predict the probability of a return[cite: 78].
* [cite_start]**Scoring:** Generated a "Return Risk Score" (0% to 100%) for every order in the dataset[cite: 79].

### 3. Data Visualization (Power BI)
* [cite_start]Built an interactive dashboard for supply chain managers to monitor return risks[cite: 79].
* [cite_start]Implemented **drill-through filters** allowing users to click on a high-risk category and view detailed product-level insights[cite: 81].
* Visualized geographic heat maps and bar charts to pinpoint problem areas.

## 📂 Repository Contents
* [cite_start]`Return_Prediction.ipynb` - The Python codebase containing the preprocessing and Logistic Regression model[cite: 81].
* `Orders_With_Returns.sql` - The SQL queries used to clean and merge the initial datasets.
* [cite_start]`High_Risk_Products.csv` - An exported list of the top 10 products most likely to be returned[cite: 82].
* `Ecom_Return_Dashboard.pdf` - A static export of the interactive Power BI dashboard.
* `Final_Project_Report.pdf` - A 2-page executive summary detailing the methodology and business recommendations.

## 💡 Key Business Insights
* **Category Risk:** Certain categories (e.g., Clothing) experience significantly higher return rates compared to standard office supplies.
* **Proactive Mitigation:** By utilizing the Return Risk Score, the company can flag high-risk transactions prior to shipping and verify order accuracy, potentially saving thousands in reverse-logistics costs.

---
*Developed by Kalai Magal during the Elevate Labs Internship.*
