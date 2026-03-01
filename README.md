
# FastAPI CRUD Library

A RESTful API built with FastAPI for managing a book library with full CRUD operations.

## Features

- **GET /books** - Retrieve all books
- **GET /books/title/{title}** - Search books by title
- **GET /books/** - Filter books by year and author (query parameters)
- **POST /books/create_book** - Add a new book
- **PUT /books/update_book** - Update an existing book
- **DELETE /books/delete_book/{id}** - Remove a book by ID

## Setup

1. Install dependencies: `pip install fastapi`
2. Load book data from `library.json`
3. Run with: `uvicorn api:app --reload`

## Query Parameters

- `start_year` (int): Filter books published after this year (default: 1950, range: 1500-current year)
- `author` (str): Filter by author name (optional)
