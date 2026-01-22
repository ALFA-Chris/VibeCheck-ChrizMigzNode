# VibeCheck-ChrizMigzNode
=================================================================
VIBECHECK 411L (VEGAS DASHBOARD EDITION)
=================================================================

VibeCheck 411L is a full-stack web application featuring a "Vegas-style" 
neon dashboard interface. It connects a responsive HTML/CSS frontend to 
a Node.js/Express REST API to deliver fortunes, jokes, mood analysis, 
and interactive counters.

------------------------------------------------------------------------
FEATURES
------------------------------------------------------------------------
- Neon Dashboard UI: Horizontal layout with glowing effects.
- Fortune Teller: Fetches randomized fortunes.
- Joke Generator: Delivers tech-humor on demand.
- Mood Analysis: Returns custom messages based on input.
- Smash Counter: Demonstrates POST requests (server-side counting).
- Secret Vault: Protected endpoint requiring a specific code (411L).

------------------------------------------------------------------------
PREREQUISITES
------------------------------------------------------------------------
1. Node.js (https://nodejs.org/)
2. npm (included with Node.js)

------------------------------------------------------------------------
INSTALLATION STEPS
------------------------------------------------------------------------
1. Create a folder and place these three files inside:
   - index.js
   - index.html
   - app.js

2. Open your terminal or command prompt in that folder.

3. Initialize the project:
   npm init -y

4. Install dependencies (Express and CORS):
   npm install express cors

------------------------------------------------------------------------
HOW TO RUN
------------------------------------------------------------------------
STEP 1: START THE BACKEND
   Run the following command in your terminal:
   node index.js

   (You should see: "VibeCheck API running at http://localhost:3000")

STEP 2: LAUNCH THE FRONTEND
   Keep the terminal open. Double-click the "index.html" file to open 
   it in your web browser.

------------------------------------------------------------------------
API ENDPOINTS (http://localhost:3000)
------------------------------------------------------------------------
GET  /api/fortune
   - Returns a random fortune.

GET  /api/joke
   - Returns a random developer joke.

GET  /api/vibe?mood=[happy|tired|stressed]
   - Returns a vibe check message based on the mood query.

POST /api/smash
   - Increments the server-side "Smash" counter.

GET  /api/smashes
   - Returns the current total smash count.

GET  /api/secret?code=411L
   - Returns a secret message if the code is correct.

------------------------------------------------------------------------
FILE DESCRIPTIONS
------------------------------------------------------------------------
- index.js   : The backend server logic (Node.js/Express).
- index.html : The user interface (HTML/CSS).
- app.js     : The client-side logic that connects buttons to the API.

===============================================================
Created for CPE 411L VibeCheck-ChrizMigzNode
===============================================================
