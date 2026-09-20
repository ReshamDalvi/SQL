## 🏦 Nexora Bank – Banking Management System

Scenario:

Nexora Bank is a fictional banking organization providing financial services to customers across different cities in Maharashtra. The bank operates through multiple branches, with each branch managed by a branch manager.

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

