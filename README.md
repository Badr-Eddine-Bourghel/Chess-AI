# ♟️ Chess AI

A fully playable chess game built with Python and Pygame, featuring drag-and-drop piece movement, move validation, sound effects, and switchable board themes.

---

## 📸 Preview

> _A two-player chess game rendered with Pygame, with highlighted valid moves, hover effects, and last-move indicators._

---

## 🚀 Features

- **Drag-and-drop movement** — Click and drag pieces across the board naturally
- **Move validation** — Only legal moves are allowed for each piece
- **Turn system** — Alternates between White and Black players
- **Move highlighting** — Valid moves are shown when a piece is selected
- **Last move indicator** — The previous move is highlighted on the board
- **Hover effect** — Highlights the square under the cursor
- **Sound effects** — Different sounds for regular moves and captures
- **Theme switcher** — Cycle through board color themes with a keypress
- **Game reset** — Restart the game at any time

---

## 🛠️ Tech Stack

- **Language:** Python 3
- **Library:** [Pygame](https://www.pygame.org/)

---

## 📁 Project Structure

```
Chess-AI/
├── main.py          # Entry point — game loop and event handling
├── src/
│   ├── game.py      # Game state, rendering, and turn management
│   ├── board.py     # Board representation and move calculation
│   ├── piece.py     # Piece types and their logic
│   ├── move.py      # Move representation
│   ├── square.py    # Square representation
│   ├── dragger.py   # Drag-and-drop logic
│   └── const.py     # Constants (board size, colors, etc.)
└── assets/          # Images and sounds
```

---

## ⚙️ Installation

**1. Clone the repository**

```bash
git clone https://github.com/Badr-Eddine-Bourghel/Chess-AI.git
cd Chess-AI
```

**2. Install dependencies**

```bash
pip install pygame
```

**3. Run the game**

```bash
python main.py
```

---

## 🎮 Controls

| Action | Input |
|---|---|
| Move a piece | Click and drag |
| Switch board theme | `T` |
| Reset the game | `R` |
| Quit | Close the window |

---

## 📌 How It Works

The game loop in `main.py` handles all Pygame events:

- **Mouse down** — Detects if a piece belongs to the current player and begins dragging, calculating all valid moves for that piece.
- **Mouse motion** — Updates the dragged piece's position and highlights the hovered square.
- **Mouse up** — Validates the drop target and executes the move if legal, then switches turns.
- **Key press** — `T` cycles board themes; `R` resets the full game state.

---

## 🔮 Planned Improvements

- [ ] AI opponent using Minimax with Alpha-Beta pruning
- [ ] Check and checkmate detection
- [ ] En passant and castling support
- [ ] Move history / notation panel
- [ ] Promotion UI for pawns

---

## 👤 Author

**Badr-Eddine Bourghel**
[GitHub](https://github.com/Badr-Eddine-Bourghel)

---

## 📄 License

This project is open source. Feel free to fork and build on it!
