---
title: "Ultimate Tic-Tac-Toe AI Game"
excerpt: "Two projects with two different decision-making algorithms for an advanced AI-driven version of Tic-Tac-Toe.<br/>"
collection: portfolio
---

The Ultimate Tic-Tac-Toe AI Game is a sophisticated and challenging twist on the classic Tic-Tac-Toe game. This project involves the development of both the game logic and the user interface, creating an engaging experience for players.

## Features

- **Alpha-Beta Pruning**:
  - Implemented using the Raylib library, Alpha-Beta Pruning helps the AI player make optimized decisions by efficiently pruning the search tree, reducing the number of nodes evaluated and thereby speeding up the decision-making process.
  - The algorithm ensures that the AI player is both competitive and quick, providing a challenging opponent for human players.

- **Monte Carlo Tree Search (MCTS)**:
  - Integrated using the Pygame library, MCTS is employed to enhance the AI strategy in complex game scenarios.
  - This algorithm allows the AI to make informed decisions by simulating numerous possible game outcomes and selecting the move that leads to the most favorable results.
  - MCTS is particularly effective in handling the larger search space of Ultimate Tic-Tac-Toe, making the AI robust and adaptable.

## Implementation Details

1. **Alpha-Beta Pruning Using C++**:
   - Developed with the Raylib library, the game interface provides a smooth and interactive experience.
   - The Alpha-Beta Pruning algorithm significantly reduces the computation time by eliminating branches in the search tree that do not need to be explored, allowing the AI to perform efficiently even under time constraints.

2. **Monte Carlo Tree Search Using Python**:
   - Utilizing the Pygame library, the user interface is designed to be intuitive and user-friendly.
   - MCTS enhances the AI's strategic depth by evaluating multiple potential moves through random simulations, improving the quality of the AI's decisions over time.

## Screenshots

**Alpha-Beta pruning game:**
<br/>
<img src='https://orgonah.github.io/YasinDanesh.github.io/images/Alpha-Beta.png' alt='Alpha-Beta Image' style="margin-bottom:15px; width: 70%">
<br/>
<br/>
<br/>
**MCTS game:**
<br/>
<img src='https://orgonah.github.io/YasinDanesh.github.io/images/MCTS.png' alt='MCTS Image' style="margin-bottom:15px; width: 70%">
<br/>

## Conclusion

The Ultimate Tic-Tac-Toe AI Game project showcases the integration of advanced AI techniques to create a challenging and enjoyable game. By Utilizing Alpha-Beta Pruning and Monte Carlo Tree Search, the AI is capable of making sophisticated decisions, providing a robust opponent for players.

## Code

The complete code for this project is available on [this repository](https://github.com/Orgonah/Ultimate_Tic_tac_toe_AI)
Feel free to explore the repositories to understand the implementation details and contribute to the project.
