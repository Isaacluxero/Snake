# Snake Game in C

## Overview

This project implements a classic snake game in C. The game involves controlling a snake to eat fruits and grow longer while avoiding collisions with walls and itself. The game is represented on a grid, and the snake can move in four directions: up, down, left, and right.

## Project Structure

The project consists of several C files:

- `state.c`: Contains functions related to managing the game state, such as initializing the board, updating the game state, and freeing memory.
- `snake.c`: Contains the main function `main` to run the game, as well as functions to handle input/output and game logic.
- `custom_tests.c`: Contains custom unit tests to ensure the correctness of helper functions and game logic.

## Functions Implemented

### create_default_state

Created a default game state with a predefined board layout, including walls, fruits, and snakes.

### free_state

Freed all memory allocated for a given game state, including snake structs and the game board.

### print_board

Printed the game board to a specified file pointer, allowing users to visualize the game state.

### update_state

Updated the game state by moving snakes according to game rules, handling collisions, eating fruits, and growing in length.

### load_board

Read a game board from a file stream into memory, supporting reading from stdin and other streams efficiently.

### initialize_snake

Initialized snake structs based on the loaded game board, finding snake heads and tails, and setting up the game state accordingly.

### main

Filled in the missing parts of `snake.c`, including handling input/output, updating the game state, and running the game loop to simulate snake movements and interactions.

## Running the Game

To run the game, compile the code and execute the `snake` executable. Use command-line arguments to specify input and output files, or use stdin/stdout for interactive gameplay.

For example:

```bash
gcc state.c snake.c custom_tests.c -o snake
./snake -i tests/input.snk -o output.snk


