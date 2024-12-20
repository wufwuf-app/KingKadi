# Introduction
Kadi is a card game that can be played with 2-5 players using a standard 54-card deck. The game is fast-paced and simple to learn.

# Objective
The goal of Kadi is to be the first player to play all the winning cards in a single move.
Card Types

A standard 54-card deck is used, consisting of 4 suits (Hearts, Diamonds, Spades, Clubs) and 2 Jokers. Each suit has 13 cards, including Ace, 2 to 10, Jack, Queen, and King.

In Kadi, cards are specified as follows:
- Jack cards (J) are Jump Cards.
- Queen (Q) and 8 cards are Question Cards.
- King cards (K) are Kickback Cards.
- 4, 5, 6, 7, 9, 10, and Ace (A) cards are Answer Cards.
- 2, 3, and Jokers (JOK) are Penalty Cards.

# Dealing
The dealer shuffles the deck and deals 4 cards to each player. The remaining cards form the draw pile, and the top card of the draw pile is placed face up to start the discard pile. 

The following cards cannot start the discard pile:
- 2 and 3 cards
- Question Cards
- Kickback Cards
- Jump Cards
- Joker Cards
- Ace Cards

If one of these cards is drawn, the dealer returns it to the draw pile, shuffles the deck, places the top card face up, and repeats the process until a valid card is drawn.

# Rules
- Players must play a card that matches the suit or rank of the top card on the discard pile.
- If  a player chooses to play more than one card, the ranks of the cards must match, for instance if the suit top card of the discard pile is 10 Clubs, a player can choose to play 10H, 10D and 10S, changing the suit of the game to Spades.
- If a player cannot play a card, they must draw a card from the draw pile.
- If a player plays a Question Card, it must be accompanied by a matching answer card. If the player does not have an answer card, they must draw a card from the draw pile.
- If a player plays a Jump Card, the next player is skipped by them accepting the jump during their turn. However, the player who was to play next can counter the move by playing their individual Jump Card making it their turn.
- If a player plays a Kickback Card, the game direction reverses. The player who was to play next can counter the move by playing their individual Kickback Card, otherwise the game is reversed.
- Multiple Jump Cards can be played by the same player, and with each card, a player is skipped in the direction of play. Similarly, if multiple Kickback Cards are played, the direction reverses with each card.
- If a player plays an Ace card, they can declare the suit that the next player must play. If they do not, the game continues as usual.
- If a player realizes they can win on the next round of play, they must announce "Niko Kadi." Otherwise, they cannot win.
- If the draw pile runs out of cards, the discard pile (excluding the top card) is shuffled to form the draw pile.
- Penalty Cards (2, 3, and Jokers) must be followed by the next player drawing 2, 3 or 5 cards, respectively. The next player can avoid the penalty by:
    - Playing a penalty card(2 or 3) of the same rank or suit (forwards the penalty to the next player).
    - Playing a joker (forwards the penalty to the next player).
    - Playing an Ace card. The game continues with the suit of the Ace card.
- After a Joker card is played and the next player picks 5 cards, the next player after the penalized player is free to choose the game suit/rank.

```mdx
# Question Card Sequences

## Overview
Question Cards in Kadi consist of Queens (Q) and Eights (8). Players can play multiple Question 
Cards in a single turn, following specific sequencing rules. There are exactly **3,976** possible 
valid sequences.

## Available Cards
| Card Type | Cards |
|-----------|-------|
| Queens (Q) | QH, QD, QS, QC |
| Eights (8) | 8H, 8D, 8S, 8C |

## Sequencing Rules

### Same Suit Connections
- Queen → Eight 
  ```text
  QH → 8H (valid)
  QH → 8D (invalid)
  ```
- Eight → Queen
  ```text
  8H → QH (valid)
  8H → QD (invalid)
  ```

### Any Suit Connections
- Queen → Queen
  ```text
  QH → QD → QS (valid)
  ```
- Eight → Eight
  ```text
  8H → 8D → 8S (valid)
  ```

### General Rules
- Sequences can be 1-8 cards long
- No card can be used twice
- Either Queens or Eights can start a sequence

## Example Valid Sequences
```text
QS QH 8H 8S 8D
8D 8S 8H QH
8S QS QD
```

<Callout type="info">
  All sequences must follow suit-matching rules when connecting Queens (Q) 
  with Eights (8), while same card types (Q→Q or 8→8) can connect across suits.
</Callout>
```

# Winning
For a player to win, they must play all their winning cards in one move and, have had said “Niko Kadi” in the previous round. 

The winning cards are:
-	Answer Cards
-	Question Cards followed by their matching answer cards.

