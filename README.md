# ecommerce-olist-project

SQL Server data project built on the Olist Brazilian e-commerce dataset.
Goal: understand customer dissatisfaction and delivery problems, and
build a reporting layer for a Power BI dashboard.

## Business Questions
- What does "unhappy customer" mean in the data? (review_score <= 2)
- What does "late delivery" mean? (delivered date > estimated date)
- At which stage do delays happen: seller, carrier, or platform?

## Tech Stack
- Microsoft SQL Server + SSMS
- Azure Data Factory (planned)
- Power BI (planned)

## Dataset
Olist Brazilian E-Commerce dataset (Kaggle). Raw CSV files are NOT
stored in this repo. Download them from:
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## Repository Structure
```
sql/
  01_setup/        Database and table creation scripts
  02_validation/   Data quality checks
  03_reports/      Analysis and reporting queries
docs/              Requirement notes
```

## How to Run
1. Run `sql/01_setup/DB-102_create_database.sql`
2. Run `sql/01_setup/DB-102_create_orders.sql`
3. Load data (see docs)

## Naming Convention
Files start with the Jira ticket ID, e.g. `DB-102_create_orders.sql`.
Scripts are re-runnable (safe to run twice).

## Progress
- [x] Sprint 0: requirement discovery
- [ ] DB-102: create database and orders table
- [ ] DB-103: order status distribution query
- [ ] Data validation scripts

## Author
Sneha
