# Tetris Game with Junk Mechanics

## Overview
This project is a custom implementation of Tetris, designed as a multiplayer-ready game with innovative mechanics to enhance strategic depth and user engagement. The game features a **junk inventory system**, **AI opponent**, and **responsive controls** tailored for both desktop and mobile devices.

---

## Game Mechanics

### 1. **Core Gameplay**
The game operates on the traditional Tetris rules:
- Tetrominoes fall from the top of the grid and can be moved left, right, or downward.
- The goal is to complete full horizontal lines to clear them from the grid.
- The game ends when tetrominoes stack up and exceed the grid's height.

### 2. **Junk Inventory System**
- **Accumulating Junk**:
  - Each cleared line contributes to the player's **junk inventory**.
  - For every cleared line, the junk inventory counter increments by 1.
- **Using Junk**:
  - Players can choose to use stored junk to remove an equivalent number of lines from the **bottom of their grid**.
  - Junk usage can be strategic to lower the grid height and avoid losing.
- **Sending Junk to Opponents**:
  - In multiplayer mode, players can send their junk to opponents, adding "junk lines" to the bottom of the opponent’s grid.
  - Junk lines are unique—they can only be cleared by completing rows above them.

### 3. **AI Opponent**
The game includes an AI opponent with:
- **Alpha-Beta Pruning**: Evaluates moves to maximize survival and apply strategic junk usage.
- **Dynamic Strategy**:
  - Aggressive when the player’s grid is high.
  - Defensive when its own grid is at risk.

### 4. **Mobile Responsiveness**
- **Touch Gestures**:
  - Swipe left or right to move tetrominoes horizontally.
  - Swipe down to speed up the tetromino’s descent.
  - Tap to rotate the tetromino.

---

## Controls

### **Desktop**
- **Arrow Keys**:
  - &larr;: Move tetromino left.
  - Right: Move tetromino right.
  - Down: Speed up tetromino descent.
  - Up: Rotate tetromino.
- **`J` Key**: Use junk locally to remove lines from the bottom of the grid.

### **Mobile**
- **Swipe Left/Right**: Move tetromino horizontally.
- **Swipe Down**: Speed up tetromino descent.
- **Tap**: Rotate tetromino.

---

## Technical Details

### Technologies Used
- **Frontend**: HTML, CSS, and JavaScript (no frameworks).
- **Game Logic**: 
  - DOM manipulation for grid updates.
  - Alpha-Beta Pruning for AI decision-making.
  - Touch event handling for mobile gestures.
- **Responsive Design**: Ensures compatibility with both desktop and mobile devices.

### Key Features
- **Real-Time Gameplay**:
  - Smooth tetromino movements and animations.
- **Custom Junk Mechanics**:
  - Innovative system for offensive and defensive play in multiplayer.
- **AI Opponent**:
  - Intelligent decision-making for a challenging single-player experience.

---

## How to Play

1. Clone the repository:
   ```bash
   git clone https://github.com/ffaustin17/tetris-game
   ```
2. Open the `index.html` file in your browser.
3. Use the controls described above to play.

---

## Future Enhancements
- **Multiplayer Mode**:
  - Real-time interaction between two players over a network.
- **Scoring System**:
  - Points awarded based on lines cleared and junk sent to opponents.
- **Power-Ups**:
  - Add temporary advantages, such as faster junk clearance or bonus points.

---

## Credits
Created by [Fabrice Faustin].

---

## License
This project is licensed under the MIT License. See `LICENSE` for details.
