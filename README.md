# Rock Paper Scissors x99

### Index

- [Rock Paper Scissors x99](#rock-paper-scissors-x99)
    - [Index](#index)
  - [Project Overview](#project-overview)
  - [Significant Code Highlights](#significant-code-highlights)
    - [Scope](#scope)
    - [Naming](#naming)
    - [Functions](#functions)
  - [Tip(s) for use](#tips-for-use)
  - [Testing](#testing)

## Project Overview

Built all of the logic needed for a more intense version of Rock Paper Scissors (RPS). <br>

- Rather than selecting just one of Rock, Paper, or Scissors each player will select three moves.
- Each move will consist of a type (Rock, Paper, or Scissors) as well as a **strength value.**
- Each player will have 99 total points to use as strength between all three of their moves. For example, an example set of moves might be:

  - Move 1: Rock - 30 Strength Points
  - Move 2: Rock - 60 Strength Points
  - Move 3: Paper - 9 Strength Points

_The strength for each move must be at least 1._

After each player's moves are chosen, they will compare moves in the order they were selected. If two moves have different types (for example, Rock vs Scissors), then normal RPS rules will apply (in this case, Rock beats Scissors).
However, if two types are the same, then the move with more strength will win. If both strength values are
equal, then a tie is declared.

The player that wins the majority of the three rounds will be the winner of the game.

## Significant Code Highlights

### Scope

  -The project requred Twelve global variables (demonstrating knowledge of __scope__) representing each player's move types and values (3 move types and 3 move values for each player).

### Naming

- **Variable names** such as `playerOneMoveOneType`, `playerOneMoveOneValue` indicate appreciation of easy nomenclature for other professionals to follow later if/when needed.

### Functions

- #### Scope & Variables

  - My function called `setPlayerMoves`, which takes a string representing a player (in the form of `'Player One'` or `'Player Two'`), three move types, and three move values, sets the correct global move variables. The method signature for this function is: `setPlayerMoves(player, moveOneType, moveOneValue, moveTwoType, moveTwoValue, moveThreeType, moveThreeValue)` and demonstrates command of functions.

- #### Control Flow

  - A function called `getRoundWinner`, which takes a round number (`1`, `2`, or `3`), compares both player's move types and values for that round, and returns the appropriate winner (`'Player One'`, `'Player Two'`, or `'Tie'`) and demonstrate **control flow.**

  - A function called `getGameWinner`, which compares both player's move types and values for the whole game and returns the appropriate winner (`'Player One'`, `'Player Two'`, or `'Tie'`) also demonstrates **control flow.**

- #### Randomization

  - Bonus: There is a bonus function called `setComputerMoves`, which chooses three random moves for player two. The move type for each move is completely random, and the move values should be random but add up to 99. A terrific demonstration of controlflow and randomization packed into a function to create the sensation of automation for the user.

## Tip(s) for use

so you will need to use the most up-to-date version of Chrome to ensure your code runs correctly. If your
version of Chrome is too old, correctly-written code may still not run as expected.

## Testing

Learning Javascript yourself?

- A testing suite has been provided for you, checking for all essential functionality and edge cases.
- To run these tests, first open the root project directory in your terminal. Then run `npm install` to install all necessary testing dependencies (you will only need to do this step once).
- Finally, run `npm run test`. You will see a list of tests that ran with information about whether or not each test passed. After this list, you will see more specific output about why each failing test failed. 
- As you implement functionality, run the tests to
ensure you are creating correctly named variables and functions that return the proper values. 
- The tests will additionally help you identify edge cases that you may not have anticipated
when first writing the functions.
