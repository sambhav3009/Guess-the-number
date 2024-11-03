# Number Guessing Game 🎲

This is a simple command-line-based number guessing game written in C. The program generates a random number between 1 and 100, and the user tries to guess it in as few attempts as possible. After each guess, the program provides feedback to help guide the user towards the correct number.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Requirements](#requirements)
- [How to Run the Game](#how-to-run-the-game)
- [Example Output](#example-output)
- [License](#license)

## Features

- Randomly generates a number between 1 and 100 for each game.
- Provides feedback after each guess:
  - If the guess is too high, it prompts "Lower number please!"
  - If the guess is too low, it prompts "Higher number please!"
- Counts and displays the total number of guesses made by the user once the correct number is guessed.
- Simple and beginner-friendly code.

## How It Works

1. The program uses `srand(time(0));` to seed the random number generator with the current time, ensuring that a new random number is generated each time the game is run.
2. The user is prompted to guess the number.
3. Based on the user’s input, the program provides feedback:
   - "Higher number please!" if the guess is lower than the target number.
   - "Lower number please!" if the guess is higher than the target number.
4. This process repeats until the user guesses the correct number.
5. The program then displays a congratulatory message and the total number of attempts.

## Requirements

- C Compiler (e.g., GCC)
- Basic understanding of running C code from the command line

## How to Run the Game

1. Clone the repository or download the `number_guessing_game.c` file.
2. Open a terminal, navigate to the folder containing the file, and compile the program:
   ```bash
   gcc number_guessing_game.c -o number_guessing_game
