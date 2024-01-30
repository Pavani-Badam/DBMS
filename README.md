# DBMS
**Transaction Management System (DBMS Project)**

**Overview**

This project is a Database Management System (DBMS) implementation for a Transaction Management System. It includes a well-defined schema and an Entity-Relationship (ER) diagram, providing a foundation for efficient transaction processing.

**Schema**

1. Customer Table
   
Fields:

    firstName: First name of the customer.
    lastName: Last name of the customer.
    customerId (Unique Attribute): Unique identifier for each  customer.
    Address (Composite Attribute): Consists of city, zipcode, and state.

2. Transaction Table
   
Fields:

    transactionId (Unique Attribute): Unique identifier for each transaction.
    customerId: Identifier linking to the Customer Table for the associated customer.
    transaction_type: Type of transaction (e.g., deposit, withdrawal).
    trans_amount: Amount involved in the transaction.
    transactionDate: Date and time of the transaction.
    accountId: Identifier linking to the Account Table for the associated account.

3. Account Table
   
Fields:

    total_amount: Total amount in the account.
    accountId (Unique Attribute): Unique identifier for each account.
    acct_type: Type of account (e.g., savings, checking).
    customerId: Identifier linking to the Customer Table for the account holder.
    bank_Id: Identifier linking to the Bank Table for the associated bank.

4. Bank Table
   
Fields:

    bankName: Name of the bank.
    bankId (Unique Attribute): Unique identifier for each bank.
    Manager: Manager overseeing the bank operations.

**Relationships:**

    A Customer makes a Transaction.
    A Transaction updates an Account.
    An Account is in a Bank.

**Usage:**

Implement the schema and relationships in your preferred Database Management System. Utilize the provided attributes to establish meaningful connections between tables and ensure data consistency.

**Examples:**

When a customer initiates a transaction, create a new entry in the Transaction Table with the relevant details.
Update the Account Table with the transaction details, modifying the total_amount accordingly.
Ensure that the Account is associated with the correct Bank using the bank_Id attribute.

**Note:**

This project is designed as a foundation for a Transaction Management System. Customize the implementation based on specific business requirements and the chosen database platform.

Feel free to contribute, report issues, or suggest improvements to enhance the functionality and usability of this DBMS project.
