
# Basic Bank System

This repository contains a simple command-line banking application written in Java. It demonstrates foundational object-oriented programming concepts by simulating basic banking operations like account creation, deposits, and account information retrieval.

## Features

* **Account Creation:** Add new bank accounts by specifying a unique account number, customer name, and an initial balance.


* **In-Memory Storage:** Accounts are mapped and stored efficiently in memory using a Java `HashMap`.


* **Deposits:** Perform financial transactions by depositing a specified amount into an existing account, which dynamically updates the balance.


* **Account Inquiry:** Look up and display details for a specific account, outputting the account number, customer name, and current balance.


* **Error Handling:** Validates account existence, outputting an "Account not found!" message if a user attempts a transaction or inquiry on an unregistered account number.



## Repository Contents

* `Basic_Bank_System.java`: The core source code file containing all the necessary classes to execute the program.

## Architecture Overview

The system is contained within a single file and is divided into three primary classes:

* **`Account`:** The data model representing an individual customer. It safely encapsulates the `accountNumber`, `customerName`, and `balance` variables, and exposes a `deposit` method to modify the balance.


* **`Bank`:** The management class that holds the `Map<String, Account>`. It provides the core functionality methods: `addAccount`, `performTransaction`, and `displayAccountInfo`.


* **`BankingSystem`:** The main execution class. It currently runs a hardcoded simulation in the `main` method that populates the bank with two accounts ("John Doe" and "Jane Smith"), executes successful and failed transactions, and prints the resulting account states to the console.



## How to Run

1. Ensure you have the Java Development Kit (JDK) installed on your system.
2. Clone this repository or download the `Basic_Bank_System.java` file.
3. Open a terminal or command prompt and navigate to the folder containing the file.
4. Compile the Java file using the following command:
```bash
javac Basic_Bank_System.java

```


5. Execute the compiled program by running the main class:
```bash
java BankingSystem

```
