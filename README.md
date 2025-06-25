## Library Management System using MySQL Workbench
This project demonstrates a basic Library Management System implemented using MySQL Workbench. It includes tables for Authors, Books, Members, and Borrow with CRUD operations: Insert, Select, Update, and Delete.

# Tools Used
MySQL Workbench

SQL Language

Result Grid for output visualization

# Tables Overview
Authors: Stores author details.

Books: Stores book details with reference to authors.

Members: Stores member information.

Borrow: Tracks which member borrowed which book, and when.

# INSERT Commands
sql
Insert into Borrow values(60, 1, 9849, '2025/05/09', '2025/06/11');
Insert into Borrow values(84, 1, 8216, '2025/06/15', '2025/07/08');
Insert into Borrow values(70, 3, 9849, '2023/12/17', '2024/01/11');
Insert into Borrow values(44, 2, 9704, '2023/05/30', '2023/06/30');
Insert into Borrow values(98, 2, 9704, '2025/01/06', '2025/02/01');
Insert into Borrow values(86, 4, 8216, '2024/09/09', '2024/10/25');

Output: Records were successfully inserted into the Borrow table.

# SELECT Commands
sql
select * from Authors;
select * from Books;
select * from Members;
select * from Borrow;

Output:

Authors: Lists author IDs and names like Pushkal Sharma, Anjana Nair, Trevor Noah.

Books: Displays book details such as title, genre, and associated author.

Members: Shows member info including name, email, and phone number.

Borrow: Shows which member borrowed which book and the respective dates.

# UPDATE Command
sql
update Borrow set ReturnDate = null where BorrowID = 98;

Output: The ReturnDate of the record with BorrowID = 98 is set to NULL.

# DELETE Command
sql
delete from Borrow where BorrowID = 84;

Output: The record with BorrowID = 84 was deleted from the Borrow table.
