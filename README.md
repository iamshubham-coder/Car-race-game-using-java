# Car-race-game-using-java
Single-Threaded Design:

The game currently runs on a single thread, which handles both the game logic (e.g., collision detection, score updates, and obstacle movement) and rendering (e.g., drawing graphics on the screen).

The paint() method and the repaint() calls are executed on the Event Dispatch Thread (EDT), which is the main thread responsible for handling GUI updates in Java Swing.

Timer for Game Loop:

The game uses a Timer (from javax.swing.Timer) to control the game loop. This timer runs on the EDT, meaning all game logic and rendering are tied to this single thread.

While this approach works for simple games, it can lead to performance issues if the game logic becomes too complex or if rendering takes too long.


# key features
Player Movement: Control the car using the left and right arrow keys to avoid oncoming traffic.

Dynamic Obstacles: Randomly generated cars and trees create a challenging gameplay experience.

Score System: Earn points based on how long you survive in the game.

Speed Increase: The game speed increases over time, making it more difficult as you progress.

Game Over Screen: When the player collides with an obstacle, a game over screen is displayed with the option to restart the game.

Technologies Used:
Java: The core programming language used for development.

Java AWT/Swing: For rendering graphics and handling user input.

Randomization: Utilizes Java's Random class to generate dynamic obstacles.

How to Play:
Use the Left Arrow Key to move the car to the left.

Use the Right Arrow Key to move the car to the right.

Avoid collisions with other cars and trees to keep playing.

Press Enter to restart the game after a collision

