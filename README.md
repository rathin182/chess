# ChessSync — Real-Time Two-Player Chess Game

## Project Summary
ChessSync is a real-time multiplayer chess application that enables two players to play an official chess game with synchronized state, move validation, and basic chat. Built to demonstrate socket-based real-time communication, game-state consistency, and frontend-backend integration.

## Tech Stack
- Backend: Node.js, Express.js, Socket.io
- Game logic: Chess.js
- Frontend: React.js (or plain HTML/JS)
- Database: MongoDB (optional - for match history)
- Auth: Basic session / JWT (optional)

## Features
- Create/Join game room.
- Real-time move synchronization with turn enforcement.
- Move validation and check/checkmate detection via Chess.js.
- Chat during a match.
- Spectator mode (watch ongoing games).
- Reconnect support: if a player disconnects & returns, they resume the game.

## Architecture
- Clients connect to backend via Socket.io.
- Backend handles rooms (one room per match), relays validated moves to opponent, and saves match results (if DB enabled).
- Chess.js on server ensures no invalid moves are accepted.

## Setup (local)
1. Clone repo:
