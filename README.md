# Blackjack Game

This is a simple console-based Blackjack game implemented in Python. The game allows the player to play Blackjack against a computerized dealer.

## Features

- **Unlimited Decks**: Decks are shuffled together for gameplay. Sorry no card counting.
- **Card Representation**: Uses a dictionary to represent cards with their corresponding values.
- **Player Interaction**: Players can "hit" or "stay" during their turns.
- **Dealer Logic**: The dealer hits until their hand value is 17 or more.
- **Ace Handling**: Ace cards can have a value of 1 or 11, and the code handles the choice appropriately.
- **Blackjack Check**: The game checks for Blackjack scenarios (an initial hand value of 21) for both the player and the dealer.
- **Bust Handling**: Bust conditions are handled, and the game declares a winner accordingly.
- **Play Again Option**: The player can choose to play again after each round.

## Getting Started

1. Ensure you have Python installed on your machine.
2. Clone the repository to your local machine.
3. Run the `blackjack.py` file to start the game.

## How to Play

1. The game starts by shuffling the cards and dealing two cards to both the player and the dealer.
2. The player is prompted to choose between "hit" and "stay."
3. If the player chooses to "hit," a card is dealt, and the game checks for bust conditions.
4. If the player chooses to "stay," the dealer reveals their facedown card, and the game proceeds with the dealer's turn.
5. The dealer hits until their hand value is 17 or more.
6. The game declares a winner based on the final hand values.

## Game Flow

1. **`game_start()`**: Initializes the game, shuffles decks, and deals initial cards.
2. **`is_blackjack()`**: Checks for Blackjack scenarios after the initial deal.
3. **`clear_values()`**: Clears lists storing player and dealer hands and values.
4. **`game_in_play()`**: Main gameplay loop where players decide to hit or stay.
5. **`stay()`**: Player decides to stay, and the dealer's turn begins.
6. **`player_out()`**: Continues the game after the player decides to stay, completing the dealer's turn.
7. **`hit(p, v, s)`**: Handles hitting logic for both player and dealer.
8. **`deal_card(p, s)`**: Deals a card to either the player or the dealer, with an option to show the dealer's card.
9. **`end_of_game()`**: Determines the winner at the end of the game.
10. **`bust(p, v)`**: Handles bust conditions and declares a winner.
11. **`play_again()`**: Asks the player if they want to play another round.
