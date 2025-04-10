# Monopoly_Game
# 🎲 Monopoly Game Simulation

This project is a simulation of the classic Monopoly board game, built using object-oriented programming and a relational database design. It supports multiple players, real-time game sessions, and a complete property management system. Developed as a comprehensive academic project, it showcases both software and database design principles.

---

## 📦 Project Overview

- **Language:** Python  
- **Database:** SQLite3  
- **Design Focus:** Object-Oriented Architecture + Relational Data Modeling

---

## 🧩 Features

- Host multiple active game sessions simultaneously
- Track player turns, balances, and owned properties
- Manage standard properties and special board spaces
- Abstracted database interaction for clean, modular code
- Easily extendable rules and game logic

---

## 🧱 Database Structure

The project uses four main tables:

- `game_session`: Tracks each game's ID and configuration
- `players`: Stores player details and links them to game sessions
- `properties`: Contains data for buyable board properties
- `non_property_spaces`: Handles other board tiles like Jail or Chance

Relational integrity is enforced using foreign keys such as `game_id` and `owner_id`.

---

## 🧠 Software Architecture

- `Game`: Main controller for game logic and turn sequencing
- `Player`: Handles individual player data and moves
- `Property`: Manages buyable spaces
- `NonProperty`: Covers spaces like "Go to Jail" or "Free Parking"

Each class is responsible for interacting with its own database records. The codebase is structured to separate logic from persistence, allowing easy updates or upgrades.

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/monopoly-game-simulation.git
   cd monopoly-game-simulation
