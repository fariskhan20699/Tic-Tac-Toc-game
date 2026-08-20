# 🎮 Tic-Tac-Toe Game in C++

A console-based **Tic-Tac-Toe game developed in C++** using fundamental programming concepts, functions, arrays, conditional logic, loops, and input validation.

This project was built as a practical exercise to strengthen C++ programming and problem-solving skills.

---

## 📌 Project Overview

This is a two player Tic-Tac-Toe game played directly in the terminal.

Players take turns selecting positions from **1 to 9** on a 3×3 board. The game automatically:

* Displays the game board
* Accepts player input
* Validates the selected position
* Prevents players from selecting an occupied position
* Switches between players
* Checks rows, columns, and diagonals for a winner
* Detects a tie when all positions are filled

---

## ✨ Features

### 🎯 Two-Player Gameplay

Two players can play against each other on the same computer.

### ❌⭕ Marker Selection

Player 1 can choose either:

* `X`
* `O`

The other marker is automatically assigned to Player 2.

### 🧩 Dynamic Board

The board updates after every valid move.

Example:

```text
  X | O | 3
 ---|---|---
  4 | X | 6
 ---|---|---
  7 | 8 | O
```

### 🔒 Input Validation

The program checks:

* Invalid positions
* Positions outside `1–9`
* Already occupied positions
* Invalid player markers

### 🏆 Winner Detection

The program checks all possible winning combinations:

* 3 rows
* 3 columns
* Main diagonal
* Secondary diagonal

### 🤝 Tie Detection

If all nine positions are filled and neither player wins, the game declares a tie.

---

## 🛠️ Technologies Used

* **C++**
* Standard Library
* `iostream`
* 2D Arrays
* Functions
* Loops
* Conditional Statements
* Boolean Functions
* Input Validation

---

## 📂 Project Structure

```text
tic-tac-toe/
│
├── tic-tac-toc.cpp
└── README.md
```

---

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

### 2. Enter the Project Directory

```bash
cd YOUR-REPOSITORY
```

### 3. Compile the Program

Using `g++`:

```bash
g++ -std=c++17 tic-tac-toc.cpp -o tic-tac-toc
```

### 4. Run the Game

Linux/macOS:

```bash
./tic-tac-toc
```

Windows:

```bash
tic-tac-toc.exe
```

---

## 🎮 How to Play

### Step 1  Choose a Marker

When the program starts:

```text
Choose Your Marker: X or O
```

Enter either:

```text
X
```

or:

```text
O
```

### Step 2  Select a Position

The initial board looks like:

```text
  1 | 2 | 3
 ---|---|---
  4 | 5 | 6
 ---|---|---
  7 | 8 | 9
```

Enter the number corresponding to the position where you want to place your marker.

For example:

```text
Player 1 (X), enter your turn: 5
```

The board becomes:

```text
  1 | 2 | 3
---|---|---
  4 | X | 6
---|---|---
  7 | 8 | 9
```

---

## 🧠 Concepts Practiced

This project focuses on several important C++ concepts.

### Variables

```cpp
int currentPlayer;
char currentMaker;
```

### Two Dimensional Arrays

```cpp
char board[3][3];
```

The board is represented using a 3×3 character array.

### Functions

The program separates different responsibilities into functions:

```cpp
drawBoard();
marker();
winner();
swapPlayerAndMarker();
fun();
```

### Boolean Functions

The `marker()` function returns `true` when a move is successfully placed and `false` when the selected position is already occupied.

### Loops

Loops are used for:

* Board checking
* Row checking
* Column checking
* Game turns

### Conditional Statements

`if` and `else` statements are used for:

* Input validation
* Winner detection
* Player switching
* Occupied positions

---

## 🏗️ Game Logic

The main game flow is:

```text
Start Game
    ↓
Choose X or O
    ↓
Initialize Player 1
    ↓
Display Board
    ↓
Enter Position
    ↓
Validate Position
    ↓
Place Marker
    ↓
Display Updated Board
    ↓
Check Winner
    ↓
Winner?
 ┌──Yes──→ End Game
 │
 No
 ↓
Switch Player
 ↓
Repeat
 ↓
9 Valid Moves?
 ┌──No──→ Continue Game
 │
 Yes
 ↓
Tie
 ↓
End Game
```

---

## 🚀 Possible Future Improvements

The current project is intentionally kept simple. Future versions could include:

* [ ] Play Again option
* [ ] Score tracking
* [ ] Single-player mode
* [ ] Computer/AI opponent
* [ ] Difficulty levels
* [ ] Better terminal UI
* [ ] Object-Oriented Programming implementation
* [ ] Separate `.h` and `.cpp` files
* [ ] Persistent player statistics
* [ ] Improved input handling

---

## 🎓 Learning Objective

The main purpose of this project is to practice turning programming logic into a complete working application.

It demonstrates how basic C++ concepts can be combined to create an interactive console-based game.

---

## 👨‍💻 Author

**Muhammad Faris Khan**

BS Computer Science Student

---

## 📄 License

This project is available for educational and learning purposes.
