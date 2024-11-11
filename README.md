## Simple Library Management System

A basic library management system built with React and MySQL.

### Features
- View available books
- Borrow books
- Track borrowed books
- Basic user authentication

### Tech Stack
- Frontend: React + TypeScript + Tailwind CSS
- Backend: Node.js + Express
- Database: MySQL

### Setup Instructions
1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up MySQL database:
   ```bash
   mysql -u root -p < schema.sql
   ```
4. Start the application:
   ```bash
   npm run dev
   ```

### Database Schema
- Users (id, name, email, password, role)
- Books (id, title, author, isbn, available)
- Borrows (id, book_id, user_id, borrow_date, return_date)

### API Endpoints
- GET /api/books - Get all books
- POST /api/books/borrow - Borrow a book
- GET /api/borrows - Get user's borrowed books
- POST /api/auth/login - User login
- POST /api/auth/register - User registration

### License
MIT