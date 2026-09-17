# FinTrack – Bank Management System

FinTrack is a console-based Bank Management System developed in **C++**. It simulates core banking operations while demonstrating Object-Oriented Programming, Data Structures and Algorithms, file handling, and modular software design.

## Features

### Admin Module

* Create new customer accounts
* Delete existing accounts
* View all registered accounts
* Search accounts using account number
* View basic bank analytics such as total accounts and total balance
* Create Savings and Current accounts

### Staff Module

* Deposit money into an account
* Withdraw money from an account
* Transfer funds between accounts
* Validate transaction amounts
* Maintain minimum balance according to account type

### Customer Module

* Login using account number and password
* View account details
* View transaction history

## Data Structures Used

### Binary Search Tree (BST)

A custom Binary Search Tree is used to store, search, insert, and delete customer accounts using the account number.

### Hash Table

A custom Hash Table is used for customer credential lookup and authentication.

Hash collisions are handled using **separate chaining with linked nodes**.

## File Handling

The application uses file handling to preserve account and credential information between program executions.

Individual transaction history is also recorded in separate transaction files with timestamps.

## Technologies and Concepts

* C++17
* Object-Oriented Programming
* Data Structures and Algorithms
* Binary Search Tree
* Hash Table
* Linked Lists
* File Handling
* Modular Programming

## Project Structure

```text
FinTrack-Bank-Management-System/
│
├── include/
│   ├── bst/
│   ├── hashtable/
│   ├── modules/
│   └── utils/
│
├── src/
│   ├── bst/
│   ├── hashtable/
│   ├── modules/
│   ├── utils/
│   └── main.cpp
│
├── data/
│   ├── accounts.txt
│   ├── credentials.txt
│   └── transactions/
│
├── Makefile
├── README.md
└── .gitignore
```

## Build and Run

### Using Make

Build the project:

```bash
make build
```

Run the program:

```bash
make run
```

### Compile Manually

```bash
g++ -std=c++17 src/main.cpp src/bst/*.cpp src/hashtable/*.cpp src/modules/*.cpp src/utils/*.cpp -Iinclude -o fintrack
```

Then run:

```bash
./fintrack
```

## Banking Rules

The application maintains a minimum balance during withdrawals and fund transfers:

* Savings Account: 1000
* Current Account: 5000

Transactions with invalid or non-positive amounts are rejected.

## What I Learned

Through this project, I gained practical experience in:

* Designing a modular C++ application
* Implementing a Binary Search Tree from scratch
* Implementing a Hash Table with separate chaining
* Working with pointers and dynamically allocated nodes
* Applying OOP concepts to a real-world project
* Managing persistent data using file handling
* Implementing basic authentication logic
* Handling deposits, withdrawals, and fund transfers
* Debugging a multi-file C++ project

## Future Improvements

* Add authentication for Admin and Staff modules
* Integrate MySQL or PostgreSQL instead of text-file storage
* Improve password security using a production-grade password hashing algorithm
* Add advanced reporting and account statements
* Add unit tests
* Add a graphical or web-based interface

## Author

**Harsh Dhuriya**

Computer Science Engineering Student
C++ | DSA | Software Development

