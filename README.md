# Library-MS-Project 
README
📚 JournalEase - Library Management System
JournalEase is a modern Library Management System (LMS) built to streamline the management of books, track borrowing records, and enhance the user experience for both librarians and patrons. It offers an intuitive interface and robust backend using Python, Tkinter, and MySQL.

📌 Key Features
Add Book: Add new books to the library collection with ease.
Search Book: Quickly find books by Title, Author, or ISBN.
Issue Book: Efficiently issue books to library users.
Book Holder: Keeps track of who currently has a specific book.
Return Book: Mark books as returned and update availability.
View All Books: Display a complete list of books in the system.
Update and Delete Book Records
🛠️ Technologies Used
Python: Backend logic implementation using a versatile and readable language.
Tkinter: GUI development for a clean and user-friendly desktop interface.
MySQL: Relational database to manage books, users, and transactions efficiently.
PyMySQL: Interface between Python and MySQL database.
📷 UI Snapshots 
https://private-user-images.githubusercontent.com/82410098/439614082-b443194a-5c95-4e97-a1bd-962d3124df44.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NDcyOTUxMTUsIm5iZiI6MTc0NzI5NDgxNSwicGF0aCI6Ii84MjQxMDA5OC80Mzk2MTQwODItYjQ0MzE5NGEtNWM5NS00ZTk3LWExYmQtOTYyZDMxMjRkZjQ0LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA1MTUlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwNTE1VDA3NDAxNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTY0YWFmNzkxN2Q1NzliYWRkYjhkNmQ5NTU4OTAyYjE5NDIwYWYxN2ZhODNjOGY3MzY2OWM2MmQ2NmMyMDJlZjkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.cB_hKcjsVjDI6Y3f4PA5mRW1wZdeOVcFK2o7wVmRJ2g
All Books Add Book Search Book 2 Search Book 1 Issue Book Return book 2 Return Book 1

📁 Project Structure
main.py : Main logic and GUI functionality
custom.py : Font and color configuration
credentials.py : MySQL username and password (user-defined)
🛢️ Database
CREATE DATABASE library_management;
CREATE TABLE book_list(
	book_id VARCHAR(10) NOT NULL,
	book_name VARCHAR(50) NOT NULL,
	author VARCHAR(50) NOT NULL,
	edition VARCHAR(10) NOT NULL,
	price Int(6) NOT NULL,
	qty Int(4) NOT NULL,
	PRIMARY KEY ( book_id )
); 
CREATE TABLE borrow_record(
	book_id VARCHAR(10) NOT NULL,
	book_name VARCHAR(50) NOT NULL,
	stu_roll VARCHAR(15) NOT NULL,
	stu_name VARCHAR(50) NOT NULL,
	course VARCHAR(10) NOT NULL,
	subject VARCHAR(30) NOT NULL,
	issue_date date NOT NULL,
	return_date date NOT NULL
);
Developed as a part of the OOP Lab Project at Daffodil International University.

