# ShelfTrack — Library Management System

A desktop library management system built in Java with a MySQL backend, 
developed as my final project for the PSI (Programação de Sistemas 
Informáticos) course.

## About
ShelfTrack replaces manual library record-keeping with a structured digital 
system for managing books, readers, and loans. It was built following an 
iterative development approach, with continuous testing of authentication, 
loan/return flows, and automatic book status updates.

## Features
- User authentication with bcrypt-hashed passwords
- Role-based views (Manager / Employee)
- Book catalog management (title, author, ISBN, genre, availability)
- Reader registry
- Loan tracking with due dates and automatic status (`Loan` / `Returned` / `Late`)
- Search/filter functionality

## Tech Stack
- Java (Swing, NetBeans)
- MySQL
- Architecture: DAO / DTO / VIEW layers

## Database Schema
4 relational tables (`livros`, `leitores`, `utilizadores`, `emprestimos`) with 
foreign key constraints. See `shelftrack_bd.sql` for the full schema.

## How to Run
1. Import `shelftrack_bd.sql` into a local MySQL instance
2. Open the project in NetBeans
3. Update database credentials in `ConexaoDAO.java` if needed
4. Run the project

## Known Improvements
- Database credentials are currently hardcoded — should be moved to an 
  environment variable or config file
- Planned but not implemented: automatic return notifications, a statistics 
  module for loan history

## Screenshots
<img width="414" height="378" alt="image" src="https://github.com/user-attachments/assets/22bc2dea-194a-4cd3-b30a-e48a2c9e377f" />

<img width="245" height="178" alt="image" src="https://github.com/user-attachments/assets/55523bce-2505-4617-9b45-325f669550a3" />

<img width="428" height="241" alt="image" src="https://github.com/user-attachments/assets/7c562722-2996-4404-ba07-a4a591ab9762" />

