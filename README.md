# Mastermind Game

## Description

This is a console-based implementation of the classic Mastermind game, written in Python. The objective of the game is to guess a secret code consisting of a sequence of colors within a limited number of tries.

## Features

- Randomly generates a secret code from a predefined set of colors.
- Allows the user to input guesses and provides feedback on correct and incorrect positions.
- Limited number of attempts to guess the correct code.
- Simple and interactive console interface.

## Requirements

- Python 3.7 or higher

## Installation

1. Clone the repository or download the source code.

    ```sh
    git clone https://github.com/yourusername/mastermind-game.git
    ```

2. Navigate to the project directory.

    ```sh
    cd mastermind-game
    ```

## Usage

1. Run the game:

    ```sh
    python mastermind.py
    ```

2. Follow the on-screen instructions to play the game.

### Example

```sh
$ python mastermind.py
Welcome to the mastermind, you have 10 tries to guess the code.
The valid colors are R G B Y W O
Good luck!

Guess: R G B Y
Correct Positions: 1 | Incorrect Positions: 2

Guess: B W O R
Correct Positions: 0 | Incorrect Positions: 3

...

You guessed the code in 7 tries!
```

## Code Overview

### Constants

COLORS: List of valid colors (["R", "G", "B", "Y", "W", "O"]).
TRIES: Number of attempts allowed (10).
CODE_LENGTH: Length of the secret code (4).

### Functions

generate_code: Generates a random secret code from the list of colors.
guess_code: Prompts the user to enter a guess and validates the input.
check_code: Compares the user's guess to the secret code and returns the number of correct and incorrect positions.
game: Main game loop that manages the gameplay.


### Main Workflow

The game starts by displaying a welcome message and the valid colors.
The secret code is generated randomly.
The user is prompted to enter guesses.
After each guess, the game provides feedback on the number of correct and incorrect positions.
The game ends when the user guesses the code correctly or runs out of attempts.
Customization

You can change the number of attempts by modifying the TRIES constant.
You can adjust the length of the code by changing the CODE_LENGTH constant.
You can add or remove colors by updating the COLORS list.


## Contributing

Feel free to submit issues or pull requests if you find bugs or have improvements.
