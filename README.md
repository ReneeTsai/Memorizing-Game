# 🃏 Memorizing Game

A web-based memory card matching game built using **Flask**, **JavaScript**, **HTML/CSS**, and **SQLite**.

## 📸 Project Screenshot

![MyImage](./public/S2-2.A18_MemorizingGame.PNG)

## 🎮 Game Rules

- The game uses a standard **52-card deck** (spades, hearts, diamonds, clubs; each from 1 to 13).
- All cards are laid **face down** at the start of the game.
- Players can flip **two cards at a time**:
  - ✅ If the numbers match (e.g., 7♦ and 7♠), they stay face up.
  - ❌ If not, they flip back down.
- Each correct match scores **10 points**.
- The goal is to match all **26 pairs** for a total of **260 points**.

## 💡 Features

- 🔐 User **registration**, **login**, and **logout**
- 📊 Individual player score tracking using **SQLite**
- 🎲 Full game logic written in **JavaScript**
- 🧠 Real-time score and attempt counter
- 🖼️ Responsive frontend interface
- 🔄 Session handling to persist login status

## 🗂️ Project Structure

