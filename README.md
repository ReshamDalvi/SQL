## 🏦 Nexora Bank – Banking Management System

Scenario:

Nexora Bank is a banking organization providing financial services to customers across different cities in Maharashtra. The bank operates through multiple branches, with each branch managed by a branch manager.

The bank wants to develop a Banking Management System to store and analyze its banking operations in a structured SQL database.

The system maintains information about:
- Customers
- Branches
- Accounts
- Transactions
- Loans

### 1. Customers

The bank stores personal and registration information for every customer, including:
- Customer ID
- Customer Name
- Gender
- Age
- Phone
- Email
- City
- Customer Status
- Branch ID
- Registration Date

A customer is associated with a particular branch and can have one or more accounts and loans.

### 2. Branches

Nexora Bank operates through multiple branches across Maharashtra, including Mumbai, Dombivli, Thane, Navi Mumbai, Pune, Nashik, and Nagpur.

For each branch, the system stores:
- Branch ID
- Branch Name
- City
- State
- Branch Manager
- IFSC Code
- Contact Number
- Opening Date

A branch can have multiple customers, accounts, and loans.

### 3. Accounts

Customers can maintain different types of accounts:
- Savings
- Current
- Salary
- Fixed Deposit

For each account, the system stores:
- Account ID
- Customer ID
- Branch ID
- Account Type
- Balance
- Account Status
- Opening Date

A customer can have multiple accounts, allowing analysis of account ownership and customer banking behavior.

Account statuses include:
- Active
- Inactive
- Dormant
- Closed

### 4. Transactions

Customers perform banking transactions through their accounts.
The system records two main transaction types:
- Deposit
- Withdrawal

For every transaction, the bank stores:
- Transaction ID
- Account ID
- Transaction Date
- Transaction Type
- Amount
- Transaction Description

An account can have multiple transactions, allowing analysis of transaction activity and customer financial behavior.

### 5. Loans

Nexora Bank provides different types of loans to customers:
- Home Loan
- Personal Loan
- Vehicle Loan
- Education Loan

For each loan, the system stores:
- Loan ID
- Customer ID
- Branch ID
- Loan Type
- Loan Amount
- Interest Rate
- Loan Term
- Loan Status
- Loan Date

A customer can have one or more loans, and each loan is associated with a particular branch.

Loan statuses include:
- Active
- Closed
- Rejected




## 🏦 Nexora Bank – SQL Business Analysis Question Bank

- #### 👥 Customer Analysis
1. What is the total number of customers?
2. How many customers are Active vs Inactive?
3. How are customers distributed across cities?
4. Which cities have the highest number of Active customers?
5. How many customers registered each year?
6. Which customers are older than the overall average age?

- #### 💳 Account & Balance Analysis
1. How many accounts are there for each account type and status?
2. Which customers have multiple accounts?
3. What is the total account balance by customer?
4. Who are the top 10 customers by total account balance?
5. What is the total account balance by branch?
6. Which customers have both Savings and Fixed Deposit accounts?

- #### 💸 Transaction Analysis
1. What is the total number and total amount of transactions?
2. What are the total Deposit and Withdrawal amounts?
3. Which customers have the highest total transaction activity?
4. Which accounts have more Withdrawals than Deposits?
5. Which customers have both Deposit and Withdrawal transactions?
6. What is the monthly transaction amount trend?
7. Which transaction descriptions are used most frequently?

- #### 🏦 Loan Analysis
1. How many loans are there by loan type and status?
2. What is the total loan amount by loan type?
3. What is the total loan amount by branch?
4. Who are the top customers by total loan amount?
5. Which customers have multiple loans?
6. Which loan types have the highest average loan amount and interest rate?

- #### 👤 Customer Financial Relationship
1. Which customers have accounts but no loans?
2. Which customers have loans but no accounts?
3. Which customers have both accounts and loans?
4. Which customers have high account balances but no loans?
5. Which customers have loan amounts greater than their total account balance?

- #### 🏢 Branch Performance
1. Which branches have the highest number of customers, accounts, and loans?
2. Which branches have the highest total account balance?
3. Which branches have the highest total loan amount?
4. Compare account balances, loan amounts, and transaction activity across branches.

- #### 🧩 Customer Segmentation & Classification
1. Categorize customers into Young, Adult, Middle-Aged, and Senior based on age.
2. Categorize customers based on their total account balance as Low, Medium, or High.
3. Categorize customers based on their banking relationship: Account Only, Loan Only, Both, or No Product.

- #### 🔎 Customer & Banking Insights
1. Rank customers by their total account balance using RANK().
2. Find the top 3 customers by account balance in each city using a window function.
3. Find customers whose total account balance is above the overall average using a subquery.
4. Find pairs of customers living in the same city using a self join.
5. Create a consolidated customer banking view showing customer, account, and loan information.

- #### 📈 Financial Performance Analysis
1. Which loan types have the highest total number of active loans?
2. Which account types have the highest average balance?
3. Which branches have a higher total account balance than total loan amount?
4. Which branches have the highest transaction activity?
5. Which branches have both high account balances and high loan exposure?

- #### 📅 Banking Trends & Operations
1. How many new accounts were opened in each year?
2. How many loans were issued in each year?
3. What is the loan approval, rejection, and closure distribution?
4. What is the average time between customer registration and account opening?
5. What is the average time between customer registration and taking a loan?
6. On which days of the week are transactions most frequently performed?




## 📊 Key Performance Indicators
- Total Customers: 100
- Total Accounts: 150
- Total Loans: 75
- Total Transactions: 500
- Total Account Balance: ₹14.51M
- Total Loan Amount: ₹92.97M
- Total Transaction Amount: ₹5.95M
- Average Account Balance: ₹96,700
- Average Loan Amount: ₹1.24M
- Average Transaction Value: ₹11,896
- Average Accounts per Customer: 1.50
- Average Loans per Customer: 0.75



  
## 🎯 Project Conclusion

Nexora Bank SQL analysis provides a comprehensive view of the bank's customers, accounts, branches, transactions, and loans.

The analysis helps Nexora Bank understand customer demographics, monitor account balances, evaluate branch performance, track transaction behavior, and analyze the loan portfolio.

Customer and financial relationship analysis helps identify high-value customers, multiple-account holders, active banking relationships, and customers using multiple financial products.

CASE-based classification helps segment customers based on age, account balance, transaction activity, and banking relationships for better analysis.

Overall, this SQL project demonstrates how banking data can be organized, analyzed, and transformed into meaningful business insights to support data-driven decision-making.


# SQL


# 🏦 Nexora_Bank Project

```text
                 NEXORA BANK PROJECT
                         │
                         ▼
                  SQL DATABASE
                         │
          ┌──────────────┼──────────────┐
          │              │              │
          ├── Customers  ├── Accounts   ├── Branches
          ├── Loans      └── Transactions
          │
          ▼
                  DATA VALIDATION
                         │
          ├── Duplicate Checks
          ├── NULL Checks
          ├── Foreign Key Validation
          ├── Amount Validation
          └── Date Validation
                         │
                         ▼
                   SQL ANALYSIS
                         │
          ├── SELECT / WHERE
          ├── DISTINCT / ORDER BY
          ├── GROUP BY / HAVING
          ├── Aggregate Functions
          ├── JOIN
          ├── CASE
          ├── SUBQUERIES
          ├── WINDOW FUNCTIONS
          ├── SELF JOIN
          └── VIEWS
                         │
                         ▼
                  BUSINESS INSIGHTS
                         │
          ├── Customer Insights
          ├── Account & Balance Insights
          ├── Transaction Insights
          ├── Loan Insights
          ├── Branch Performance
          └── Financial Insights
