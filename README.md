# Library-MS-Project 

:

📚 JournalEase - Library Management System
JournalEase is a modern Library Management System (LMS) designed to streamline book management, track borrowing records, and enhance the experience for both librarians and patrons. Built with Python, Tkinter, and MySQL, it features an intuitive graphical interface and a powerful backend.

🚀 Features
🔹 Add Book – Easily add new books to the library collection.

🔍 Search Book – Find books by Title, Author, or ISBN.

📖 Issue Book – Efficiently issue books to library users.

🙋‍♂️ Book Holder – Track who currently has a specific book.

🔄 Return Book – Mark books as returned and update availability.

📚 View All Books – Display a complete list of books in the system.

✏️ Update & Delete Book Records – Modify or remove existing book entries.

🛠️ Technologies Used
Python – Backend logic with a clean, versatile language.

Tkinter – Desktop GUI framework for a responsive user interface.

MySQL – Relational database for managing book records and transactions.

PyMySQL – Connects Python with the MySQL database.

🖼️ UI Snapshots
All Books
![Screenshot_15-5-2025_141332_github com](https://github.com/user-attachments/assets/a78ad8cc-bdaf-4d95-bbd0-a61dc7d79f6e)

Add Book
![Screenshot_15-5-2025_14142_github com](https://github.com/user-attachments/assets/e00a7e95-c26b-4a21-9b1f-de511e2de561)
![Screenshot_15-5-2025_141455_github com](https://github.com/user-attachments/assets/2bd118ea-93d0-446c-9591-030c748162a3)

Search Book (Example 1 & 2)
![Screenshot_15-5-2025_141532_github com](https://github.com/user-attachments/assets/15e46765-dde0-4437-ae23-b24f6eb29b9c)
![Screenshot_15-5-2025_141634_github com](https://github.com/user-attachments/assets/c14f1a65-7d36-4f2e-a6d4-d1cbe5d78e31)

Issue Book
![S![Screenshot_15-5-2025_141657_github com](https://github.com/user-attachments/assets/c61ed194-7ad0-4aaa-8055-2dc38254f4be)
creenshot_15-5-2025_141558_github com](https://github.com/user-attachments/assets/890c7ae5-8e1c-479e-b634-c751fc701248)

Return Book (Example 1 & 2)
![Screenshot_15-5-2025_141657_github com](https://github.com/user-attachments/assets/adbe8184-aed1-4353-a735-12a9d51b0c98)


📁 Project Structure
plaintext
Copy
Edit
📁 JournalEase/
├── main.py            # Main application logic and GUI
├── custom.py          # UI styling (fonts, colors, etc.)
├── credentials.py     # MySQL credentials (user-defined)
🛢️ Database Schema
sql
Copy
Edit
CREATE DATABASE library_management;

CREATE TABLE book_list (
    book_id VARCHAR(10) NOT NULL,
    book_name VARCHAR(50) NOT NULL,
    author VARCHAR(50) NOT NULL,
    edition VARCHAR(10) NOT NULL,
    price INT(6) NOT NULL,
    qty INT(4) NOT NULL,
    PRIMARY KEY (book_id)
);

CREATE TABLE borrow_record (
    book_id VARCHAR(10) NOT NULL,
    book_name VARCHAR(50) NOT NULL,
    stu_roll VARCHAR(15) NOT NULL,
    stu_name VARCHAR(50) NOT NULL,
    course VARCHAR(10) NOT NULL,
    subject VARCHAR(30) NOT NULL,
    issue_date DATE NOT NULL,
    return_date DATE NOT NULL
);
🎓 Project Info
Developed as part of the Object-Oriented Programming (OOP) Lab Project at Daffodil International University.

