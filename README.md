# Library-Management-System
Project Overview
The Library Management System is designed to efficiently manage all aspects of library operations, including book tracking, employee management, and customer interactions. The system provides a comprehensive database to keep records of branches, employees, books, customers, issue statuses, and return statuses.

Database Structure
The project consists of a database named library, which includes the following tables:

Branch

Branch_no (PRIMARY KEY)
Manager_Id
Branch_address
Contact_no
Employee

Emp_Id (PRIMARY KEY)
Emp_name
Position
Salary
Branch_no (FOREIGN KEY referencing Branch_no in the Branch table)
Books

ISBN (PRIMARY KEY)
Book_title
Category
Rental_Price
Status (values: 'yes' for available, 'no' for not available)
Author
Publisher
Customer

Customer_Id (PRIMARY KEY)
Customer_name
Customer_address
Reg_date
IssueStatus

Issue_Id (PRIMARY KEY)
Issued_cust (FOREIGN KEY referencing Customer_Id in the Customer table)
Issued_book_name
Issue_date
Isbn_book (FOREIGN KEY referencing ISBN in the Books table)
ReturnStatus

Return_Id (PRIMARY KEY)
Return_cust
Return_book_name
Return_date
Isbn_book2 (FOREIGN KEY referencing ISBN in the Books table)
