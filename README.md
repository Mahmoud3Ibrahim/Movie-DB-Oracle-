# Oracle to Access Integration – Assignment 02 (CST2355)

This project demonstrates how to set up a relational database in Oracle and connect it to a Microsoft Access frontend using ODBC. It was completed as part of Assignment 02 for CST2355 at Algonquin College.

## 🛠 Project Overview

- Create a new user in Oracle Database.
- Execute a provided SQL script (`Assignment2.sql`) to build tables and populate data.
- Set up an ODBC connection to connect Oracle with Microsoft Access.
- Open the provided Access file and verify data and form functionality.

## ⚙️ Setup Instructions

### Step 1: Create a New Oracle User

1. Open **Command Prompt** and run:
   ```
   sqlplus / as sysdba
   ```

2. Create a new user:
   ```sql
   CREATE USER A IDENTIFIED BY 123;
   GRANT ALL PRIVILEGES TO A;
   ALTER USER A ACCOUNT UNLOCK;
   ```

### Step 2: Connect via SQL Developer

1. Open **SQL Developer**.
2. Create a new connection with:
   - **Username**: A
   - **Password**: 123
   - Other fields: Match your lab settings (Hostname, Port, Service Name)
3. Test and connect.
4. Run the `Assignment2.sql` script to set up the schema and data.

### Step 3: Link Oracle with MS Access

1. Open **ODBC Data Source Administrator**.
2. Create a new DSN with the same credentials:
   - Name: ASSIGNMENT02
   - Username: A
   - Password: 123
3. Open the provided **Assignment 02 Access file**.
4. When prompted, enter:
   - Username: A
   - Password: 123
   - Service Name: your Oracle service name (usually `orcl`)

## ✅ Verification

- Tables should appear in MS Access.
- Forms should open and display data correctly.
- If everything loads and works properly, the integration is successful.

## 🧠 Skills Demonstrated

- Oracle SQL user and privilege management
- SQL script execution and schema creation
- ODBC configuration and database connectivity
- MS Access frontend integration with Oracle backend

---

📌 **Course**: CST2355 – Database Systems  
👨‍💻 **Author**: Mahmoud Ibrahim  
📅 **Term**: Winter 2025
