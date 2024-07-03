# Flappy Bird Clone

This is a simple Flappy Bird clone created using Python and the Tkinter library. The game features basic gameplay mechanics such as jumping, pipe obstacles, scoring, and a high score system.

## Features

- **Bird Jumping**: Press the spacebar to make the bird jump.
- **Pipe Obstacles**: Pipes move from right to left, and the bird must avoid them.
- **Scoring System**: Earn points by passing through the pipes.
- **High Score**: The highest score is saved and displayed.
- **Game Over**: The game ends when the bird collides with a pipe.

## Prerequisites

- Python 3.x
- Tkinter library (usually comes pre-installed with Python)

## How to Run

1. Clone this repository:
   

2. Run the game:
    ```bash
    python flappy.py
    ```

## Controls

- **Spacebar**: Makes the bird jump.

## Code Explanation

### `FlappyBird` Class

- **Attributes**:
  - `canvas`: The main canvas where the game is rendered.
  - `bird`: The bird represented as a yellow rectangle.
  - `pipe_upper` and `pipe_lower`: The pipes represented as green rectangles.
  - `score_label`: Displays the current score.
  - `high_score_label`: Displays the high score.
  - `start_button`: Button to start the game.
  - `new_game_button`: Button to start a new game.
  - `y`: The vertical speed of the bird.
  - `score`: The current score.
  - `high_score`: The highest score achieved.
  - `game_over`: Boolean flag indicating if the game is over.
  - `game_over_text`: Reference to the game over text object.

- **Methods**:
  - `__init__`: Initializes the game.
  - `start_game`: Starts the game and initializes the game loop.
  - `new_game`: Resets the game to its initial state.
  - `move`: Handles the movement of the bird and pipes.
  - `jump`: Makes the bird jump.
  - `check_collision`: Checks for collisions between the bird and pipes.
  - `save_high_score`: Saves the high score to a file.
  - `get_high_score`: Retrieves the high score from a file.

### `main` Function

- Initializes the Tkinter root window and starts the game.

## File Structure

- `flappy_bird.py`: The main game script.
- `high_score.txt`: File used to store the high score.
