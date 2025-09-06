# Library_Management_System
Overview

This is a simple Java-based Library Management System that simulates basic library operations such as issuing and returning books. The system consists of three classes: Book, Member, and Library. It demonstrates object-oriented programming concepts, including encapsulation and interaction between objects.

Files
Book.java: Defines the Book class, which represents a book with a unique number and an issuance status (isIssued).
Member.java: Defines the Member class, which represents a library member who can issue and return books.
Library.java: Contains the main method to demonstrate the functionality of issuing and returning books.

Functionality
Book Class:
Stores a book’s number and issuance status.
Provides a toString method to display the book’s status.

Member Class:
Allows a member to issue a book if it is not already issued and the member has no other book.
Allows a member to return a book, making it available again.

Library Class:
Creates sample books and members.
Demonstrates issuing and returning books with appropriate console output.

Prerequisites
Java Development Kit (JDK) 8 or higher.
A Java compiler (e.g., javac).
A terminal or IDE to compile and run the program.

How to Run
Ensure Files are in the Same Directory:
Place Book.java, Member.java, and Library.java in the same directory.

Compile the Program:

javac Library.java

This command compiles all three files (Library.java, Book.java, Member.java) as they are interdependent.


Run the Program:
java Library

Expected Output:
Ravi issued Book 1
Cannot issue Book 1 to Neha
Ravi returned Book 1
Neha issued Book 1
Book 1 (Issued: true)
Book 2 (Issued: false)

Code Structure
Book.java:
Attributes: number (int), isIssued (boolean).

Constructor: Initializes the book number.
Method: toString() for displaying book details.

Member.java:
Attributes: name (String), issuedBook (Book).
Methods: issueBook(Book) to issue a book, returnBook() to return a book.

Library.java:
Contains the main method to create books and members, simulate issuing/returning, and display results.

Notes
The program enforces rules such as preventing a book from being issued if it’s already issued or if a member already has a book.
The code is kept simple for demonstration purposes and can be extended with features like multiple book issuance, a book catalog, or user input.
If you prefer a single-file setup, you can combine all classes into Library.java by removing the public modifier from Book and Member classes, though separate files are recommended for better organization.

Limitations
The program uses hardcoded books and members.
It does not persist data (e.g., to a file or database).
Only one book can be issued to a member at a time.

Future Enhancements
Add a user interface for interactive input.
Support multiple book issuances per member.
Implement a database for persistent storage.
Add error handling for edge cases.
