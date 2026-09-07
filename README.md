# 🏦 Banking Customer & Transaction Analytics — Power BI

An end-to-end **Power BI banking analytics project** designed to analyze customer behavior, transactions, banking products, branch performance, customer activity, and financial risk through interactive and business-focused dashboards.

The project demonstrates practical skills in **Power BI, Power Query, DAX, data modeling, data visualization, KPI development, interactive reporting, risk analysis, and What-If scenario analysis**.

---

## 📌 Project Overview

The banking industry generates large volumes of customer, transaction, account, loan, credit card, and activity data.

This project transforms raw banking data into an interactive analytical solution that enables users to explore business performance, customer behavior, financial products, branch performance, transaction trends, and potential risks.

The solution consists of **7 interactive Power BI dashboards**, each designed to answer specific business questions.

---

## 🎯 Business Objectives

The main objectives of this project are to:

- Monitor overall banking performance
- Analyze customer demographics and behavior
- Identify high-value customer segments
- Analyze transaction trends and channels
- Monitor account balances
- Analyze credit card utilization and outstanding amounts
- Analyze loan portfolios and financial exposure
- Compare branch-level performance
- Understand customer activity and engagement
- Identify anomalous and failed transactions
- Analyze financial risk
- Perform What-If scenario analysis
- Support data-driven business decision-making

---

# 📊 Dashboard Overview

The Power BI report contains **7 interactive dashboards**.

---

## 1️⃣ Executive Overview

Provides a high-level summary of the overall banking business.

### Key Metrics

- Total Customers
- Total Transactions
- Total Transaction Value
- Total Account Balance
- Transaction Success Rate
- Loan Exposure

### Key Analysis

- Monthly transaction value trends
- Transaction value by transaction type
- Customer distribution by segment
- Outstanding loan exposure
- Transaction status distribution
- Geographic transaction performance

### Business Questions

- How is the bank performing overall?
- What is the total transaction value?
- Which transaction types contribute the most value?
- Which customer segments are largest?
- How much loan exposure does the bank have?
- Where is transaction activity concentrated?

---

## 2️⃣ Customer Insights

Provides a detailed view of customer demographics, financial behavior, and engagement.

### Key Analysis

- Customer profile
- Customer segments
- Customer transaction value
- Account balances
- Loan exposure
- Credit card outstanding
- Transaction activity
- Customer demographics
- Financial products by customer segment

### Business Questions

- Who are the bank's customers?
- Which customer segments generate the highest transaction value?
- Which customers have higher financial exposure?
- How do customer segments differ in their product usage?
- How active are customers?

---

## 3️⃣ Customer Value

Focuses on customer segmentation, value, and financial contribution.

### Key Analysis

- Customers by segment
- Transaction value by segment
- Average customer income
- Average transaction value
- Top customers
- Customer ranking
- Income vs transaction value
- Customer value drivers
- Financial value by segment

### Advanced Analysis

The dashboard uses:

- Customer ranking
- Scatter analysis
- Decomposition Tree
- Conditional formatting
- Customer-level analysis

### Business Questions

- Which customer segments are most valuable?
- Which customers generate the highest transaction value?
- Is income related to transaction activity?
- Which segments contribute the most financial value?
- What are the major drivers of customer value?

---

## 4️⃣ Transactions

Provides detailed transaction intelligence and operational analysis.

### Key Analysis

- Transaction volume
- Transaction value
- Transaction types
- Transaction channels
- Transaction status
- Failed transactions
- Transaction trends
- Anomalous transactions
- Location-level transaction analysis
- Transaction details

### Business Questions

- Which transaction types are most common?
- Which channels generate the most transaction value?
- How are transactions trending over time?
- Where are failed transactions concentrated?
- Where are anomalous transactions occurring?
- What is the transaction success rate?

---

## 5️⃣ Products

Analyzes major banking products including accounts, credit cards, and loans.

### Account Analysis

- Total accounts
- Account balance
- Account types
- Account balance by type

### Credit Card Analysis

- Total credit cards
- Credit card outstanding
- Credit card limits
- Credit card utilization
- Credit card performance by type

### Loan Analysis

- Total loans
- Total loan amount
- Outstanding loan amount
- Loan types
- Loan status
- Average interest rate
- Average loan tenure
- Loan exposure

### Business Questions

- Which account types hold the highest balances?
- Which credit card types have the highest outstanding amounts?
- How much loan exposure does the bank have?
- Which loan types have higher outstanding balances?
- What is the average interest rate?
- Which products contribute most to financial exposure?

---

## 6️⃣ Branches

Analyzes branch performance, customer distribution, and customer activity.

### Key Analysis

- Customers by branch
- Accounts by branch
- Transaction value by branch
- Transaction volume by branch
- Account balance by branch
- Active vs inactive customers
- Customer activity rate
- Digital activity
- App usage
- Service calls
- Branch performance scorecard

### Business Questions

- Which branches perform best?
- Which branches generate the highest transaction value?
- Which branches have the most customers?
- Which branches have higher account balances?
- How active are customers across branches?
- Which branches receive more service calls?

---

## 7️⃣ Risk & What-If Simulator

Provides advanced risk analysis and scenario simulation.

### Risk Analysis

- Anomalous transactions
- Anomaly rate
- Failed transactions
- Financial exposure
- Outstanding loan exposure
- Risk categories
- Risk by customer segment
- Risk by transaction type
- Risk by channel
- High-risk transaction details

### Advanced Features

- Decomposition Tree
- Risk classification
- Conditional formatting
- Dynamic risk analysis
- What-If parameter
- Scenario analysis

### What-If Analysis

The dashboard includes a **Transaction Risk Increase** parameter that allows users to simulate changes in transaction value.

Users can select different scenarios such as:

- 0%
- 5%
- 10%
- 20%
- 30%
- 40%
- 50%

The dashboard dynamically calculates the projected transaction value based on the selected scenario.

### Business Questions

- Where are anomalous transactions concentrated?
- Which transaction types have higher risk?
- Which channels have more anomalies?
- Which customer segments show higher risk?
- What is the bank's financial exposure?
- How would transaction value change under different growth scenarios?

---

# 🗂️ Data Model

The project uses a structured relational data model consisting of dimension and fact tables.

## Dimension Tables

| Table | Description |
|---|---|
| `Dim_Date` | Date, month, year, quarter, and calendar attributes |
| `Dim_Customers` | Customer demographics and customer segmentation |
| `Dim_Branches` | Branch, city, state, and branch information |
| `Dim_Products` | Banking product information |
| `Dim_Accounts` | Customer account information and account balances |

## Fact Tables

| Table | Description |
|---|---|
| `Fact_Transactions` | Customer transaction records |
| `Fact_Loans` | Loan portfolio and loan exposure data |
| `Fact_Credit_Cards` | Credit card and credit utilization data |
| `Fact_Customer_Activity` | Customer login, service call, app usage, and interaction data |

---

# 🔗 Data Relationships

The model uses relationships between customers, dates, accounts, transactions, loans, credit cards, branches, and customer activity.

The main relationships include:

- Customers → Branches
- Transactions → Accounts
- Transactions → Customers
- Transactions → Date
- Loans → Customers
- Loans → Date
- Credit Cards → Customers
- Credit Cards → Date
- Customer Activity → Customers
- Customer Activity → Date

The model was designed to minimize ambiguous filtering paths and provide consistent interactive analysis across dashboards.

---

# 🧹 Data Preparation

Data preparation was performed using **Power Query**.

Key transformation activities included:

- Promoting headers
- Correcting data types
- Cleaning date fields
- Creating calendar attributes
- Creating Month-Year labels
- Validating numeric fields
- Validating Boolean fields
- Renaming tables for logical modeling
- Preparing tables for relationships
- Ensuring consistent ID data types

---

# 🧮 DAX Measures

The project uses DAX to create business metrics and analytical calculations.

---

📊 Power BI Features Demonstrated

This project demonstrates a wide range of Power BI capabilities:-

- Data Preparation
    Power Query
    Data cleaning
    Data transformation
    Data type management
    
- Data Modeling
    Dimension tables
    Fact tables
    Relationships
    Filter propagation
    Star-schema principles
    
- DAX
    Aggregations
    CALCULATE
    DIVIDE
    DISTINCTCOUNT
    AVERAGE
    RANKX
    SELECTEDVALUE
    Dynamic calculations
    
- Visualizations
    KPI Cards
    Bar Charts
    Column Charts
    Line Charts
    Donut Charts
    Scatter Plots
    Maps
    Treemaps
    Waterfall Charts
    Gauge Charts
    Tables
    Matrix
    Decomposition Tree
    
- Interactivity
    Slicers
    Cross-filtering
    Drill-down
    Conditional formatting
    Bookmarks
    Reset Filters
    Page Navigation
    Dynamic Titles
    
- Advanced Analytics
    Anomaly Analysis
    Risk Classification
    Customer Ranking
    Decomposition Tree
    What-If Parameters
    Scenario Analysis

---

💡 Key Business Insights

The dashboard is designed to help stakeholders identify:

- Overall banking transaction performance
- Customer segment contribution
- High-value customers
- Transaction channel performance
- Product-level financial exposure
- Loan portfolio trends
- Credit card utilization
- Branch performance differences
- Customer engagement patterns
- Areas with higher transaction risk
- Anomalous transaction concentration
- Potential financial exposure
- Impact of different transaction growth scenarios


📁 Project Structure

Banking-Customer-Transaction-Analytics-PowerBI/
│
├── Dataset/
│   ├── Dim_Date.csv
│   ├── Dim_Customers.csv
│   ├── Dim_Branches.csv
│   ├── Dim_Products.csv
│   ├── Dim_Accounts.csv
│   ├── Fact_Transactions.csv
│   ├── Fact_Loans.csv
│   ├── Fact_Credit_Cards.csv
│   └── Fact_Customer_Activity.csv
│
├── Screenshots/
│   ├── Executive.png
│   ├── Customer.png
│   ├── Value.png
│   ├── Transactions.png
│   ├── Products.png
│   ├── Branches.png
│   └── Risk.png
│
├── Banking Customer & Transaction Analytics.pbix
│
└── README.md


----

🖼️ Dashboard Screenshots

Executive Overview
  <img width="827" height="379" alt="image" src="https://github.com/user-attachments/assets/6ade374e-e7ba-44af-b3f4-8f306eeadaa1" />

Customer Insights
  <img width="827" height="379" alt="image" src="https://github.com/user-attachments/assets/ca125b57-a64a-4470-b4a7-2c7099965ff2" />

Customer Value
  <img width="830" height="383" alt="image" src="https://github.com/user-attachments/assets/c55d8fc3-a651-4706-ac37-d9e081cfbb60" />

Transactions
  <img width="828" height="379" alt="image" src="https://github.com/user-attachments/assets/d9f3c760-88ac-4e48-94d7-dd474705c201" />
 
Products
  <img width="830" height="380" alt="image" src="https://github.com/user-attachments/assets/4516f12b-9f2d-4ec0-a9f3-d187a47c8c06" />

Branches
    <img width="829" height="380" alt="image" src="https://github.com/user-attachments/assets/afa6e0ef-a861-4172-8f76-b2e4453154af" />

Risk & What-If Simulator
  <img width="833" height="379" alt="image" src="https://github.com/user-attachments/assets/6752d455-0754-4518-a62a-02cd14050451" />


----

🛠️ Tools & Technologies

| Technology      | Purpose                                       |
| --------------- | --------------------------------------------- |
| **Power BI**    | Dashboard development and visualization       |
| **Power Query** | Data cleaning and transformation              |
| **DAX**         | Business calculations and analytical measures |
| **CSV**         | Source data                                   |
| **GitHub**      | Project version control and portfolio hosting |



----


📌 Project Highlights

📊 7 Interactive Dashboards

      Seven business-focused dashboards provide different perspectives of banking operations.

👥 Customer Analytics

      Customer demographics, segmentation, transaction behavior, and financial value are analyzed.

💳 Product Analytics

      Accounts, credit cards, and loans are analyzed to understand financial exposure.

💰 Financial Analysis

      Transaction value, account balances, loan exposure, and credit card outstanding amounts are monitored.

🏦 Branch Analytics

      Branch-level customer, transaction, balance, and activity performance is compared.

⚠️ Risk Analytics

      Anomalous and failed transactions are analyzed to identify potential risk areas.

🔮 What-If Analysis

      Interactive scenario analysis demonstrates how changes in transaction activity could affect projected transaction value.


----

🎓 Skills Demonstrated-

  - Business Intelligence
  - Data Analytics
  - Power BI
  - Power Query
  - DAX
  - Data Modeling
  - Data Visualization
  - KPI Development
  - Customer Analytics
  - Financial Analytics
  - Transaction Analytics
  - Risk Analytics
  - Scenario Analysis
  - Dashboard Design
  - Business Reporting

---

🚀 Future Enhancements

Potential future improvements include:

  - Automated data refresh
  - Real-time transaction monitoring
  - Machine learning-based fraud prediction
  - Customer churn prediction
  - Advanced customer lifetime value modeling
  - Predictive loan default analysis
  - Power BI Service deployment
  - Row-Level Security
  - Automated alerts
  - Integration with SQL databases or APIs

----


👩‍💻 Author-

Akanksha Garg

Data Analytics | Power BI | SQL | Python | Cloud


----


⭐ Project

If you find this project useful or interesting, consider giving the repository a ⭐.
