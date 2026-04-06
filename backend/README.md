# Book Tracker API

## Overview

This is the backend API for the Book Tracker application. It is built using Node.js, Express, and PostgreSQL. The API allows users to retrieve, add, and update book data stored in a database.

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

This API does not currently use authentication. It is open for learning purposes.

## Deployment Guide

The backend is deployed on Render.

Live API:

```
https://module5-backend-api.onrender.com/api/v1/books
```

## Contributing

To contribute:

1. Fork the repo
2. Create a branch
3. Make changes
4. Submit a pull request

## License

This project uses the MIT License.