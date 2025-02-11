
---

# Book Search Engine

## Description

The **Book Search Engine** is a full-stack application that allows users to search for books using the Google Books API. Originally built with a RESTful API, this project has been refactored to use GraphQL with Apollo Server, offering an optimized and flexible way to manage data requests. The application is built using the **MERN stack**: MongoDB, Express.js, React, and Node.js.

Users can search for books, view book details, and save their favorite books to their personal collection on the back end.

## Key Features

- **Book Search**: Search for books using the Google Books API.
- **Save Books**: Save favorite books to the back-end MongoDB database.
- **Authentication**: User authentication with JWT to securely manage accounts.
- **GraphQL API**: Replaced the existing RESTful API with a GraphQL API using Apollo Server.
- **Deployment**: Deployed to Render with a MongoDB database hosted on MongoDB Atlas.

## Technologies Used

- **MongoDB**: Database to store saved books and user data.
- **Express.js**: Server framework for building the back-end API.
- **React**: Front-end library for building the user interface.
- **Node.js**: JavaScript runtime for the server-side logic.
- **Apollo Server**: GraphQL server to handle queries and mutations.
- **JWT Authentication**: Secure user authentication.
- **MongoDB Atlas**: Cloud-based MongoDB database.
- **Render**: Platform for deploying the application.

## Installation

To run the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables:
   - Create a `.env` file in the root directory.
   - Add necessary variables, such as `MONGODB_URI`, `JWT_SECRET`, and others.
4. Run the application:
   ```bash
   npm run develop
   ```

## Usage

Once the application is running, you can:

1. Sign up or log in to your account.
2. Search for books by title, author, or subject.
3. Save books to your personal collection for later access.
4. View and manage saved books.

## API

The application now uses **GraphQL** to handle data fetching and mutations. Here's a brief overview of the available queries and mutations:

- **Queries**:
  - `searchBooks(query: String!)`: Search for books using a query string.
  - `me`: Fetch the authenticated user's data.
  - `savedBooks`: Fetch the user's saved books.

- **Mutations**:
  - `saveBook(bookData: BookInput!)`: Save a book to the user's collection.
  - `removeBook(bookId: ID!)`: Remove a book from the user's collection.

## Deployment

The application is deployed to **Render** with a MongoDB database hosted on **MongoDB Atlas**. To view the live version of the app, visit the link below:

[Live Application](https://book-search-xhlx.onrender.com/)

## Contributing

Thanks to **OpenAI** and my **classmates** for their help and guidance in with this project.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- **Classmates** for their feedback and suggestions.
- **ChatGPT** for assistance with coding and project setup.

---
