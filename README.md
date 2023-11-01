# Snake-game-AI
Snake Game by implementing the A* Algorithm shown on replit


This code is an implementation of the classic Snake game using the Pygame library in Python. It defines the game mechanics and graphics for a Snake game and also includes an AI component for controlling the snake.

Here's a breakdown of the code's structure and key components:

Importing Libraries:

pygame: Pygame is a popular library for creating 2D games in Python.
sys: Provides access to some variables used or maintained by the interpreter and to functions that interact with the interpreter.
random: Used for generating random numbers.
from pygame.locals import *: Imports constants that are commonly used in Pygame.
Colors: Various color constants are defined, which will be used to draw different elements of the game.

Game Constants:

FPS: Sets the frames per second for the game.
WINDOW_WIDTH and WINDOW_HEIGHT: Define the dimensions of the game window.
SCREEN_SIZE: The size of the game screen.
GRID_SIZE: The size of the grid used for the game board.
GRID_WIDTH and GRID_HEIGHT: Calculate the number of grid cells in the width and height.
MARGIN and TOP_MARGIN: Define margins for the game layout.
Snake Class:

The Snake class defines the behavior and attributes of the snake.
create(): Initializes the snake with a length of 2 and a random starting direction.
control(direction): Allows changing the snake's direction based on user input.
move(): Moves the snake in the current direction.
draw(): Draws the snake on the game screen.
eat(): Handles when the snake eats food, increasing its length.
Feed Class:

The Feed class defines the behavior and attributes of the snake's food.
create(): Generates random coordinates for the food.
draw(): Draws the food on the game screen.
Main Function:

The main() function initializes the game, creates the game window, and enters the game loop.
runGame Function:

runGame(snake, feed): Manages the game loop.
Handles user input for controlling the snake.
Calls the AI component to make decisions for the snake's movement.
Checks for collisions and updates the game display.
execEvent Function:

Maps keyboard events to snake movement directions.
terminate Function:

Exits the game.
Rendering Functions:

renderRect, drawRect, and makeText functions are used for drawing various elements on the screen.
showTitle Function:
Displays the game title.
showGameInfo Function:
Displays the score.
drawGrid Function:
Draws a grid on the game board.
gameOver Function:
Displays a game-over message when the game ends.
Main Execution:
The game is started by calling main() when the script is run.
To edit the values and change how the game looks during outputs, you can modify the constants and functions within the code. For example, you can change the colors, the game window dimensions, the font used for text, or the appearance of game elements. You can also customize the game mechanics, such as the snake's initial length, the game speed (FPS), and how the AI controls the snake's movement. Experimenting with these parameters will allow you to customize the game to your preferences and desired gameplay experience.
