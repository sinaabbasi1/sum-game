# :heavy_plus_sign: Sum Game
A simple arithmetic game designed in Proteus.

## Getting started

You need the Proteus Design Suite to play this game.

1. **Clone the repository:** <br />
```
git clone https://github.com/sinaabbasi1/sum-game.git
```
2. **Open and run the project:** Navigate to the `src/` directory and then using Proteus software run the game.

## Game Environment

**Sum Game** takes place in a 3x3 grid that forms the game environment. Each cell in the grid contains two blue 7-segment BCD displays, showing a two-digit number. Next to each cell is a button for selecting it. Additionally, there are three distinct cells, each with green 7-segment BCD displays, arranged so that the first cell's value is equal to the sum of the values in the second and third cells.
This is a two-player game that requires you to obtain scores under timed conditions. Each player has a pair of red 7-segment BCD displays—one for time and the other for score. Two red LEDs are used to indicate each player’s turn. The game also includes subcircuits and input buttons for interacting with the grid, along with Reset, Clk (clock), and Start controls.

<!--
## Screenshots

| ![Initial Game Setup](./screenshots/initial_game_setup.png) | ![First Move](./screenshots/first_move.png) | ![Player 2's (Susan) Winning Opportunity](./screenshots/player_2's_winning_oppurtunity.png) |
|:--:|:--:|:--:|
| *a. Initial Game Setup* | *b. First Move* | *c. Player 2's (Susan) Winning Opportunity* |

| ![Player 1's Defensive Move](./screenshots/player_1's_defensive_move.png) | ![Player 2's Second Attempt to Win](./screenshots/player_2's_second_attempt_to_win.png) | ![Player 2 Wins](./screenshots/player_2_wins.png) |
|:--:|:--:|:--:|
| *d. Player 1's Defensive Move* | *e. Player 2's Second Attempt to Win* | *f. Player 2 Wins* |
-->

## Game Rules

In the Sum Game, each player competes to select numbers from a 3x3 grid to form a correct sum. Each cell in the grid can only be selected once, and the first cell chosen must be the sum of the next two selections. The order of selection matters, and the turn alternates between players after each completes three selections.

The first turn always goes to the player on the left. Each player has 25 seconds to complete their turn, with the countdown paused when it’s not their turn. If a player forms a correct combination of numbers, they score a point. However, if time runs out during their turn, their game ends, and only the opponent can continue.

To ensure fairness, the circuit guarantees that at least one correct answer is possible each time the numbers are randomly distributed across the grid. This adds a layer of strategy, as players must act quickly and think critically to win.

## How to Play

In the Sum Game, each round consists of selecting a two-digit number that must equal the sum of two other two-digit numbers. Therefore, each player selects three cells per round. The game begins with the player on the left and continues as turns alternate, following the previously mentioned scoring and timing rules. The game continues until both players' timers reach zero. The player with the higher score at the end is declared the winner.

Alternatively, if a player reaches a score of 10 before time runs out, they automatically win, regardless of the remaining time.

## Contributing

Feel free to submit issues or pull requests if you find bugs or want to improve the game.

## License

This project is open-source and available under the [MIT License](LICENSE).
