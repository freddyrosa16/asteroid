# 🚀🪐 Asteroids Game (Pygame)

A simple Asteroids-style arcade game built with Python and Pygame.
Control your ship, shoot asteroids, and survive as long as possible.

------------------------------------------------------------------------

## 🎮 Features

-   🧑‍🚀 Player-controlled spaceship
-   🪐 Randomly spawning asteroids
-   💥 Asteroid splitting mechanic
-   🔫 Shooting system with cooldown
-   ⚡ Real-time movement and collision detection
-   📊 Game state & event logging (JSONL files)

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   Python 3
-   Pygame

------------------------------------------------------------------------

## 📂 Project Structure

    asteroids/
    │── main.py
    │── player.py
    │── asteroid.py
    │── asteroidfield.py
    │── shot.py
    │── circleshape.py
    │── constants.py
    │── logger.py

------------------------------------------------------------------------

## ▶️ How to Run

Make sure you have dependencies installed:

``` bash
uv pip install pygame
```

Run the game:

``` bash
uv run main.py
```

------------------------------------------------------------------------

## 🎮 Controls

-   **W** → Move forward\
-   **S** → Move backward\
-   **A** → Rotate left\
-   **D** → Rotate right\
-   **SPACE** → Shoot

------------------------------------------------------------------------

## 🧾 Gameplay

-   You start in the center of the screen
-   Asteroids spawn and move around
-   Shooting an asteroid splits it into smaller ones
-   If an asteroid hits you → **Game Over**

------------------------------------------------------------------------

## 📊 Logging System

The game automatically logs:

-   `game_state.jsonl` → snapshots of the game state
-   `game_events.jsonl` → important events (like hits and splits)

This is useful for debugging or building analytics later.

------------------------------------------------------------------------

## 🧠 Core Concepts

-   **Sprite Groups** for updating and drawing objects
-   **Vector Math** for movement and rotation
-   **Collision Detection** using radius distance
-   **Game Loop** with delta time (`dt`)

------------------------------------------------------------------------

## 📌 Notes

-   Runs at \~60 FPS using delta time
-   Uses simple geometric shapes (no assets required)
-   Logging stops after \~16 seconds to avoid huge files

------------------------------------------------------------------------

## 🧪 Example Output

Console:

    Game over!

Generated files:

-   `game_state.jsonl`
-   `game_events.jsonl`
