📊 Telecom Customer Churn & Retention Performance Dashboard

Power BI | Data Analytics Project

📌 Project Overview

This project analyzes customer churn behavior and revenue impact in a telecom company using Power BI. The dashboard provides a complete visual overview of customer distribution, churn patterns, revenue loss, contract types, payment methods, and service usage.

The goal of this project is to help business teams understand why customers are leaving and how churn affects revenue, enabling data-driven decision making.

🎯 Key Objectives

Analyze customer churn patterns

Identify high-risk contract types

Measure revenue lost due to churn

Evaluate impact of internet service, payment method & tech support

Build an interactive executive-level dashboard

🛠 Tools & Technologies Used

Power BI

Microsoft Excel (Data Cleaning)

DAX (Data Analysis Expressions)

CSV Dataset

📂 Dataset Details

Source: Telecom Customer Dataset

Total Records: 7,000+ customers

Key Fields Used:

CustomerID

Churn

ContractType

InternetService

PaymentMethod

TechSupport

MonthlyCharges

TotalCharges

Tenure

📈 KPIs Displayed

Total Customers

Churned Customers

Active Customers

Churn Rate (%)

Total Revenue

Lost Revenue from Churn

📊 Visualizations Included

Customer Churn by Contract Type

Lost Revenue by Internet Service Type

Churn Rate (%) by Contract Type (Line Chart)

Customer Churn by Payment Method

Customer Churn by Tech Support

Donut Chart (Churned vs Active Customers)

Interactive Slicer for Contract Type

🧮 Important DAX Measures Used
Total Customers = DISTINCTCOUNT(telecom_churn_dataset[CustomerID])

Churned Customers = 
CALCULATE(
    [Total Customers],
    telecom_churn_dataset[Churn] = "Yes"
)

Active Customers = 
CALCULATE(
    [Total Customers],
    telecom_churn_dataset[Churn] = "No"
)

Churn Rate % = 
DIVIDE([Churned Customers],[Total Customers],0)

Total Revenue = SUM(telecom_churn_dataset[TotalCharges])

Lost Revenue = 
CALCULATE(
    [Total Revenue],
    telecom_churn_dataset[Churn] = "Yes"
)

🖼 Dashboard Preview

(Upload your dashboard image here in GitHub using the image file you downloaded)

Example:

![Dashboard Preview](dashboard.png)

✅ Key Business Insights

Month-to-Month contracts show the highest churn

Fiber optic users generate the highest revenue loss

Customers without tech support have higher churn

Electronic check users churn more than bank transfer users

Almost 27% of customers have churned, causing significant revenue loss

📌 How to Use This Project

Download the .pbix Power BI file

Open in Power BI Desktop

Refresh the dataset

Explore KPIs using slicers and charts

💼 Resume-Ready Description (1-Line)

"Built an interactive Telecom Customer Churn & Revenue Analysis Dashboard in Power BI using DAX and real-world telecom data to identify churn drivers and revenue loss."

👤 Author

Rahul
Aspiring Data Analyst
Skills: Power BI | SQL | Excel | Python | Data Visualization

⭐ Project Value

This project demonstrates:

Business analytics thinking

Data cleaning & modeling

DAX mastery

Professional dashboard design

Storytelling with data

🏆 Final Note for Recruiters

This dashboard showcases real-world business insights, interactive filtering, revenue impact analysis, and executive-level design suitable for enterprise decision-making.
