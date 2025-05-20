# LibraryDatabaseManagmentSystem
## Project Description

This project implements a **Library Management System** database using MySQL.  
It manages core data entities such as **Authors, Books, Members**, and **Borrowings** with properly defined relationships and constraints.  

### Key Features:
- Stores information about books and their authors (many-to-many relationship).
- Tracks library members.
- Manages book borrowings, including borrow date, due date, and return date.
- Enforces data integrity using primary keys, foreign keys, and constraints.

## Database Design

The database schema includes the following tables:

- **Authors:** Stores author details.
- **Books:** Stores book information with ISBN and available copies.
- **BookAuthors:** Join table for many-to-many relationship between books and authors.
- **Members:** Stores library member details.
- **Borrowings:** Tracks which member borrowed which book and related dates.

## How to Setup

1. Install MySQL on your system if you haven’t already.
2. Open MySQL Workbench or your preferred MySQL client.
3. Create a new schema (database), e.g. `LibraryDB`.
4. Run the provided `library_management.sql` file to create all tables and insert sample data.

```bash
mysql -u your_username -p LibraryDB < library_management.sql
