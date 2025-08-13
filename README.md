# TicTacToe (SwiftUI)

A polished TicTacToe game for iOS, built entirely with SwiftUI.  
Features real-time **win/draw detection**, a **restart function**, and a clean, responsive interface.

---

## Screenshots

<p align="center">
  <img src="./images/main_screenshot.png" alt="Playing" width="250">
  <img src="./images/main_screenshot2.png" alt="Win" width="250">
  <img src="./images/main_screenshot3.png" alt="Draw" width="250">
</p>

---

## Features
* **Two-Player Local Play** – Alternate turns between X and O on the same device.
* **Win Detection** – Automatically detects wins in rows, columns, and diagonals.
* **Draw Detection** – Identifies stalemates when the board is full.
* **Restart Button** – Reset the game instantly without relaunching.
* **Clean UI Design** – Simple, intuitive, and responsive layout.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/seahpark247/TicTacToe.git
   cd TicTacToe
2. Open the project in Xcode:
   ```bash
   open TicTacToe.xcodeproj
3. Build and run the application on your device or simulator. 

## How to Run
1. Open the project in **Xcode 15** or newer.
2. Select an iOS Simulator (e.g., iPhone 15).
3. Launch the app.
4. Tap any empty cell to place your mark (X or O).
5. The game alternates turns automatically.
6. The status text will display:
* "X wins!" or "O wins!" when a player wins.
* "Draw!" if the board is full with no winner.
* "Playing..." during active play.
7. Tap Restart to reset the board at any time.

## How to Capture Screenshots

### 1) Playing — `playing.png`
Play until both **X** and **O** are visible, then take a screenshot.

### 2) Win — `win.png`
Quick win for **X**:
1. (0,0) → X  
2. (1,0) → O  
3. (0,1) → X  
4. (1,1) → O  
5. (0,2) → X ✅ *X wins (top row)*

### 3) Draw — `draw.png`
Fill the board without a winner:
1. (0,0) X  
2. (1,1) O  
3. (0,1) X  
4. (0,2) O  
5. (2,0) X  
6. (1,0) O  
7. (1,2) X  
8. (2,1) O  
9. (2,2) X ✅ *Draw*

> Use the **Restart** button to reset the board anytime.

## Technologies
* Swift – Core development language.
* SwiftUI – Declarative UI framework.
* State Management – @State for board tracking and turn handling.
* Custom View Modifiers – For reusable styles on cells, buttons, and status text.

## Code Overview
The game logic is handled in `ContentView.swift`:
- `board: [[Player]]` — current state of the game board
- `currentPlayer` — active player
- `makeMove(row:col:)` — handles moves and turn switching
- `checkWinner(player:)` — determines the winner
- `isDraw()` — checks for a draw
- `resetBoard()` — resets the game state

### UI Modifiers
- **Cell** — style for game board cells
- **RestartButton** — style for the restart button
- **StatusText** — style for the game status label

## License
MIT License — free to use, modify, and share.
