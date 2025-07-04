# Library Management System

![Library Management System Screenshot](screenshot.png)

A comprehensive Library Management System built with Python, SQLite, and Tkinter for managing book inventory, members, and transactions.

## Features ✨

- **📚 Book Management**  
  Add, edit, delete, and track book inventory
- **👥 Member Management**  
  Register and manage library members
- **🔄 Transaction Processing**  
  Handle book borrowing and returns
- **🗃️ Database Integration**  
  SQLite backend with 10+ relational tables
- **🖥️ User-Friendly GUI**  
  Tkinter interface with intuitive controls

## Database Schema 🗄️
```mermaid
erDiagram
    BOOK ||--o{ TRANSACTION : "has"
    BOOK ||--|{ AUTHOR : "written_by"
    BOOK ||--|{ PUBLISHER : "published_by"
    BOOK ||--|{ CATEGORY : "classified_as"
    MEMBER ||--o{ TRANSACTION : "makes"
    STAFF ||--|{ BRANCH : "works_at"
