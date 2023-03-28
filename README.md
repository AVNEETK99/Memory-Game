# Memory-Game

Memory game is a popular game that requires players to match pairs of cards with identical images or symbols. The objective of the game is to turn over two matching cards at a time, with the goal of matching all pairs in the least amount of time and number of moves. The game is usually played with a deck of cards arranged in a grid, and players take turns flipping over two cards at a time, trying to remember where each card is located on the grid. The game is often used as a fun way to exercise memory and cognitive skills, and is enjoyed by both children and adults.

## Instructions to run the game

* Open the Github repository where the game code is hosted.

* Click on the green "Code" button and then select "Download ZIP" to download the code as a ZIP file.

* Extract the ZIP file to a folder on your computer.

* Open a command prompt or terminal window and navigate to the folder where you extracted the code.

* Type ```python memory.py``` and press Enter to start the game.

* Follow the prompts to play the game.

## Functionality of the code

* The code imports the ```"random"``` and ```"turtle"``` modules.

* A ```"Screen"``` object is created, which creates a new window for the game.

* The background color of the window is set to black.

* A function named ```"Square"``` is defined that takes two arguments, x and y, which are the coordinates of the square. This function draws a square at the given coordinates with a white border and a purple fill.

* A function named ```"Numbering"``` is defined that takes two arguments, x and y, which are the coordinates of a square. This function returns the index of the square in the list of tiles.

* A function named ```"Coordinates"``` is defined that takes an argument, count, which is the index of a square. This function returns the coordinates of the square on the screen.

* A function named ```"click"``` is defined that takes two arguments, x and y, which are the coordinates of a mouse click. This function checks if the clicked square is the same as the previously clicked square, and if they are a match, it reveals the tiles. If they are not a match, the clicked square becomes the new mark.

* A function named ```"draw"``` is defined that updates the screen with the current state of the game. This function clears the screen, draws the tiles, and reveals any matching tiles. It then updates the screen and sets a timer to call itself again in 10 milliseconds.

* A list named ```"tiles"``` is created, which contains the numbers 0 to 31 twice, representing the pairs of matching tiles.

* A dictionary named ```"state"``` is created with an initial value of {'mark': None}. This dictionary keeps track of the currently marked tile.

* A list named ```"hide"``` is created with an initial value of [True] * 64. This list keeps track of which tiles are hidden and which are revealed.

* The tiles in the ```"tiles"``` list are shuffled randomly.

* The turtle's animation speed is turned off.

* A mouse click event listener is registered, which calls the ```"click"``` function when the mouse is clicked.

* The ```"draw"``` function is called to start the game.

* The ```"done"``` function is called, which prevents the window from closing.
