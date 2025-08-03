🃏 Memorizing Game
A web-based memory card matching game built using Flask, JavaScript, HTML/CSS, and SQLite.

<br>
🖼️ Project Screenshot


<br>
🎮 Game Rules
The game uses a standard 52-card deck (spades, hearts, diamonds, clubs; each from 1 to 13).

All cards are laid face down at the start of the game.

Players can flip two cards at a time:

✅ If the numbers match (e.g., 7♦ and 7♠), they stay face up.

❌ If not, they flip back down.

Each correct match scores 10 points.

The goal is to match all 26 pairs for a total of 260 points.

<br>
💻 Features
🔐 User registration and login/logout system

📊 Individual player score tracking via SQLite database

🧠 Game logic entirely in JavaScript

📝 Responsive frontend with real-time score and attempt counter

🔄 Server-managed session to persist login state

<br>
📁 Project Structure
graphql
複製
編輯
project/
├── static/
│   ├── app.js               # JavaScript logic for the card game
│   └── style/
│       └── style.css        # Styling for the game UI
├── templates/
│   ├── index.html           # Game interface (after login)
│   └── layout.html (optional)
├── database.db              # SQLite database file (auto-generated)
├── app.py                   # Flask backend logic
└── README.md                # You are here
<br>
🧠 Tech Stack
Layer	Tech
Frontend	HTML, CSS, JavaScript
Backend	Python (Flask)
Database	SQLite
Auth	Flask Sessions
Deployment	Localhost / Flask server

<br>
🚀 How to Run
Install dependencies

bash
複製
編輯
pip install flask
Start the Flask server

bash
複製
編輯
python app.py
Play the game

Visit http://127.0.0.1:5000

Register an account

Log in

Enjoy matching cards!

🔒 Note: The database file database.db will be created automatically on first run.

<br>
🗃️ Database Schema
users

id (INTEGER PRIMARY KEY)

username (TEXT, unique)

password (TEXT)

scores

id (INTEGER PRIMARY KEY)

user_id (INTEGER, FOREIGN KEY)

score (INTEGER, default 0)

tries (INTEGER, default 0)

<br>
✅ To Do (Optional Improvements)
 Show player’s score history

 Add timer and ranking

 Add game restart or new round button

 Hash passwords using werkzeug.security

 Deploy to cloud (e.g., Render, Heroku)

<br>
🙋 Author
Made with 💡 and 🎹 by Rachel Tsai
Based on CS50 Web Programming
