# Rhino-inside-DOOM

> "Yes... Rhino can run DOOM."

![Status](https://img.shields.io/badge/Status-Prototype-orange?style=flat-square)
![Language](https://img.shields.io/badge/Language-Python-blue?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Rhino_7%2F8-black?style=flat-square)

![Header Image](header_image.png)
### **Concept**
**Rhino-inside-DOOM** is a pure Python implementation of a **Raycasting Engine** (Wolfenstein 3D style) running directly within the **Rhino 3D** viewport.
It bridges the gap between architectural spatial logic and retro game mechanics, utilizing Rhino's geometry kernel for rendering.

### **Features**
* **Core Engine:** `raycasting_engine.py` implements the DDA algorithm purely in Python without external game engines.
* **Rhino Integration:** `renderer_rhino.py` handles dynamic drawing via Rhino's Display Pipeline (Conduit).
* **Input System:** `player_controller.py` utilizes `ctypes` to hook keyboard inputs (WASD) for real-time navigation.

### **How to Run**
1. Open `Rhino_DOOM_Core.gh` in Grasshopper.
2. Set the Boolean Toggle to **True**.
3. **Rip and Tear.** (Move with WASD)
