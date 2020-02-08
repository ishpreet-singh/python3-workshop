
# A real world Problem

## Design a Tic tac Toe

<pre>
          |   |
        X | O | X
          |   |
        -----------
          |   |
        O | X | O
          |   |
        -----------
          |   |
        X | O | X
          |   |
</pre>

Below is a set of steps for you to follow to try to create the Tic Tac Toe Milestone Project game!


Some suggested tools before you get started:
To take input from a user:

```
player1 = input("Please pick a marker 'X' or 'O'")
```

Note that `input()` takes in a string. If you need an integer value, use

```
position = int(input('Please enter a number'))
```


> **Step 1:** Write a function that can print out a board. Set up your board as a list, where each index 1-9 corresponds with a number on a number pad, so you get a 3 by 3 board representation.

```
from IPython.display import clear_output

def display_board(board):
    
    pass



```

TEST Step 1: run your function on a test version of the board list, and make adjustments as necessary

```
test_board = ['#','X','O','X','O','X','O','X','O','X']
display_board(test_board)
```

> **Step 2:** Write a function that can take in a player input and assign their marker as 'X' or 'O'. Think about using while loops to continually ask until you get a correct answer.

```
def player_input():
    
    pass
```

TEST Step 2: run the function to make sure it returns the desired output


```
player_input()
```


> **Step 3:** Write a function that takes in the board list object, a marker ('X' or 'O'), and a desired position (number 1-9) and assigns it to the board.

```
def place_marker(board, marker, position):
    
    pass
```

TEST Step 3: run the place marker function using test parameters and display the modified board

```
place_marker(test_board,'$',8)
display_board(test_board)
```

> Step 4: Write a function that takes in a board and a mark (X or O) and then checks to see if that mark has won.

```
def win_check(board, mark):
    
    pass
```

TEST Step 4: run the win_check function against our test_board - it should return True

```
win_check(test_board,'X')
```

> Step 5: Write a function that uses the random module to randomly decide which player goes first. You may want to lookup random.randint() Return a string of which player went first.

```
import random

def choose_first():
    pass
```

> Step 6: Write a function that returns a boolean indicating whether a space on the board is freely available.

```
def space_check(board, position):
    
    pass
```

> Step 7: Write a function that checks if the board is full and returns a boolean value. True if full, False otherwise.

```
def full_board_check(board):
    
    pass
```

> Step 8: Write a function that asks for a player's next position (as a number 1-9) and then uses the function from step 6 to check if it's a free position. If it is, then return the position for later use.

```
def player_choice(board):
    
    pass
```

> Step 9: Write a function that asks the player if they want to play again and returns a boolean True if they do want to play again.

```
def replay():
    
    pass
```

> Step 10: Here comes the hard part! Use while loops and the functions you've made to run the game!


```
print('Welcome to Tic Tac Toe!')

#while True:
    # Set the game up here
    #pass

    #while game_on:
        #Player 1 Turn
        
        
        # Player2's turn.
            
            #pass

    #if not replay():
        #break
```


# Thank You