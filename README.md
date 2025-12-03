Understanding the existing game logic The detailed analysis of Lane Runner Game (that was all I could understand) This is a simple console-based lane runner game. The player is at the bottom and can move left or right using arrow key. Obstacles fall from the top in random lanes, and the player has to avoid them. If an obstacle reaches the bottom in the same lane as the player, the game ends. How it works : The game keeps running in a loop. First, it checks if the player pressed left or right arrow keys and the player moves. Then it draws the lanes, obstacles, and player on the screen. The obstacle moves down one step in each loop. If the obstacle reaches the bottom where the player is, the game shows “GAME OVER” and stops. If the obstacle reaches the bottom but the player is not in that lane, a new obstacle comes from the top in a random lane.
Here obstaclePos is the lane of the current obstacle. 
rand() is used to place the obstacle randomly. 
_kbhit() and getch() are used to read player input without waiting. 
Sleep() controls the speed of the game.

(Modified Version)
This is an improved console-based Game written in C.
The player moves left and right to avoid falling obstacles. This modified version includes multiple added features such as lives, score, difficulty levels, and restart option.

**  Features Implemented
1. Score System
Score increases over time (or when the player survives obstacles).
Shows the score on the screen during the game.
Displays "Final Score" after the game ends.

2. Player Lives
Player gets 3 lives instead of instant game over.
Each collision subtracts one life.
When lives reach 0 → Game Over.

3. Difficulty Levels
Game speed increases automatically after certain score milestones.
Makes gameplay more challenging as the player survives longer.

4. Restart Game Option
After Game Over, the player is asked:
“Do you want to play again? (y/n)”
Choosing y restarts the game without restarting the program.

**  How to Play
- Use LEFT and RIGHT arrow keys to move the player.
- Avoid the falling obstacles.
- Score increases on each successful dodge.
- You have 3 lives — hitting an obstacle reduces 1 life.
- When lives reach 0, the game ends and restart option appears.
