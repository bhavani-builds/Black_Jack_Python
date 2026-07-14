# 🃏 Blackjack Game (Python)

A simple command-line Blackjack (21) game built in Python. Play against the computer, hit or stand, and see who gets closer to 21 without going over!

```
.------.            _     _            _    _            _    
|A_  _ |.          | |   | |          | |  (_)          | |   
|( \/ ).-----.     | |__ | | __ _  ___| | ___  __ _  ___| | __
| \  /|K /\  |     | '_ \| |/ _` |/ __| |/ / |/ _` |/ __| |/ /
|  \/ | /  \ |     | |_) | | (_| | (__|   <| | (_| | (__|   < 
`-----| \  / |     |_.__/|_|\__,_|\___|_|\_\ |\__,_|\___|_|\_\
      |  \/ K|                            _/ |                
      `------'                           |__/           
```

## 📋 Features

- Play a full round of Blackjack against a computer dealer
- Automatic card dealing and score calculation
- Handles Aces intelligently (counts as 11 or 1 depending on the hand)
- Detects Blackjack, busts, and draws
- Simple, readable console output with a fun ASCII art logo
- Option to play multiple rounds in a row

## 🎮 How to Play

1. You and the computer are each dealt 2 cards.
2. Your full hand is shown; only the computer's first card is revealed.
3. Choose to **hit** (`y`) to take another card, or **stand** (`n`) to pass.
4. The computer automatically draws cards until its score is 17 or higher.
5. Scores are compared and the winner is announced.

### Rules

- Card values: number cards = face value, face cards (J/Q/K) = 10, Ace = 11 or 1
- A 2-card hand totaling 21 is a **Blackjack** (automatic win, unless it's a draw)
- Going over 21 is a **bust** (automatic loss)

## 🛠️ Requirements

- Python 3.x
- No external dependencies — uses only the standard library (`random`)

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/blackjack-python.git
   cd blackjack-python
   ```
2. Run the game:
   ```bash
   python solution.py
   ```
3. Follow the on-screen prompts to play!

## 📁 Project Structure

```
.
├── art.py         # ASCII art logo displayed at the start of each game
├── solution.py     # Main game logic (dealing, scoring, comparing, game loop)
└── README.md
```

## 🧩 Code Overview

| Function | Description |
|---|---|
| `deal_card()` | Returns a random card value from the deck |
| `calculate_score(cards)` | Calculates the total score for a hand, adjusting for Aces and Blackjack |
| `compare(u_score, c_score)` | Compares user and computer scores and returns the game result |
| `play_game()` | Runs a full round of the game, including dealing, hit/stand logic, and the computer's turn |

## 🙌 Acknowledgements

Inspired by beginner Python projects that teach control flow, functions, and simple game logic through a classic card game.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
