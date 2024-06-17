# CODSOFT-IntershipTask-1
NAME: MITHILA R
DOMAIN: JAVA PROGRAMMING
ID: CS11WX246615
DURATION: 20 MAY 2024-20 JUNE 2024

OVERVIEW:
This Java program implements a number guessing game where the user has 5 chances to guess a 
randomly generated number between 1 and 100. It uses `Scanner` for user input and handles `InputMismatchException` 
to ensure only integers are accepted. 
After each game, it prompts the user to play again and displays the score upon completion.

Objective: This Java program implements a number guessing game where the user tries to guess a randomly generated number between 1 and 100 within a limited number of attempts.

Main Components:

Initialization:

1.Initializes a Scanner object sc for user input.
2.Sets chances to 5, which represents the number of attempts allowed per game.
2.Initializes end to track the number of successful guesses and playagain to control game replay.

Game Loop (while (playagain)):

1.Generates a random number (rand) using getrandN(1, 100).
2.Allows the user to guess the number in a loop (for loop iterating chances times).
Compares the user's input (user) with rand:
3.If correct, increments end, displays a success message, and breaks out of the loop.
4.If too high or too low, provides appropriate feedback.
End of Game:

If the user exhausts all chances without guessing correctly, informs them of the correct number (rand).
Asks the user if they want to play again (playagain based on user input).
Helper Methods:

getrandN(int min, int max): Generates a random integer within the specified range (min to max).
getInput(Scanner sc): Ensures the user input is an integer, handling InputMismatchException by prompting the user to enter a valid integer.

Conclusion:

Once the user decides not to play again, the program outputs a closing message and displays the number of successful guesses (end).



