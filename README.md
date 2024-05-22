# Server-Side Repository: Tails & Tables

## Introduction

Welcome to the Tails & Tables server-side repository! This server provides the API for the Tails & Tables mobile application, supporting user authentication, profile management, place discovery, reviews, and favorites functionality.

## Features

- **User Management**: Register, login, and manage user profiles.
- **Place Data**: Fetch and provide data for pet-friendly places.
- **Reviews**: Handle user reviews for places.
- **Favorites**: Manage user favorite places.

## Tech Stack

- **MongoDB**: For the database.
- **Express.js**: For the server framework.
- **Node.js**: For the server environment.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/tails-and-tables-server.git
    cd tails-and-tables-server
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Environment variables**:
    Create a `.env` file in the root directory and add the following:
    ```env
    PORT=5000
    MONGODB_URI=your_mongodb_uri
    JWT_SECRET=your_jwt_secret
    ```

4. **Start the server**:
    ```bash
    npm start
    ```

## Directory Structure

tails-and-tables-server/
├── controllers/ # Route handlers
├── models/ # Mongoose models
├── routes/ # Express routes
├── middleware/ # Middleware functions
├── utils/ # Utility functions
├── config/ # Configuration files
├── server.js # Entry point of the server
├── package.json # Dependencies and scripts
└── README.md # Project documentation

markdown
Copiar código

## API Endpoints

- **Authentication**:
  - `POST /api/auth/register`: Register a new user.
  - `POST /api/auth/login`: Login a user.

- **User Profile**:
  - `GET /api/user/profile`: Get user profile.
  - `PUT /api/user/profile`: Update user profile.

- **Places**:
  - `GET /api/places`: Get nearby pet-friendly places.

- **Reviews**:
  - `POST /api/reviews`: Submit a review.
  - `GET /api/reviews/:placeId`: Get reviews for a place.

- **Favorites**:
  - `POST /api/favorites`: Add a place to favorites.
  - `GET /api/favorites`: Get user's favorite places.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

