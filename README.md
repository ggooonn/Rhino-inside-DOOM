# Rhino-inside-DOOM
> **"Yes... Rhino can run DOOM."**

**Rhino-inside-DOOM** is a proof-of-concept project that implements a DOOM-style raycasting engine directly within the **Rhino 3D** viewport using **Grasshopper** and **Python**.

This is not just a game; it is a computational design study on how to port spatial logic and rendering algorithms into an architectural modeling environment.

---

## Why? (Background)

The question "Can it run DOOM?" is the ultimate benchmark for any computing system. As an architecture student interested in computational design, I wanted to answer this question for the software we use every day.

Instead of running the original binary, this project **reconstructs the core logic of the DOOM engine (Raycasting)** using Python script inside Grasshopper. It bridges the gap between game level design and architectural spatial composition.

## How it Works (Technical Approach)

This project does not use any external game engines (like Unity or Unreal). It runs purely on Rhino's geometry kernel and Python.

* **The Brain (Logic):** A custom **Python** script handles the game loop, player physics, and raycasting calculations. It calculates the intersection between the player's view vector and the 2D map data.
* **The Eyes (Display):** * *Method A (Geometry):* Generating dynamic Rhino Meshes/Breps based on ray distance.
    * *Method B (Conduit):* Using `Rhino.Display.DisplayConduit` for pixel-level rendering (Planned).
* **The Hands (Input):** Using `ctypes` (Windows API) to hook keyboard inputs (WASD) for real-time navigation within the Rhino viewport.
