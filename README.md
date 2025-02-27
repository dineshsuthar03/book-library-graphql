# LibraryGraphQL

This is a simple proof-of-concept project that demonstrates a Flask-based GraphQL API for managing a library's book collection.

## Features
- Query all books in the library.
- Query a specific book by ID.
- Add a new book to the library.

## Setup

1. Create a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
Install the dependencies:

bash
Copy code
pip install -r requirements.txt
Run the Flask app:

bash
Copy code
python app.py
Access the GraphQL interface at:

arduino
Copy code
http://127.0.0.1:5000/graphql












Example Queries
Query all books:
graphql
Copy code
{
  allBooks {
    id
    title
    author
    year
  }
}
Query a specific book:
graphql
Copy code
{
  book(id: 1) {
    id
    title
    author
    year
  }
}
Mutation to add a new book:
graphql
Copy code
mutation {
  createBook(title: "Brave New World", author: "Aldous Huxley", year: 1932) {
    book {
      id
      title
      author
      year
    }
  }
}
mathematica
Copy code

#### 8. **Run the Application**
Run the Flask application to start the GraphQL API:
```bash
$ python app.py
Now, navigate to http://127.0.0.1:5000/graphql to access the GraphQL interface where you can try out the queries and mutations.

Example Queries and Mutations
Query all books:

graphql
Copy code
{
  allBooks {
    id
    title
    author
    year
  }
}
Query a specific book:

graphql
Copy code
{
  book(id: 1) {
    id
    title
    author
    year
  }
}
Add a new book:

graphql
Copy code
mutation {
  createBook(title: "Brave New World", author: "Aldous Huxley", year: 1932) {
    book {
      id
      title
      author
      year
    }
  }
}#   b o o k - l i b r a r y - g r a p h q l  
 