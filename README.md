AI Mood-Based Playlist Generator

Project Description

This project is a back-end application for a mood-based playlist generator. It is designed to interpret a user's mood using Gemini AI and then create a personalized music playlist from Spotify and Apple Music APIs. The application supports user authentication and persistent storage of playlist history using MongoDB and Clerk.

✨ Features

    User Authentication: Secure user authentication is handled by Clerk.

Mood-based Playlist Generation: Accepts a mood description from the user to generate a playlist. (Note: The core logic for API calls to Gemini, Spotify, and Apple Music is a placeholder in the provided code).

Playlist History: Allows authenticated users to view their past generated playlists.

Shareable Playlists: Publicly accessible routes to share individual playlists with anyone, regardless of their login status.

Database Integration: Utilizes MongoDB to store and manage user-specific data, including playlist history.

API Management: Handles API keys and credentials securely on the server-side.

🛠️ Technology Stack

    Backend: Node.js & Express

    Authentication: Clerk

    Database: MongoDB

    APIs: Gemini API, Spotify API, Apple Music API (planned integration) 

    Development Tools: nodemon

📋 Setup Instructions

Prerequisites

    Node.js

    npm or yarn

    A MongoDB Atlas account 

API keys from Google Gemini, Spotify, and Clerk 

API Keys and Environment Variables

Create a .env file in the root directory and populate it with your credentials:
Ini, TOML

PORT=8888
CLIENT_ID=f85cd5c6bae44670b4075e84e7d4012e
CLIENT_SECRET=6f3b6f21c0f5496db7764a46fcf197e2
REDIRECT_URI=http://localhost:8888/callback
GEMINI_API_KEY=AIzaSyD-mSI9ZUpMsymNCM9cf3zVh2bCNlRvWR4
FRONTEND_URI=http://localhost:3000
MONGO_URI=mongodb+srv://gousemoideen:Gouse12345!@cluster0.0bnjmyc.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0

Installation

    Clone the repository:
    Bash

git clone <repository_url>
cd <project_directory>

Install the dependencies listed in package.json:
Bash

npm install
# or
yarn install

The main dependency is nodemon, used for development.

Start the server:
Bash

    npm start
    # or
    yarn start

The server will start on the port specified in the 

.env file, which is 8888 by default.

🧪 Routes

    POST /generate

        Description: Generates a new playlist based on a mood. This is a protected route that requires a logged-in user.

    GET /history

        Description: Retrieves the playlist history for the authenticated user.

    GET /playlist/:id

        Description: Fetches a specific playlist by its ID. This is a public route.
