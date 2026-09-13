# Fatal Echo

A 2D precision platformer built with Python and Pygame, featuring custom level parsing, platforming physics, pixel-mask collision detection, enemy behaviors, animation systems, camera scrolling, and multi-level progression.

## Overview

**Fatal Echo** is a 2D precision platformer developed in Pygame. The project was built to explore game programming fundamentals while implementing the underlying systems from scratch.

The game uses data-driven level layouts, modular entity classes, custom collision handling, and an animation system to support multiple levels, enemies, environmental objects, and player mechanics.

## Features

* **Data-driven levels**

  * CSV-based level layouts
  * Custom parsing and sprite generation
  * Multiple level components including terrain, enemies, collectibles, hazards, and spawn points

* **Player movement and physics**

  * Gravity and vertical momentum
  * Jumping and movement mechanics
  * Grounded/airborne state handling
  * Health and damage systems

* **Custom collision system**

  * Rectangle-based collision detection
  * Pixel-mask collision detection
  * Custom slope collision handling
  * Collision resolution for platforming movement

* **Animation system**

  * Frame-based character animations
  * Animation timing loaded from external data
  * Multiple player and enemy animation states

* **Enemy behaviors**

  * Multiple enemy types with independent movement and behavior
  * Patrol and attack behaviors
  * Enemy animations and state transitions

* **Camera system**

  * Player-centered scrolling
  * World-to-screen coordinate transformation

* **Game progression**

  * Multiple levels
  * Collectibles and scoring
  * Health and game-over systems
  * Level transitions
  * Menus and gameplay states

## Tech Stack

* **Language:** Python
* **Framework/Library:** Pygame
* **Data:** CSV
* **Graphics:** Pygame Surface and Sprite systems
* **Collision:** Pygame Rect and Mask systems

## Project Structure

```text
Fatal-Echo/
├── data/
│   ├── ...
│   └── ...
├── animation.py       # Animation loading and frame management
├── button.py          # UI button functionality
├── csv_loader.py      # CSV-based data and level loading
├── enemy.py           # Enemy classes and behaviors
├── level_map.py       # Level construction, collisions, and camera
├── main.py            # Main game loop and game states
├── player.py          # Player movement, physics, and interactions
├── score.py           # Score calculation and tracking
└── README.md
```

## Getting Started

### Prerequisites

* Python 3.x
* Pygame

### Installation

Clone the repository:

```bash
git clone https://github.com/EwickVon-1/Fatal-Echo.git
cd Fatal-Echo
```

Install Pygame:

```bash
pip install pygame
```

### Running the Game

Start the game with:

```bash
python main.py
```

## Controls

| Action     | Input     |
| ---------- | --------- |
| Move left  | `A` / `←` |
| Move right | `D` / `→` |
| Jump       | `Space`   |
| Pause      | `Esc`     |

> Controls may vary depending on the current game state.

## Technical Highlights

### Data-Driven Level Construction

Level layouts are stored as CSV data rather than being hard-coded directly into the game logic. The level loader interprets these layouts and constructs the appropriate sprites and entities at runtime.

This separates level design from gameplay code and makes it possible to create and modify levels without changing the core game systems.

### Custom Collision Handling

The platforming system combines rectangular collision detection with pixel-mask collision detection.

Pixel masks are used for more precise interactions with non-rectangular terrain such as slopes, allowing the player to interact with the environment more naturally than with simple bounding boxes.

### Modular Game Objects

The game separates major systems into individual modules for the player, enemies, levels, animation, scoring, UI, and data loading.

This keeps gameplay responsibilities separated and makes individual systems easier to modify without changing the entire game.

## What I Learned

This project gave me practical experience with:

* Designing a game loop and state-driven application
* Object-oriented programming in Python
* 2D physics and collision resolution
* Pixel-perfect collision detection
* Data-driven level design
* Sprite and animation management
* Separating gameplay systems into reusable modules
* Managing game state and progression
* Debugging interactions between multiple gameplay systems

## Project Status

Fatal Echo is a completed personal project and is preserved here as a portfolio project.

The repository was
