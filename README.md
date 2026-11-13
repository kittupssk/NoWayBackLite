# NoWayBackLite

**Catch the thief, or be the thief, on a new road map every game.**

**Play it:** https://kittupssk.github.io/NoWayBackLite/

A cop-and-robber puzzle on a map of junctions and roads. Both sides can see each other, both must move one step every turn, and nobody can wait. That one rule is what makes it a puzzle: if you and your opponent move in step, you can chase forever. The way to break the rhythm is a triangle of roads.

## How to play

- **Play as the police:** corner the computer thief by moving onto it, or by leaving it no road to escape along. Aim to match **par**, the fewest moves it can take against a perfect thief.
- **Play as the thief:** stay free for the number of police moves shown, against a computer police that plays perfectly on Hard.
- **Difficulty:** Easy, Normal and Hard change the map size, how well the computer plays, and how much thinking a map demands.
- **Hints:** a limited number per game show the best move.
- **Replays:** after each game, watch the best possible route or escape, or replay your own game.

## What makes every map fair

- A new random map every game, with no dead ends and no crossing roads.
- Every map is solved exactly before you play, so the goal is always possible with perfect play.
- Hard maps are checked so that simply walking toward the thief, or simply running away from the police, never works.

## Credits

Inspired by the puzzle in [Is it possible to catch the Thief?](https://www.youtube.com/watch?v=49oA4XFGeBI) by Logically Yours.

A lighter companion to [NoWayBack](https://kittupssk.github.io/NoWayBack/), a hidden-movement police and thief game by Krishnamohan Parimi ([source](https://github.com/kittupssk/NoWayBack)).

## Technical notes

The whole game is one self-contained `index.html` (HTML, CSS, SVG and JavaScript), with no build step and no dependencies apart from Google Fonts. The solver works backwards from every possible catch (retrograde analysis) to find the perfect move from any position.
