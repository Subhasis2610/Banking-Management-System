# Banking Management System

## Overview

The Banking Management System is a Java-based application designed to manage and interact with customer records, accounts, and loans in a banking environment. It provides a command-line interface for performing various banking operations such as adding, updating, and deleting customer records, viewing account and loan details, and managing transactions.

## Features

- **Customer Records Management**
  - Show all customer records.
  - Add new customer records.
  - Delete existing customer records.
  - Update customer information (Name, Phone No, City).

- **Account Management**
  - Show account details for a specific customer.
  - Deposit money into an account.
  - Withdraw money from an account.

- **Loan Management**
  - Show loan details for a specific customer.

## Requirements

- **Java Development Kit (JDK) 8 or later**
- **Oracle Database** (or compatible database system)
- **JDBC Driver** for Oracle Database

## Setup

### Prerequisites

1. **Java JDK**: Ensure you have Java JDK 8 or later installed. You can download it from the [Oracle website](https://www.oracle.com/java/technologies/javase-downloads.html).

2. **Oracle Database**: Install and set up an Oracle Database. Create the necessary tables (`Customers`, `Accounts`, `Loans`) with appropriate fields.

3. **JDBC Driver**: Make sure you have the Oracle JDBC driver (`ojdbc8.jar`) available. You may need to add this to your project's classpath.

### Configuration

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/Subhasis2610/BankingManagementSystem.git
    ```

2. **Database Connection**:

    Update the `DatabaseConnection.java` file with your Oracle database connection details:

    ```java
    private static final String JDBC_URL = "jdbc:oracle:thin:@localhost:1521/XEPDB1"; // Update as per your configuration
    private static final String DB_USER = "SYSTEM";
    private static final String DB_PASS = "silu";
    ```

3. **Compile the Code**:

    Navigate to the project directory and compile the Java files:

    ```bash
    cd BankingManagementSystem/src
    javac *.java
    ```

4. **Run the Application**:

    Run the `BankingManagementSystem` class:

    ```bash
    java BankingManagementSystem
    ```

## Usage

Once the application is running, you will be presented with a menu to choose various operations:

1. **Show Customer Records**: Displays a list of all customer records in the database.

2. **Add Customer Record**: Allows you to add a new customer to the database.

3. **Delete Customer Record**: Allows you to delete an existing customer from the database.

4. **Update Customer Information**: Lets you update information for an existing customer.

5. **Show Account Details**: Displays account details for a specified customer.

6. **Show Loan Details**: Shows loan details for a specified customer.

7. **Deposit Money**: Allows you to deposit money into a specified account.

8. **Withdraw Money**: Allows you to withdraw money from a specified account.

9. **Exit**: Exits the application.

## Code Structure

- `DatabaseConnection.java`: Contains the JDBC connection logic to the Oracle database.
- `BankingManagementSystem.java`: Main application class that handles user interactions and performs various banking operations.

## Contributing

Feel free to fork the repository and make changes. If you would like to contribute back to the main project, please follow these steps:

1. Fork the repository on GitHub.
2. Create a new branch for your changes.
3. Commit your changes and push them to your fork.
4. Open a pull request with a description of your changes.


## Contact

For any questions or feedback, please reach out to:

- **Email**: subhasispatra978@gmail.com
- **GitHub**: [Subhasis2610](https://github.com/Subhasis2610)

---

**Note**: This project is intended for educational purposes and may require adjustments to fit specific use cases or environments.
