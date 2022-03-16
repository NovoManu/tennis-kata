# Tennis Game Kata JavaScript
Kata is taken here: https://github.com/ardalis/kata-catalog/blob/main/katas/Tennis%20Scoring.md

## Prerequisites
Node>=16

## Getting started
```
npm ci
```

## Testing
We can run all test cases with `npm test`

To start development in TDD mode use `npm run tdd`

## Introduction
We are going to create a game between two tennis players.
We should specify a game rules and players.

## Tennis game rules
In a game of tennis, a player begins with a score of zero (0). With each success, the player earns more points. The points are earned in this sequence:
0
15
30
40
If a player has 40 and scores again, that player wins the game as long as the other player does not also have 40 points. If both players reach 40 points it is referred to as a 'deuce.'

Scoring during deuce give a player advantage. If the other player scores again, the score returns to deuce. If a player has advantage and scores again, that player wins the game.

## Players
There are three types of player in the game: weak, middle, strong.
The probability between two players:
1. weak/weak, middle/middle, strong/strong - 50/50
2. weak/middle - 30/70
3. weak/strong - 10/90
4. middle/strong - 30/70

## Goal
We should create a game and simulate it between two type of players.
Write a program to handle each of these requirements while scoring a two player game of tennis.

Milestone 1:
Have a possibility to create a player with: name, gender and skills (week, middle, strong)
On this stage we should be possible to create a new player with parameters.

Milestone 2:
Create a simulation between two players which simulate one game between players. No scores is needed.
On this stage we should be possible to create a simulator with two players.

Milestone 3:
Create a score table between two players without deuce handling.
On this stage the two players should be able to finish the game if one of the players is above 40 points.

Milestone 4:
Handle a deuce case and create a full game simulation.
On this stage:
1. Players must be able to score points
2. The game must be able to be completed with a winner
3. The ‘deuce’ case should be handled
4. After a game has been won, a winner must be determined
5. The current score of either player should be available at any point during the game
