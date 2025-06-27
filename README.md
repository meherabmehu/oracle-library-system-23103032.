# oracle-library-system-23103032.

📘 University Library Management System
Final Assignment – Database (MySQL/Oracle/SQL Server) Course

📋 Assignment Overview
This project serves as the final assignment for the Database course. It involves the complete implementation of a University Library Management System using Oracle Database, aligned with the assignment requirements.

🎯 Assignment Objectives
This assignment demonstrates my ability to:

📚 Design and implement a comprehensive database system for library operations

🧩 Apply normalization principles and relational database design concepts

💻 Develop complex SQL and PL/SQL solutions

🔐 Implement database security and optimize performance

🧠 Learning Outcomes Achieved
Database Design: Applied ER modeling and normalization up to 3NF

SQL Proficiency: Mastered DDL, DML, DCL, and TCL operations

PL/SQL Programming: Developed procedures, functions, and triggers

Database Administration: Managed users and performed basic tuning

✅ Assignment Components Completed
Part 1: Database Design & Setup (15 Marks)
✅ 1.1: Created tables (BOOKS, MEMBERS, TRANSACTIONS) with proper constraints

✅ 1.2: Inserted sample data (20 books, 15 members, 25 transactions)

Part 2: Basic SQL Operations (20 Marks)
✅ 2.1: Retrieval queries (e.g., available books, overdue members, top borrowed books)

✅ 2.2: Data manipulation (e.g., insert members, update fines, archive records)

Part 3: Advanced SQL Queries (25 Marks)
✅ 3.1: Join operations (INNER, LEFT, SELF, CROSS)

✅ 3.2: Subqueries (e.g., high fines, least borrowed books)

✅ 3.3: Aggregates and window functions (e.g., rankings, trends)

Part 4: PL/SQL Programming (25 Marks)
✅ 4.1: ISSUE_BOOK stored procedure

✅ 4.2: CALCULATE_FINE function

✅ 4.3: Trigger for updating available_copies on return

Part 5: Database Administration (15 Marks)
✅ 5.1: Created users with appropriate privileges (librarian, student_user)

✅ 5.2: Performance optimization using indexing and execution plans

🛠️ Technologies Used
Component	Technology
Database	Oracle Database
Query Language	SQL (DML, DDL, DCL, TCL)
Procedural Language	PL/SQL
Tools Used	Oracle SQL*Plus / GUI

⭐ Key Features
1. 📖 Books Management
Stores title, author, publisher, ISBN, category

Tracks total and available copies

Enables categorization and inventory control

2. 👤 Member Management
Supports different user types (students, faculty, staff)

Stores contact info, membership type, and status

3. 📝 Transaction Management
Tracks book issue and return operations

Manages due dates, fines, and return status

Supports real-time fine calculation

🔍 Query Capabilities
📌 Data Retrieval
Available books

Members with overdue books

Most borrowed books

Inactive/low-activity members

✍️ Data Manipulation
Register new members

Update fine records

Archive old transactions

🔗 Join Operations
INNER JOIN – active member transactions

LEFT JOIN – all books with or without borrow history

SELF JOIN – member referral system

CROSS JOIN – analytical reports

🧠 Subqueries
Identify high-fine members

List rarely borrowed books

Calculate average borrowings

Filter top borrowers

📊 Analytics
SUM, COUNT, AVG for statistical reports

RANK(), NTILE(), LAG() for trends and activity insights

🔄 PL/SQL Automation
1. ISSUE_BOOK Procedure
Validates book availability

Inserts new transaction

Automatically updates inventory

Includes error handling logic

2. CALCULATE_FINE Function
Accepts transaction_id

Calculates fine at ₹5/day post due date

Returns fine amount

3. Trigger: UPDATE_AVAILABLE_COPIES
Triggered on return

Automatically increments available_copies

Maintains data consistency

🔐 Database Administration
Role-Based Access Control
Role	Permissions
librarian	Full access to all operations
student_user	SELECT access on BOOKS only

Performance Optimization
Indexed columns: book_id, member_id, issue_date

Analyzed execution plans for optimization

Ensured query efficiency for frequent operations

📁 Project Structure
pgsql
Copy
Edit
oracle-library-system-[student-id]/
│
├── README.md                 → This documentation
│
└── sql/
    ├── setup.sql             → Schema creation + sample data
    ├── queries.sql           → All SQL queries (basic + advanced)
    ├── plsql.sql             → Stored procedures, functions, triggers
    └── admin.sql             → User management and performance optimization
📄 File Descriptions
setup.sql: DDL scripts, table creation with constraints, sample data

queries.sql: SQL queries with comments and expected outcomes

plsql.sql: PL/SQL blocks including procedure/function/trigger logic

admin.sql: User roles, privilege assignments, indexing

🚀 Execution Instructions
Connect to Oracle:

sql
Copy
Edit
sqlplus username/password@database
Run the scripts in order:

sql
Copy
Edit
@sql/setup.sql
@sql/queries.sql
@sql/plsql.sql
@sql/admin.sql
🗂️ Database Schema Overview
BOOKS
book_id, title, author, publisher, publication_year, isbn, category, total_copies, available_copies, price

MEMBERS
member_id, first_name, last_name, email, phone, address, membership_date, membership_type

TRANSACTIONS
transaction_id, member_id, book_id, issue_date, due_date, return_date, fine_amount, status

📌 Assignment Requirements Fulfilled
✔️ 20 books across multiple categories

✔️ 15 members (varied user types)

✔️ 25 transaction records with returned, overdue, and pending entries

✔️ All required SQL queries including joins, subqueries, analytics

✔️ Functional PL/SQL components with fine logic and inventory updates

✔️ User creation and performance indexing implemented
