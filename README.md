# Server-side Online Book Review Application

## Overview
A server-side application that allows users to view book details and manages their reviews.

## Features
- Retrieve a list of all books available in the bookshop
- Search for specific books and retrieve their details based on the book’s ISBN code, author names and titles
- Retrieve reviews/comments for specified books
- Register as a new user of the application
- Login to the application
- Add a new review for a book (logged in users only)
- Modify a book review (logged in users can modify only their own reviews)
- Delete a book review (logged in users can delete only their own reviews)

## Tech Stack
- Node.js
- Express
- REST API
- JWT (Authentication)

## Project Flow
1. Client sends a GET request to the server url.
2. All Books retrieved.
3. Client sends to GET request to retrieve books based on isbn, author and title.
4. Client specified book details retrieved.
5. Client sends the GET request to retrieve book review based on isbn specified in the url.
6. Book reviews retrieved.
7. Client sends a login request.
8. Client is authenticated and user jwt is generated.
9. On subsequent requests from client which require authentication Client is verified then request is processed.

## Installation & Setup
Clone the repository  
git clone https://github.com/JayaNeem/expressBookReviews.git

Navigate into the folder  
cd expressBookReviews/final_project

Run the project  
node index.js

## Key Concepts Learned 
- JWT Authentication

## Future Improvements
- (Multiple users) Access the application at the same time to view and manage different book reviews simultaneously.

## Notes
This project was created as part of learning Node and Express from Coursera. (Final Project)
