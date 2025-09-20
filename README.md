# PyQt6 Chess Trainer

## Description
A lightweight chess training application built with **PyQt6** and **python-chess**. After each move you play (White or Black), the system immediately suggests the best move for the side to move (your opponent), using the Stockfish engine. You stay in full control: the engine never plays for you. It only highlights its recommended reply.

Main features:
- Play manually as White or Black
- See engine's best reply immediately after your move
- Highlight of your last move (blue) and the engine’s suggested reply (red)
- Configurable engine time per move

---

## Stockfish

### What is it?
**Stockfish** is one of the strongest open-source chess engines available.  
It evaluates positions and suggests the best moves using the Universal Chess Interface (UCI) protocol.  
This app runs Stockfish **locally**, so it works offline and without latency.

### Installation

- **macOS (Homebrew):**
  ```bash
  brew install stockfish
  ```

- **Linux (Debian/Ubuntu):**
  ```bash
  sudo apt-get update
  sudo apt-get install stockfish
  ```

- **Windows:**
  Download a prebuilt binary from the [official Stockfish site](https://stockfishchess.org/download/)  
  Set the path.

---

## Installation

   ```bash 
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt
   ```

---

## Usage

1. Start the app:
   ```bash
   python3 main.py
   ```

2. Play any move (as White or Black).  
   The system will highlight and display the best reply for the opponent.

3. Use controls on the right:
   - **New game**: reset to starting position
   - **Undo**: revert your last move
   - **Rotate board**: flip orientation
   - **Engine time (ms)**: adjust engine’s thinking time per move