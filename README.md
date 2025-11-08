# Minesweeper

A Python-based Minesweeper game with GUI built using Tkinter, featuring an AI solver that can automatically play the game using logical inference.

## About

This is a classic Minesweeper implementation with a graphical interface that includes:
- Traditional Minesweeper gameplay with left-click to reveal cells and right-click to flag mines
- Visual feedback with images for different cell states (0-8 neighboring mines, flags, mines)
- A hint system to reveal safe cells
- An AI player that uses logical reasoning to solve the game automatically

The AI uses a knowledge-based approach with sentence inference to deduce safe moves and identify mines based on revealed cell information.

## Features

- **Interactive GUI**: Clean interface with image-based cells
- **Hint System**: Get hints for safe cells when stuck
- **AI Solver**: Watch the AI solve the puzzle using logical inference
- **Configurable Settings**: Customize grid size, mine count, and board dimensions

## Project Structure

- `main.py` - Entry point and GUI initialization
- `cell.py` - Cell class managing individual cell behavior and game logic
- `computer.py` - AI implementation with knowledge-based reasoning
- `settings.py` - Game configuration (grid size, dimensions, images)
- `utilities.py` - Helper functions for calculations
- `images/` - Visual assets for the game

## Setup

### Prerequisites

- Python 3.10+ (uses match-case statements)
- Tkinter (usually comes with Python)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/Iongshiba/minesweeper.git
cd minesweeper
```

2. Ensure you have Python installed with Tkinter support:
```bash
python --version
```

## How to Run

Run the game using:
```bash
python main.py
```

## How to Play

- **Left Click**: Reveal a cell
- **Right Click**: Flag/unflag a cell as a potential mine
- **Hint Button**: Highlights a safe cell to help you progress
- **AI Move Button**: Toggle AI mode to watch the computer solve the game

## Game Controls

The game window displays:
- Cells remaining counter
- Mines remaining counter
- Hint button for assistance
- AI move toggle button

## AI Implementation

The AI uses a knowledge-based system that:
1. Maintains sets of known safe cells and mines
2. Creates logical sentences about unknown cells based on revealed information
3. Performs inference to deduce new safe cells and mines
4. Makes moves based on safe deductions or calculated risks
