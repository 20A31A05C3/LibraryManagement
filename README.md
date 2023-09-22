**Library Management System**
__Overview__
The Library Management System is a Python application designed to streamline library operations. It utilizes the Tkinter library for the graphical user interface and pymysql for database connectivity. This software simplifies the management of a library's inventory and keeps track of book issuances efficiently.

__Features__
Librarian Interface:
Add Books: Easily add books to the library database, including details like subject, title, author, and serial number.
Issue and Return Books: Manage the issuance and return of books to/from students with a straightforward interface.
View Available Books: Instantly check the list of books available in the library for easy reference.
View Issued Books: Keep track of books that have been issued to students.
Delete Books: Remove books from the database when necessary.
Admin Interface:
User Management: Admins can add and manage users, including librarians and other administrators.
View User Information: Access user information such as name, user ID, branch, and mobile number.
Delete Users: Admins have the authority to delete users as required.

__Prerequisites__
Before running the application, make sure you meet the following prerequisites:

Python is installed on your system.

The pymysql package for MySQL database connectivity is installed. You can install it using:

pip install pymysql
__Usage__
Follow these steps to use the Library Management System:

Clone or download this repository to your local machine.

Navigate to the project directory:

cd Library-Management-System

Run the application:

python library_management_system.py

Log in as either a librarian or an admin.

Librarians can manage books, issue/return books, and perform related tasks.
Admins can add/manage users and access user-related functions.

__Database Setup__
The application relies on a MySQL database to store book and user information. To set up the database, follow these steps:

Install MySQL on your system if it's not already installed.

Start the MySQL server.

Create a new database named "Library."

Within the "Library" database, create the following tables:

Book: Stores book information, including subject, title, author, and serial number.
BookIssue: Tracks book issuance details such as student ID, serial number, issue date, and expiry date.
Login: Stores user information, including name, user ID, branch, and mobile number.
Update the database connection details in the code (library_management_system.py) to match your MySQL server configuration:

python

con = pymysql.connect(host="localhost", user="root", password="your_mysql_password", database="Library")

__Contributing__

Contributions to this project are highly encouraged! If you encounter any issues, have ideas for new features, or want to suggest improvements, please don't hesitate to open an issue or submit a pull request.
