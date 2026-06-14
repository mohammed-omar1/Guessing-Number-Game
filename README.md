# Number Guessing Game in C

A simple, lightweight command-line game written in C where the player has to guess a randomly generated number between 1 and 100.

## Features
- Generates a random number between 1 and 100 using a time-based seed.
- Provides real-time feedback (`TOO LOW!` or `TOO HIGH!`) for each guess.
- Tracks and displays the total number of attempts once you guess correctly.

## Requirements
To compile and run this game, you will need a C compiler installed (such as `gcc` or `clang`).

## Getting Started

### 1. Compile the code
Use your terminal or command prompt to run:
```bash
gcc main.c -o guessing_game
```

### 2. Run the game
- **On Linux / macOS:**
  ```bash
  ./guessing_game
  ```
- **On Windows:**
  ```cmd
  guessing_game.exe
  ```

## Gameplay Preview

```text
************************
* NUMBER GUESSING GAME *
************************
Guess a number between 1 - 100: 50
TOO HIGH!
Guess a number between 1 - 100: 25
TOO LOW!
Guess a number between 1 - 100: 37
CORRECT!
The answer is 37
It took you 3 tries
```

## How It Works
- **`srand(time(NULL))`**: Seeds the random number generator using the system clock so that the target number is different every play session.
- **`do-while` loop**: Continuously prompts for input until the user guesses the correct number.
- **`scanf` & `printf`**: Used for standard terminal input and output.

## License
This project is open source and free to use, modify, and distribute.
