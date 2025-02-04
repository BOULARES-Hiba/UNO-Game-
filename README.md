# Java UNO Game Implementation

A command-line implementation of the classic UNO card game written in Java, developed as an academic project for university coursework.

## About

This project was developed as part of a university programming course to demonstrate object-oriented programming concepts in Java, including:
- Inheritance and polymorphism (card hierarchy)
- Encapsulation (player and game state management)
- Design patterns (dependency injection for Scanner)
- Clean code principles and documentation

## Features

- Support for 1-4 human players
- AI bot players for single-player mode or partial bot games
- Full implementation of classic UNO rules including:
  - Number cards (0-9)
  - Action cards (Skip, Reverse, Draw Two)
  - Wild cards (Wild, Wild Draw Four)
- Interactive gameplay with clear game state display
- Automatic card validation and move checking
- Support for multiplayer games with any combination of human and bot players

## Requirements

- Java 8 or higher
- Terminal/Command Prompt for playing the game

## How to Run

1. Compile all Java files:
```bash
javac *.java
```

2. Run the game:
```bash
java Main
```

## Gameplay Instructions

1. When prompted, enter the number of human players (1-4)
2. If applicable, enter the number of bot players (game requires 2-4 total players)
3. Enter names for human players
4. During your turn:
   - View your hand and the current top card
   - Choose a valid card to play or draw a new card
   - For Wild cards, select a color when prompted

## Game Rules

- Each player starts with 7 cards
- Players must play a card that matches either the color or number/symbol of the top card
- Special cards:
  - Skip: Next player misses their turn
  - Reverse: Changes direction of play
  - Draw Two: Next player draws 2 cards and misses their turn
  - Wild: Can be played on any card, player chooses the new color
  - Wild Draw Four: Same as Wild, but next player draws 4 cards and misses their turn
- First player to empty their hand wins

## Project Structure

- `Main.java`: Game entry point and setup
- `Game.java`: Core game logic and turn management
- `Player.java`: Base player class
- `HumanPlayer.java`: Human player implementation
- `BotPlayer.java`: AI player implementation
- `Card.java`: Base card class
- `NumberCard.java`: Number card implementation
- `ActionCard.java`: Action card implementations
- `WildCard.java`: Wild card implementations
- `Deck.java`: Card deck management

## Future Improvements

- Add graphical user interface
- Add save/load game functionality
- Enhance bot AI strategy
- Include game statistics tracking

## Acknowledgments

This project was developed as part of OOP at USTHB. Special thanks to the course instructors and teaching assistants for their guidance and support.
