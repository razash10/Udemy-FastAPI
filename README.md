# Udemy-FastAPI
Udemy course for learning FastAPI - RESTful APIs using Python, SQLAlchemy, OAuth, JWT and more

## Books Project

This project is a simple FastAPI application for managing a collection of books. It includes the following features:

- **Read all books**: Retrieve a list of all books.
- **Read a book by title**: Retrieve a book by its title.
- **Read books by category**: Retrieve books by their category.
- **Read books by author**: Retrieve books by their author.
- **Read books by author and category**: Retrieve books by their author and category.
- **Create a new book**: Add a new book to the collection.
- **Update a book**: Update the details of an existing book.
- **Delete a book**: Remove a book from the collection.

### Endpoints

- `GET /books`: Retrieve all books.
- `GET /books/{book_title}`: Retrieve a book by its title.
- `GET /books/`: Retrieve books by category (query parameter `category`).
- `GET /books/byauthor/`: Retrieve books by author (query parameter `author`).
- `GET /books/{book_author}/`: Retrieve books by author and category (query parameters `book_author` and `category`).
- `POST /books/create_book`: Create a new book.
- `PUT /books/update_book`: Update an existing book.
- `DELETE /books/delete_book/{book_title}`: Delete a book by its title.

### Running the Application

To run the application, use the following command:

```sh
uvicorn 1_Books.books:app --reload
```

### API Documentation

Once the application is running, you can access the interactive API documentation at: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
