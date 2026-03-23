# 3-Symbol Tic Tac Toe: Game Design & Implementation

## Abstract

This project presents an advanced variant of Tic Tac Toe, expanded from the traditional 3×3 grid to a 5×5 playing field with a three-symbol system. The human player controls the symbol **X** and plays first, while the system intelligently alternates between symbols **O** and **Z** across consecutive turns.

### Game Overview

**Objective:** Align three of your symbols (X) in a row—horizontally, vertically, or diagonally—before the system completes a similar alignment with either O or Z.

**Board Size:** 5×5 grid (25 cells)

**Symbols:**
- **X** (Blue) - Human Player
- **O** (Purple) - System AI #1
- **Z** (Orange) - System AI #2

**Turn Sequence:** X → O → Z → X → O → Z → ...

### Innovation & Design Rationale

#### Problem Statement
Traditional 3×3 Tic Tac Toe, when played optimally, always results in a draw. This reduces strategic depth and makes the game unwinnable for the human player against intelligent AI. The expanded 5×5 grid with three symbols fundamentally changes the game dynamics:

1. **Increased Strategic Complexity** - More possible winning combinations (40+) create diverse strategic paths
2. **Balanced Difficulty** - The expanded board provides enough space for both offense and defense
3. **Winnable Gameplay** - Players have realistic opportunities to defeat the system while maintaining challenge
4. **Dual AI Opposition** - The system's control of two alternating symbols adds layer of complexity

#### Technical Implementation

**AI Algorithm:** Minimax with Alpha-Beta Pruning
- Evaluates all possible game states within depth limits
- Makes strategically optimal decisions for both O and Z
- Balances computational efficiency with decision quality
- Depth limiting prevents exponential time complexity on larger board

**Win Detection:** Dynamic combination generation
- Generates all 40 possible three-in-a-row combinations algorithmically
- Horizontal: 15 combinations (5 rows × 3 starting positions)
- Vertical: 15 combinations (5 columns × 3 starting positions)
- Diagonal: 10 combinations (2 directions × 5 starting positions)

**User Interface:** Progressive multi-page design
1. **Instructions Page** - Game rules, symbols, and strategy tips
2. **Game Page** - Interactive 5×5 board with real-time feedback
3. **Results Page** - Outcome display with winning combo highlight

### Key Features

✅ **Responsive Design** - Adapts to desktop, tablet, and mobile screens  
✅ **Real-Time Feedback** - Turn indicators and game status updates  
✅ **Intelligent AI** - Strategic play from both system symbols  
✅ **Complete Win Detection** - All 40 winning combinations checked  
✅ **Beautiful UI** - Modern gradient design with smooth animations  
✅ **Accessible** - Clear instructions and color-coded symbols  

### Winning Conditions

- **Player Wins:** Three X's in a row (any direction)
- **System Wins:** Three O's OR three Z's in a row (either symbol can win)
- **Draw:** 25 moves completed with no winner

### Strategic Depth

The game requires players to:
- Balance offensive and defensive strategies
- Think multiple moves ahead
- Navigate dual AI threats
- Utilize the 5×5 space strategically
- Control key positions (center, corners, edges)

### Conclusions

By expanding the traditional Tic Tac Toe to a 5×5 grid with three symbols and introducing dual AI opponents, we create a game that maintains strategic depth while remaining winnable for skilled players. This design successfully bridges the gap between the deterministic 3×3 version and completely open-ended game design, demonstrating how fundamental rule changes can transform a simple game into an engaging challenge.

---

## Files Included

- **tictactoe_3symbols_5x5.html** - Complete game implementation (single HTML file)
- **ABSTRACT.md** - Design documentation and game analysis
- **README.md** - Setup and usage instructions

## Author

Created: 2026-03-23

## License

MIT License - Free to use and modify