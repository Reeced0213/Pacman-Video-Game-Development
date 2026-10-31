# Pacman-Video-Game-Development
My video game development for Pacman
Pac-Man Browser Game

Overview

This project is a browser-based Pac-Man game built using HTML, CSS, and JavaScript. The game features a custom maze, an animated Pac-Man character, three ghosts, collectible dots, a scoring system, and collision detection.

The goal is to navigate the maze, collect all the dots, and avoid the ghosts. The project focuses on applying JavaScript programming concepts to create an interactive game with smooth character movement and real-time updates.

Features

Interactive Gameplay: Control Pac-Man using the keyboard's arrow keys.

Custom Maze: Navigate a maze containing walls, open paths, and collectible dots.

Animated Characters: Pac-Man has an animated mouth, and three colored ghosts move throughout the maze.

Scoring System: Earn 10 points for each dot collected.

Collision Detection: The game ends when Pac-Man collides with a ghost.

Win Condition: Collect all the dots to win the game.

Restart Functionality: Restart the game and play again.

Smooth Movement: Use JavaScript animation and frame-based updates to move characters between tiles.

Technologies Used

HTML5: Provides the game's structure and canvas element.

CSS3: Styles the game interface.

JavaScript: Handles character movement, keyboard input, scoring, collision detection, and game logic.

HTML Canvas API: Renders the maze, characters, dots, and game-over screen.

requestAnimationFrame(): Updates the game continuously to create smooth animations.

Git and GitHub: Used for version control and project documentation.

How to Play

Open the game in your browser.

Use the arrow keys to control Pac-Man.

Collect the white dots throughout the maze to earn points.

Avoid the ghosts.

Collect every dot to win.

Use the Restart button to begin a new game.

How It Works

Maze and Grid System

The maze is represented by a two-dimensional array of characters. Each character represents a type of tile, such as a wall, an empty space, or a collectible dot.

The game converts grid positions into pixel coordinates so characters can move smoothly through the maze.

Character Movement

Pac-Man and the ghosts move between tile centers. Before a character begins moving toward another tile, the game checks whether that tile contains a wall.

The movement system uses fixed destination coordinates to prevent characters from changing destinations halfway through a move.

Game Loop and Animation

The game uses requestAnimationFrame() to repeatedly update character positions, check game conditions, and redraw the canvas.

The elapsed time between animation frames is used to calculate movement, helping keep character speed consistent across different frame rates.

Scoring and Collision Detection

When Pac-Man reaches a tile containing a dot, the dot disappears and the score increases by 10 points.

The game also calculates the distance between Pac-Man and each ghost. If a ghost gets close enough, the game ends.

Challenges and Problem-Solving

One of the main challenges was implementing smooth character movement while preventing characters from passing through walls.

The initial movement logic had issues with tile detection and movement destinations. I worked through the problem by examining how pixel coordinates corresponded to maze tiles and restructuring the movement system so each character travels toward a fixed destination.

This process helped me understand the importance of consistent coordinate calculations, collision checks, and testing individual functions when debugging an interactive application.

What I Learned

Applying JavaScript fundamentals to an interactive application.

Working with objects, arrays, functions, loops, and conditional statements.

Handling keyboard events and user input.

Drawing graphics using the HTML Canvas API.

Implementing animation with requestAnimationFrame().

Using coordinate calculations for movement and collision detection.

Debugging problems involving character movement and maze boundaries.

Organizing a project into separate HTML, CSS, and JavaScript files.

Future Improvements

Add sound effects and background music.

Introduce additional maze designs and difficulty levels.

Improve ghost behavior with more advanced pathfinding.

Add a high-score system.

Make the game responsive to different screen sizes.

Add mobile-friendly controls.

Project Structure

PacMan Dev/
├── assets/
│   └── pacman.png
├── game.html
├── game.css
├── game.js
└── README.md

Developer

Created as a personal programming project to develop practical JavaScript skills and explore interactive game development.

