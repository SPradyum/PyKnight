# ♟️ PyKnight – A Python Chess Engine with Minimax & Alpha-Beta Pruning  

PyKnight is a clean and extensible chess engine written in Python.  
This is a simple chess engine/interface created using Flask.
It utilizes chessboard.js and chess.js for the frontend chessboard logic, and Python chess for the backend chessboard logic. 
- All calculations are done on the backend using Python.

It uses the `python-chess` library along with classical AI techniques, including:
- ✅ Minimax search  
- ✅ Alpha-Beta pruning  
- ✅ Iterative deepening  
- ✅ Move ordering  
- ✅ Piece-Square tables  
- ✅ Material & positional evaluation  

This engine is perfect for hobbyists, students, and researchers who want to understand how chess engines work or build their own GUI/AI on top of it.

---

## 🚀 Features

### ✅ **1. Minimax Search**
Classic recursive minimax algorithm for computing optimal moves.

### ✅ **2. Alpha-Beta Pruning**
Improves search efficiency dramatically by pruning unnecessary branches.

### ✅ **3. Iterative Deepening**
Depth-by-depth search that returns the best move found at every stage.

### ✅ **4. Board Evaluation**
The engine uses:
- Material scoring  
- Piece-square tables for positional strength  
- Checkmate/stalemate detection  

### ✅ **5. Move Ordering**
Sorts moves to help Alpha-Beta pruning work more efficiently.

### ✅ **6. FEN Support**
Initialize any game state instantly using a FEN string.

---
## Pip Install
```bash
Install flask by running:
    pip install flask

Install python chess by running:
    pip install python-chess[uci,gaviota]
```
---

## 🧠 Evaluation Strategy

PyKnight calculates a score based on:

- **Material values** (pawn=100, knight=300, bishop=310, rook=500, queen=900, king extremely high)
- **Piece-square tables** to reward strong squares  
- **Side-to-move advantage**  
- **Checkmate detection**

---

## 🏎️ Performance Notes

The engine supports:
- Deep search (up to 60 ply)
- Move ordering for improved pruning
- Iterative deepening for stable best-move returns
- Debug output for:
- Nodes searched
- Time taken
- Best lines

## 🤝 Contributing
Contributions are welcome!
Open an issue or submit a PR if you want to improve the engine.
