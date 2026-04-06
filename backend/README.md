# Book Tracker API

## Overview

This is the backend API for the Book Tracker application. It is built using Node.js, Render, Netlify and PostgreSQL. The API allows users to retrieve, add, and update book data stored within a database.

## Installation & Setup

To run this project locally:

```bash
git clone https://github.com/hayezp/Module5-api.git
cd Module5-api
npm install
npm start
```

The server will run on:

```
http://localhost:5000
```

## API Documentation

### GET /api/v1/books

Returns all books.

### GET /api/v1/books/:id

Returns a single book by ID.

### GET /api/v1/books/distinct/titles

Returns unique book titles for dropdown.

### POST /api/v1/books

Creates a new book.

### PUT /api/v1/books/:id

Updates an existing book.

### Example Response

```json
{
  "id": 1,
  "title": "Book Title",
  "author": "Author Name",
  "genre": "Fiction",
  "published_year": 2020,
  "rating": 4.5
}
```

## Database Setup

Create a table:

```sql
CREATE TABLE books (
  id SERIAL PRIMARY KEY,
  title VARCHAR(150),
  author VARCHAR(120),
  genre VARCHAR(60),
  published_year INT,
  rating DECIMAL(2,1)
);
```

## Authentication & Security

This API does not have any current authentication. It is open for a class project and learning purposes.

## Deployment Guide

The backend is deployed on Render.

Live API:

```
https://module5-backend-api.onrender.com/api/v1/books
```

## Contributing
If you want to make changes to this project, you can:

1. Make a copy of the project (fork it)
2. Make your changes
3. Submit your changes

This project has been created for learning purposes in a programming class, so contributions are not required, but are gratefully accepted.

## License

This project is for school and learning purposes. There is no official license applied.