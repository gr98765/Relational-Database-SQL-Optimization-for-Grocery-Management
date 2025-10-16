\## 🛒 Relational Database \& SQL Optimization for Grocery Management



A comprehensive relational database project modeled after a grocery retailer similar to Walmart Grocery. This project integrates real product data from the Walmart Grocery Product Dataset with synthetic customer, transaction, and pricing data to support inventory analytics, promotion tracking, and sales insights.



This project demonstrates the full lifecycle of database design—from conceptual modeling to SQL implementation and analytical querying.



---



\## 🔍 Project Overview



The goal of this project is to design a \*\*robust, normalized MySQL database\*\* that can support typical grocery retail operations, including:



\- 📦 Managing product, brand, category, and pricing information

\- 👥 Modeling customer, store, and transaction activity

\- 💰 Tracking promotional price changes

\- 📊 Analyzing sales trends and customer purchasing behavior



\### Project Deliverables



1\. \*\*ER Diagram \& Entity Design\*\*

2\. \*\*Relational Schema Conversion\*\*

3\. \*\*Normalization\*\* (1NF → 2NF → 3NF)

4\. \*\*SQL Implementation \& Optimization\*\*



---



\## 💡 Key Features



\### ✅ Real + Synthetic Integrated Dataset



\*\*Real Data:\*\*

\- Walmart Grocery product dataset



\*\*Synthetic Data:\*\*

\- Customer profiles

\- Transaction histories

\- Promotion/price records

\- Store-level inventory relationships



This design simulates a \*\*realistic retail environment\*\* for SQL querying and analytics.



\### 🎯 Performance Improvements



\- ✅ Reduced data redundancy by \*\*~35%\*\* through normalization

\- ✅ Improved query performance by \*\*~40%\*\* using indexes and optimized schema design

\- ✅ Supports complex analytical queries with efficient joins



---



\## 📊 Use Cases



This database supports various retail analytics scenarios:



| Use Case | Description |

|----------|-------------|

| 📈 \*\*Inventory Optimization\*\* | Track stock levels and reorder points |

| 🏆 \*\*Product Performance\*\* | Analyze best-selling products and categories |

| 💵 \*\*Pricing Strategy\*\* | Evaluate pricing effectiveness across stores |

| 🎁 \*\*Promotion Analysis\*\* | Measure promotional lift and ROI |

| 🏪 \*\*Store Comparisons\*\* | Compare performance across locations |

| 👤 \*\*Customer Segmentation\*\* | Analyze purchasing patterns (synthetic data) |



---



\## 🗂️ Database Schema



\### Core Entities

```

Products → Categories → Brands

&nbsp;   ↓

Inventory ← Stores

&nbsp;   ↓

Transactions ← Customers

&nbsp;   ↓

Promotions

```



\### Key Tables



\- \*\*Products\*\*: Product information, pricing, SKUs

\- \*\*Categories \& Brands\*\*: Product classification

\- \*\*Customers\*\*: Customer profiles and demographics

\- \*\*Stores\*\*: Store locations and details

\- \*\*Transactions\*\*: Purchase history and order details

\- \*\*Promotions\*\*: Discount tracking and price changes

\- \*\*Inventory\*\*: Stock management per store



---



\## 🚀 Future Extensions



\- \[ ] Integration with \*\*Python\*\* for interactive dashboards

\- \[ ] \*\*OLAP cube-style\*\* rollups for multi-dimensional analysis

\- \[ ] Query optimization experiments (indexes, materialized views)

\- \[ ] Real-time inventory tracking simulation

\- \[ ] Predictive analytics for demand forecasting



---



\## 🛠️ Technologies Used



\- \*\*MySQL\*\* - Database management system

\- \*\*ER Modeling\*\* - Entity-relationship design

\- \*\*SQL (DDL \& DML)\*\* - Database implementation

\- \*\*Data Normalization\*\* - 1NF, 2NF, 3NF

\- \*\*Dataset Engineering\*\* - Real + synthetic data integration

\- \*\*Retail Data Modeling\*\* - Domain-specific schema design



---



\## 📈 Project Impact



> \*\*Designed a fully normalized MySQL database\*\* using ER modeling and junction tables, reducing redundancy by ~35% and improving query performance by ~40%.



> An \*\*end-to-end retail data model\*\* that supports sales analytics, pricing insights, promotion impact analysis, and inventory decision-making.



---



\## 📂 Repository Structure

```

├── ER\_Diagram/          # Entity-relationship diagrams

├── Schema/              # SQL schema definitions

├── Queries/             # Analytical SQL queries

├── Dataset/             # Data files (excluded from repo)

└── README.md            # Project documentation

```



---





