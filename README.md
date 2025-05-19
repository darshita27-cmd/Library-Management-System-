# Library-Management-System-
# Library Database System

This repository contains a SQL database system for managing a library's operations, including user information, book inventory, circulation records, and fines.

## Database Schema

### Tables

1. **USERS**
   - Stores library user information
   - Fields: USER_ID (PK), USER_NAME, ADDRESS, CONTACT

2. **BOOKS**
   - Contains book inventory details
   - Fields: BOOK_CODE (PK), TITLE, AUTHOR_NAME, PUBLISHER, ISBN, NUMBER_OF_COPIES, EDITION

3. **CIRCULATION**
   - Tracks book checkouts and returns
   - Fields: USER_ID, BOOK_CODE, ISSUE_DATE, DUE_DATE, RETURN_DATE

4. **FINES**
   - Records fines imposed on users
   - Fields: USER_ID, BOOK_CODE, AMOUNT, REASON_OF_FINE

### Views

- **USER_FINE**: Aggregates fine information with user and book details

## Setup Instructions

1. Execute the SQL script to:
   - Create the database
   - Create all tables
   - Populate with sample data
   - Create the view

2. The script includes:
   - Sample user records (30 users)
   - Sample book records (multiple copies of 30 different titles)
   - Sample circulation records
   - Sample fine records

## Features

- Tracks multiple copies of each book title
- Manages book checkouts, due dates, and returns
- Records fines for late returns, damaged books, and lost books
- Provides a view to see user fines with book details

## Sample Queries

The script includes several example operations:
- Database and table creation
- Data insertion
- Table alterations (column rename)
- Data updates
- Data deletion

## Notes

- The database is designed for a library management system
- Includes relationships between users, books, and circulation records
- Contains sample data for testing and demonstration purposes

To use, simply execute the entire SQL script in your MySQL environment.
