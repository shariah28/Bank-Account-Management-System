# Bank-Account-Management-System
Object-oriented C++ banking system supporting customer account management, checking, and savings accounts, loans, and credit services.

# Bank Account Management System (BAMS) 
                    A console-based banking system developed using C++ & OOP

A C++ banking management system developed as a team project to simulate common banking operations through a console-based application. The system utilizes object-oriented programming principles to organize customer information and different financial services, including loans, credit card accounts, savings and checking accounts.  

# Features

The application provides functionality for managing multiple bank account types and customer operations, including:
* Customer and account management
* Checking & Savings account operations
* Credit card account management
* Loan management
* Balance and account information retrieval
* Menu-driven console interaction

# Technologies
* **Language:** C++
* **IDE:** Microsoft Visual Studio
* **Programming Concepts:** Object-Oriented Programming (OOP), classes, inheritance, encapsulation, constructors, and member functions
* **Interface:** Command-line / console application

# System Architecture
Banking functionality is separated into multiple C++ classes, with each class responsible for a particular type of account, service, or customer-related operation. 

| Class | Functionality |
|-------|---------------|
| Customer | Stores & manages customer-related information |
| Account | Provides the common structure and functionality used by banking accounts. |
| Checking | Handles functionality associated with customer checking accounts. |
| Savings | Handles functionality associated with customer savings accounts. | 
| Credit | Manages credit card account information and related operations. | 
| Loan | Handles customer loan information and loan-related operations | 
      
# Contributions
This project was completed collaboratively, as a team of 2. My primary development responsibilities focused on three areas of the banking system:
## Credit Card Accounts
Implemented functionality supporting the system's credit card account operations and associated account information such as:
* Applying for a credit card
* Credit card application decisions based on credit score provided by user input
    - Decisions were measured whether user input was above or below a set score:
        - **DENIED:** scores 550 or lower
        - **APPROVED FOR GOLD CREDIT CARD:** scores 675 or greater
        - **APPROVED FOR ELITE CREDIT CARD:** scores 750 or greater
* Adjust credit Limit
* Cancel card 
* Check balance

## Loans
Following a similar sequence as the credit card class, the **Loan** class supports the system's loan operations including: 
* Loan Application
    - Customer's enter credit and are approved based on whether their score is above a set amount
    - Two Loan Application Options: Business or Personal
* For **Business Loans** approvals were made based on the following criteria:
    - **DENIED:** if score is lower 650
        - Customers receive a rejection letter stating they were rejected due to poor credit
    - **APPROVED FOR $100,000:** if score is above 700
    - **APPROVED FOR $250,000:** if score is above 750
*  For **Personal Loans** approvals were made based on the following criteria:
    - **DENIED:** if score is lower 650
        - Customers receive a rejection letter stating they were rejected due to poor credit
    - **APPROVED FOR $35,000:** if score is above 700
    - **APPROVED FOR $60,000:** if score is above 750
## Account
Implemented core account functionality used to represent and manage banking account information.
* Defined account attributes including account number, balance, deposit count, withdrawal count, and associated customer information.
* Implemented default and paramteterized constructors to initialize account and customer data.
* Created setter and getter methods for retrieving and updating account numbers, balances, deposits, and withdrawals.
* Implemented deposit functionality to update account balances and track the number of deposits made
* Implemented withdrawal functionality for modifying balances and tracking withdrawal activity.
* Integrated the **Customer** class with each account to associate customer information with account data.
* Created account summary output displaying **customer details, account number, current balance, deposits, and withdrawals.**

## How to Run?
The project was originally developed using Microsoft Visual Studio on Windows using C++ on. 

To run it in its original environment:
1. Clone or download the repository.
2. Open the Visual Studio solution (sln) file
3. Build the project
4. Run the console application


