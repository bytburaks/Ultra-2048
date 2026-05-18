# 2048 Puzzle Game Clone - Matrix Logic & Smooth UI Project

This repository contains a fully functional, polished clone of the famous **2048 puzzle game**, developed using **Unity** and **C#**. The project focuses heavily on 2D matrix manipulation algorithms, grid-based logic, and smooth user interface rendering to recreate the addictive, tactile feel of the original mathematical puzzle.

## 🚀 Play in Browser
You can play the web-optimized version of the game directly on your browser via GitHub Pages:
👉 **[Click Here to Play the Game](https://bytburaks.github.io/Ultra-2048/)**

---

## 🛠️ Tech Stack & Key Features

*   **Game Engine:** Unity (2D Canvas System)
*   **Language:** C# (Object-Oriented Programming, Data Structures)
*   **Data Structure:** $4 \times 4$ Two-Dimensional Array (Matrix) for board state tracking.
*   **Animations:** Scripted or Tween-based smooth tile movement and scale transitions.
*   **Persistence:** Local high-score tracking fully compatible with WebGL browsers.

---

## ⚙️ Technical Highlights (What I Implemented)

### 1. Matrix Shift & Merge Algorithm
*   Developed a robust mathematical algorithm to handle grid inputs (Up, Down, Left, Right). 
*   The script processes rows or columns using a two-step logic: compressing empty spaces (zeros) and merging adjacent elements with identical values (e.g., $2 + 2 \rightarrow 4$), preventing double-merges in a single turn.
*   Utilized conditional boundary checks to dynamically spawn a new tile (2 or 4) in a random empty cell only after a valid board-state modification.

### 2. Smooth Tile Visuals & Tweening
*   Separated the logical grid board from the visual presentation. While the backend calculations happen instantly, the frontend interpolates the positions smoothly using custom lerp functions or tween mechanics.
*   Implemented dynamic tile coloring where each cell updates its background and font styles dynamically at runtime based on its numerical value.

### 3. Game-Over & Victory Validation
*   Coded real-time state checkers that run after every move to scan for two primary conditions:
    *   **Victory:** A tile reaches the value of 2048.
    *   **Game Over:** The $4 \times 4$ matrix is completely full, and there are no valid horizontal or vertical adjacent merges remaining.

### 4. High-Score Persistence
*   Integrated a local data persistence layer using Unity's `PlayerPrefs` to cache and display the player's lifetime highest score, ensuring state recovery even after closing the browser tab.

---

## 🎮 How to Play / Controls

*   **PC:** Use the `Arrow Keys` or `WASD` to slide all tiles in the desired direction.
*   **Goal:** Merge tiles with matching numbers to double their value. Reach the **2048** tile without running out of possible moves to win!

---

## 🎮 Game Photos

<img width="313" height="611" alt="3" src="https://github.com/user-attachments/assets/98a66955-5784-4dbd-a65b-0fc7b92df352" />
<img width="312" height="602" alt="2" src="https://github.com/user-attachments/assets/03c31808-1702-409c-8987-00633862710a" />
<img width="317" height="617" alt="1" src="https://github.com/user-attachments/assets/ed9d65a7-bf7c-48b5-babf-ce4c4e731c94" />

---
