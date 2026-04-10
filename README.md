# Asterisk (HTML5 Port)

## What is Asterisk?
Asterisk is a modern HTML5 Canvas port of a classic C# WinForms game originally created by Mark Heath in 2003. 

In this frantic, single-button arcade game, you play as a single pixel continuously hurtling forward. Your only control is altitude, and your goal is to thread the needle through an increasingly dense field of asterisk (`*`) obstacles to find the gap in the right-side wall.

## How to Run
This game requires **no setup, no frameworks, and no internet connection**. 
1. Download the `asterisk.html` file.
2. Open the file directly in any modern web browser (Chrome, Firefox, Safari, Edge).
3. The game will run instantly.

## How to Play
* **Start:** Press `Enter` to begin.
* **Controls:** * **Hold `Enter`**: Your player (the yellow pixel) will rise.
  * **Release `Enter`**: Your player will fall.
* **Objective:** Survive until you reach the far right side of the screen. You must safely pass through the 30-pixel gap centered on the right-hand wall.
* **Crash Conditions:** You will trigger a Game Over if you hit:
  * The top or bottom white borders.
  * Any of the white `*` obstacles.
  * The solid sections of the right wall.
  * *Note:* Your player leaves a yellow trail behind. Though you continuously move forward, this game accurately replicates the original's exact pixel-collision mechanics!

## Difficulty Progression
Every time you beat a level, the game instantly scales up the difficulty:
1. **More Obstacles:** Each level spawns an increasing number of asterisks (Calculated as `Level × 3`).
2. **Speed Increase:** Starting at Level 5, the game's internal tick rate speeds up, giving you less reaction time to navigate the obstacle field. (The base 20ms tick drops by 1ms per level, creating a notably faster scroll).

## High Score
Your highest achieved level is automatically saved to your browser's `localStorage`. You can safely close your browser and come back later; your high score will persist in the top right corner.

## Credits
* **Original C# WinForms Game (2003):** Mark Heath ([www.wordandspirit.co.uk](http://www.wordandspirit.co.uk))
* **Original Source Code:** [Asterisk Repository](https://github.com/markheath/asterisk/tree/master/WinForms)
* **HTML5/Vanilla JS Port:** Adapted per user requirements for modern, standalone browser execution using HTML5 Canvas pixel-perfect collision.
