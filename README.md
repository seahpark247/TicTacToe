# TicTacToe (SwiftUI)

A polished TicTacToe game for iOS, built entirely with **SwiftUI**.  
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
3. Build and run on an iOS Simulator or device (Xcode 15+ recommended).

## How to Play
1. Tap any empty cell to place your mark (X or O).
2. Turns alternate automatically.
3. Status text displays:
* "X wins!" or "O wins!" → Game over with a winner.
* "Draw!" → Board is full, no winner.
* "Playing..." → Game in progress.
4. Tap Restart to reset the board anytime.

## Technologies
* **Swift** – Core development language
* **SwiftUI** – Declarative UI framework
* **@State** - For managing game state
* **Custom View Modifiers** – For reusable styling

## License
MIT License — free to use, modify, and share.
