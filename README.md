# Console Chess Game in Java 🏰♟️

**A professional console-based chess game implemented in Java.**  
Demonstrates strong object-oriented design, game logic implementation, and interactive console features.

---

## 🚀 Why This Project

This project showcases:

- **Object-Oriented Programming:** Each chess piece is a separate class implementing `isValidMove()`.  
- **Core Game Logic:** Full chess rules including castling, en passant, pawn promotion, check, and checkmate detection.  
- **Interactive Console Interface:** Move timer (30 seconds per move).  
- **Clean Code & Structure:** Designed for easy extension to GUI, AI opponent, or networked multiplayer.  

This demonstrates skills relevant for **Java development, game development, and algorithmic problem solving**.

---

## 🎯 Features

- Standard chess rules (movement, check, checkmate, stalemate)  
- Pawn promotion with choice of Queen, Rook, Bishop, or Knight  
- Castling (king-side and queen-side)  
- En passant capture  
- Move timer (30 seconds per move)  
- Move history tracking  
- Easily extendable for GUI or network play  

---

## 🏗 Project Structure

```text
src/main/java/com/example/chess/
├── ConsoleMain.java       # Entry point of the console game, handles user interaction
├── logic/
│   ├── GameLogic.java    # Core game rules, move validation, special moves
│   └── Move.java         # Representation of a move, coordinates and promotion
└── model/
    ├── Piece.java         # Abstract base class for all chess pieces
    ├── Pawn.java          # Pawn implementation, including movement and en passant
    ├── Rook.java          # Rook implementation, including castling logic
    ├── Knight.java        # Knight movement implementation
    ├── Bishop.java        # Bishop movement implementation
    ├── Queen.java         # Queen movement implementation
    └── King.java          # King movement implementation, including castling

```

---

## 🛠 Technical Details

- **Language:** Java 24 (OpenJDK, latest stable version used during development)  
- **Object-Oriented Design:**  
  - Each chess piece (Pawn, Rook, Knight, Bishop, Queen, King) is implemented as a separate class inheriting from the abstract `Piece` class.  
  - The `GameLogic` class handles all game rules, validations, special moves, and game state.  
- **Move Validation:**  
  - Each piece implements its own `isValidMove()` method.  
  - Supports standard chess movement rules, including diagonal, horizontal, vertical, and knight jumps.  
- **Special Moves:**  
  - **Castling:** King-side and Queen-side, with automatic rook movement.  
  - **En Passant:** Captures handled according to chess rules.  
  - **Pawn Promotion:** Supports promotion to Queen, Rook, Bishop, or Knight, selectable by the player.  
- **Game State Tracking:**  
  - Keeps track of current player turn (white/black).  
  - Detects **check**, **checkmate**, and **stalemate** conditions.  
  - Maintains move history for potential future features like undo/redo.  
- **Timers:**  
  - Interactive 30-second move timer implemented for console gameplay.  
- **Scalability & Extensibility:**  
  - Code structured for easy extension to GUI, AI opponent, or networked multiplayer.  
  - Clean separation of concerns between model (pieces), logic (game rules), and interface (console).  
- **Coding Standards:**  
  - Clean, readable, and maintainable code following modern Java practices.  
  - Fully uses type safety, encapsulation, and modular design.  
- **Tools & Environment:**  
  - Developed using IntelliJ IDEA (latest 2025 version)  
  - Compiled and tested with **OpenJDK 24**  
  - Cross-platform compatibility (Windows, Mac, Linux)  


---

## 💡 Potential Enhancements

- Add GUI using JavaFX or Swing  
- Add AI opponent  
- Add networked multiplayer  
- Add undo/redo move functionality  
