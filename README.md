AI Mood-Based Playlist Generator

Project Description

This project is a mood-based playlist generator that uses artificial intelligence to create personalized music playlists. Users can simply type in a mood or vibe, and the application leverages the Gemini AI to interpret the prompt and the Spotify API to curate a custom playlist.

The application aims to provide a seamless and intuitive experience, allowing users to discover new music that perfectly matches their current state of mind.

✨ Features

    Natural Language Processing: Input your mood using simple, everyday language.

    Gemini AI Integration: Utilizes AI to understand and interpret your mood description.

    Spotify API Connectivity: Generates and displays a playlist directly from Spotify's vast music library.

    Interactive UI: View track details, album art, and easily play or open the playlist in Spotify.

    Responsive Design: Optimized for a smooth experience on both desktop and mobile devices.

🚀 Demo

    Live Demo: [Link to your live demo, e.g., on Vercel or Netlify]

    Video Walkthrough: [Link to a short video demo, e.g., on YouTube or Loom]

🛠️ Technology Stack

    Frontend:

        React.js

        [UI Library, e.g., Tailwind CSS, Material-UI]

    Backend:

        Node.js & Express

    APIs:

        Google Gemini API

        Spotify API

📋 Setup Instructions

Prerequisites

    Node.js (v14 or higher)

    [yarn or npm]

API Keys

    Google Gemini API: Obtain your API key from the Google AI Studio.

    Spotify API:

        Go to the Spotify for Developers Dashboard.

        Create a new application to get your Client ID and Client Secret.

.env File

Create a .env file in the root of the project with the following variables:

REACT_APP_GEMINI_API_KEY=[Your Gemini API Key]
REACT_APP_SPOTIFY_CLIENT_ID=[Your Spotify Client ID]
REACT_APP_SPOTIFY_CLIENT_SECRET=[Your Spotify Client Secret]

Installation

    Clone the repository:
    Bash

git clone [your-repo-link]
cd [your-project-folder]

Install dependencies:
Bash

# For both frontend and backend
npm install
# or
yarn install

Run the application:
Bash

    npm start
    # or
    yarn start

The application will be available at http://localhost:3000.
