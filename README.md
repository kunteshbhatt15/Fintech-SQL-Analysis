# Fintech SQL Analysis

This project demonstrates SQL analysis on a sample fintech banking dataset. It covers customer profiles, accounts, loans, transactions, and support tickets, then uses SQL queries to explore customer segmentation, balances, loan behavior, support activity, and window-function based rankings.

## Project Files

- `Fintech SQL Analysis Cleaned.sql` - database setup, sample inserts, and analysis queries
- `ER_Diagram.md` - Mermaid ER diagram for the database schema
- `dataset/` - CSV exports of each sample table

## Database Schema

The project uses five related tables:

- `CUSTOMERS` - customer demographic and credit information
- `ACCOUNTS` - account type, balance, status, and open date
- `LOANS` - loan amount, interest rate, and approval status
- `TRANSACTIONS` - credit/debit transactions linked to accounts
- `SUPPORT_TICKETS` - customer support issues and resolution time

## Key SQL Concepts Used

- Table creation with primary keys and foreign keys
- `INSERT` statements for sample data
- String functions such as `CONCAT`, `UPPER`, `LEFT`, and `SUBSTRING_INDEX`
- Null handling with `COALESCE` and `NULLIF`
- Conditional logic with `CASE`
- Inner joins
- Aggregate functions such as `COUNT`, `MAX`, and `AVG`
- Subqueries
- Common table expressions
- Window functions such as `RANK`, `DENSE_RANK`, and running totals

## Example Analysis Questions

- Which customers have credit scores above 750?
- Which account types have above-average balances?
- Who are the top two customers by balance within each account type?
- Which customers have never taken a loan?
- Which customers have raised support tickets?
- Which loans have interest rates below the overall average?
- Which customers have balances above the average for their city?

## How to Run

1. Open MySQL Workbench or another MySQL-compatible SQL client.
2. Run `Fintech SQL Analysis Cleaned.sql`.
3. The script creates the `FINTECH_ANALYTICS` database, loads sample data, and includes analysis queries.

## ER Diagram

The ER diagram is available in `ER_Diagram.md`. GitHub can render the Mermaid diagram directly in Markdown.

## Dataset

The `dataset` folder contains CSV files matching the inserted SQL sample data:

- `customers.csv`
- `accounts.csv`
- `loans.csv`
- `transactions.csv`
- `support_tickets.csv`

## Tools

- SQL
- MySQL
- GitHub Markdown
- Mermaid ER diagrams
