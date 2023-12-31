# Bookstore Management System

The Bookstore Management System is a web application built using TypeScript, Node.js, and MongoDB. It provides functionality for managing categories, books, and variants in a bookstore.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
  - [Categories](#categories)
  - [Books (Products)](#books-products)
  - [Variants](#variants)
- [Error Handling](#error-handling)
- [Dependencies](#dependencies)
- [Conclusion](#conclusion)

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js: [Download and Install Node.js](https://nodejs.org/)
- MongoDB: [Download and Install MongoDB](https://www.mongodb.com/try/download/community)
- Git: [Download and Install Git](https://git-scm.com/)

## Getting Started

1. Clone the repository to your local machine:

   ```bash git clone <repository_url>```
  - 1. Navigate to the project directory:
       ```cd bookstore-management-system```
  - 2. Create a .env file in the project root directory and add the following environment variables:
        ```PORT=5000 # Port on which the server will run```
       ```MONGO_URL=mongodb://localhost/bookstore # MongoDB connection URL```

  - 3. Install project dependencies by running:
       ```npm install```
       
 ## Running the Application
 
   To start the Bookstore Management System on local system, use the following command:
   ``` npm start```

  This will start the server, and you should see a message indicating that the server is running on the specified port.

  ## API Endpoints

  The system provides the following API endpoints for managing categories, books (products), and variants:
  
  ### Categories
    GET /api/categories: Get a list of all categories.
    POST /api/categories: Create a new category.
    PUT /api/categories/:id: Update an existing category by ID.
    DELETE /api/categories/:id: Delete a category by ID.
    
  ### Books (Products)
    GET /api/books: Get a list of all books.
    POST /api/books: Create a new book.
    PUT /api/books/:id: Update an existing book by ID.
    DELETE /api/books/:id: Delete a book by ID.
    Variants
    GET /api/variants: Get a list of all variants.
    PUT /api/variants/:id: Update an existing variant by ID.
    DELETE /api/variants/:id: Delete a variant by ID.
    
  ### Error Handling
    Accessing an invalid endpoint will result in a 404 Not Found error.
  
  ### Dependencies
    The system uses the following main dependencies:
  
    Express.js: A web application framework for Node.js.
    Mongoose: An Object Data Modeling (ODM) library for MongoDB and Node.js.
    dotenv: A module for loading environment variables from a .env file.
    
  ### Conclusion
    You now have the Bookstore Management System up and running on your local machine. Use the provided API endpoints to manage categories, books, and variants in your bookstore. 
    Customize and extend the system according to your needs.
