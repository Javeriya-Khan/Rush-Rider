List of Features Implemented

1.	Responsive real-time player controls for lane switching.
2.	Randomized AI enemy cars moving vertically in lanes.
3.	Fuel rewards with continuous fuel drain and refueling power-ups.
4.	Speed boost power-ups affecting player car velocity temporarily.
5.	Dynamic day and night modes for enhanced visuals.
6.	Collision detection triggers crash effects, camera shake, and game over.
7.	Car selection interface allowing users to pick different cars.
8.	Score tracking displayed in real time and saved to an external file upon game over.
9.	Audio message (Game over)
10.	Background music and sound effects for immersion.
11.	Exception handling for file operations and input validation.

GUI Layout Explanation
The user interface is structured into the following components:

1.	Main Menu Screen: Start game, car selection, and exit options with clearly labeled buttons.
2.	Car Selection Shop: Interactive grid showing available cars with selection highlight and navigation buttons.
3.	Game Screen:
o	Multi-lane road background with moving enemy cars and player’s car.
o	HUD displays score, speed, and fuel level with a horizontal fuel bar color-coded for urgency.
o	Power-up icons appear dynamically with animations.
o	Day/Night toggle changes background and visual effects.
4.	Game Over Screen: Displays final score, restart, and main menu buttons with crash animation and sound effects.

File Handling and Exception Handling Overview

•	File Handling:
Game scores are saved to and loaded from a text file after each game session. This maintains a record of high scores.
The program uses structured file operations with context managers to ensure safe reading and writing.

•	Exception Handling:
Implemented try-except blocks to handle:
o	FileNotFoundError and IO Error during file operations to avoid crashes if the score file is missing or corrupted.
o	Input validation for user selections to prevent invalid choices.
o	Graceful termination and error messages for unexpected runtime exceptions during gameplay.
