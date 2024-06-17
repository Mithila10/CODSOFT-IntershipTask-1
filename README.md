# CODSOFT-IntershipTask 1
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

 #codsoft-task 2
 #student grade calculator

 Objective: Calculates the total marks, percentage, and assigns a grade based on predefined grade ranges.

Components:

Initialization:

numberOfSubjects is set to 6, indicating the total number of subjects.
sumSubjects accumulates the total marks entered by the user.
percentage calculates the average marks across all subjects.
User Input:

Uses a for loop to prompt the user for marks in each subject using Scanner input.
Stores subject names in an array subjectNames for display purposes.
Calculations and Output:

Computes percentage as sumSubjects / numberOfSubjects.
Prints the total marks (sumSubjects) and calculated percentage.
Determines the grade based on the percentage using conditional statements:
Grades are assigned based on ranges (Failed, C, B, A++).
Closing:

Closes the Scanner object sc to free up resources after use.
Considerations:

Ensures input validation and error handling for non-integer inputs are not implemented here, assuming valid inputs for simplicity.
Uses integer division for percentage calculation (sumSubjects / numberOfSubjects), which may truncate fractional parts.

#codsoft task-3
ATM Interface

Program Overview
Purpose: The ATMInterface program simulates a basic ATM (Automated Teller Machine) interface allowing users to perform operations such as depositing money, withdrawing money, checking balance, viewing transaction history, and exiting the application.

Components:

Classes:

ATMInterface: Manages user interaction through the command-line interface (main method initializes and starts the ATM).
Account: Represents the account with methods to get and set the account balance.
Transaction: Represents individual transactions with attributes such as amount, type (deposit or withdrawal), and timestamp.
Initialization:

The ATMInterface constructor initializes an Account object (accnt) and an ArrayList to store Transaction objects (transactionHistory).
User Interaction (runATM() method):

Displays a menu (printMenu() method) with options for operations.
Uses a Scanner to capture user input for selecting menu options.
Executes operations based on user input:
1. Deposit Money (depositMoney()): Prompts for amount, updates account balance, records the transaction.
2. Withdraw Money (withdrawMoney()): Checks for sufficient funds, updates account balance if possible, records the transaction.
3. Check Balance (checkBalance()): Displays current account balance.
4. Exit: Terminates the application.
5. View Transaction History (printTransactionHistory()): Outputs a list of recorded transactions.
Transaction Handling:

recordTransaction(double amount, String type): Creates a Transaction object with the specified amount, type, and current timestamp, and adds it to transactionHistory.
printTransactionHistory(): Outputs each transaction in transactionHistory using System.err for immediate output.
Output Management:

Uses System.out.println() for standard messages and System.err.println() for transaction history to differentiate immediate output.
Resource Management:

Closes the Scanner object (sc) using sc.close() after finishing user interactions to release resources.
Key Points
Functionality: Provides essential banking operations with real-time feedback on transactions and balance inquiries.
Input Handling: Uses Scanner for user input, ensuring operations are driven by user selections.
Transaction Logging: Maintains a history of transactions with timestamps for audit and user reference.
Output Clarity: Differentiates between immediate responses (like transaction history) and regular messages using output streams (System.out and System.err).
Conclusion
This program serves as a practical demonstration of implementing a simple ATM system in Java, focusing on user interaction, data management, and basic transaction handling. It showcases fundamental concepts of object-oriented programming, input/output handling, and effective use of collections for storing transaction data.




