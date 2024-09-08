# Echo - Real-Time Messaging Application

## Introduction
**Echo** is a real-time messaging application designed for secure, fast, and user-friendly communication. Built using the **MERN** stack (MongoDB, Express.js, React.js, Node.js), it allows users to send messages instantly without any page reloads and provides real-time updates on user presence.

### Key Features:
- **Real-time messaging**: Instant delivery of messages using Socket.io.
- **User-friendly design**: Built with a responsive and dynamic interface using React.js.
- **Secure communication**: Utilizes JSON Web Tokens (JWT) for secure authentication and authorization.
- **Low-latency performance**: Powered by Socket.io for smooth and efficient communication.
- **Scalable backend**: A robust backend using MongoDB to handle user data and chat history.

## Technology Stack

- **MongoDB**: NoSQL database for storing user information and chat messages.
- **Express.js**: Backend web framework that simplifies building web servers and APIs.
- **React.js**: Frontend library for creating dynamic and responsive user interfaces.
- **Node.js**: Server-side environment that enables JavaScript execution outside the browser.
- **Socket.io**: Handles real-time, bidirectional communication between clients and the server.
- **JWT**: Ensures secure authentication and authorization.

## Project Structure

```plaintext
Echo-main/
├── client/               # Frontend code
│   ├── public/           # Public files (index.html, assets)
│   ├── src/              # React components, pages, and utilities
│   │   ├── assets/       # Static resources (images, etc.)
│   │   ├── components/   # UI components (NavBar, Chat, etc.)
│   │   ├── context/      # Context API for state management
│   │   ├── hooks/        # Custom hooks for reusability
│   │   ├── pages/        # Main pages of the app
│   │   ├── utils/        # Utility functions
│   │   ├── App.jsx       # Main React component
│   │   ├── index.css     # Global CSS styling
│   │   ├── main.jsx      # Entry point for React app
│   └── vite.config.js    # Vite configuration for bundling
├── server/               # Backend code
│   ├── Controller/       # Request handlers for the API
│   ├── Models/           # MongoDB models for users, messages
│   ├── Routes/           # API routes (authentication, chat)
│   ├── index.js          # Entry point for Express server
│   ├── .env              # Environment variables
│   ├── package.json      # Server dependencies
├── socket/               # Socket.io code
│   ├── index.js          # Handles real-time events and user connections
│   ├── package.json      # Socket dependencies
```

## Core Functionality

- **Real-Time Communication**: Messages are transmitted instantly between users using **Socket.io**, which provides real-time, low-latency bidirectional communication between the server and connected clients. No page refresh is needed as messages are delivered as soon as they're sent.
  
- **User Presence**: The app also shows the online status of users, allowing participants to see who is currently available for chat.

- **Secure Authentication**: The authentication system is based on **JWT** (JSON Web Tokens), ensuring that user sessions are secure and protected.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/echo.git
   ```
2. Navigate to the server and install dependencies:
   ```bash
   cd server
   npm install
   ```
3. Navigate to the client and install dependencies:
   ```bash
   cd client
   npm install
   ```
4. Start the application:
   - Backend (Express server):
     ```bash
     node index.js
     ```
   - Frontend (React app):
     ```bash
     npm run dev
     ```
     - Socket IO (for Real-time messaging):
     ```bash
     node index.js
     ```

5. The app should now be running on `http://localhost:3000` for the client and `http://localhost:5000` for the server.

## Conclusion
Echo is a fully-featured real-time messaging app built using modern technologies for both the frontend and backend. It provides a secure and efficient communication platform with low latency and a user-friendly interface.
