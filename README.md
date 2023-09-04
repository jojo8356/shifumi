# shifumi

1. First, the code starts by importing the randint function from the random module, which will generate a random number for the computer's choice in the Rock, Paper, Scissors game.

2. Then, a BDD dictionary (database) is created to store the game elements. This dictionary contains three lists:

3. "element": contains the three elements of the game (rock, paper, scissors).
"winner": contains character strings representing the winning combinations of the game. Each combination is represented by two numbers, where the first number corresponds to the computer's choice and the second number to the player's choice.
"sentence": contains sentences describing the result of each combination.
Then the code enters a while True loop, which means it will continue to execute until an exit condition is satisfied.

4. Inside the loop, the user is prompted to enter their choice by typing "rock", "paper" or "scissors". The user input is stored in the player variable.

5. The code checks if the user's (player) choice is present in the list of elements (BDD["element"]). If so, that means the user's input is valid.

6. Then the code generates a random choice for the computer using randint(0, 2), which results in a random number between 0 and 2 inclusive. The choice of computer is stored in the choice variable.

7. The chosen values ​​and player are then used to determine the outcome of the game. If choice is different from player, it means there is a winner, and the loop ends with break. Otherwise, the game is declared a "tie" and the message "Tie, start again..." is displayed.

8. If the user's (player's) choice is not present in the list of items, the code displays "Typo!" to indicate an entry error.

9. Once the loop is complete, the code calculates the final outcome of the game using the choice and player indices to access the lists BDD["winner"] and BDD["sentence"]. If the combination f"{choice}{player}" is present in the list BDD["winner"], then the player has won, otherwise he has lost. The final message describing the result is displayed, depending on the result.
