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
* **Raycasting Core:** Custom `raycasting.py` algorithm without external game engines.
* **Viewport Rendering:** Dynamic mesh/conduit drawing in Rhino.
* **Input Hook:** `ctypes` based WASD keyboard control.

### **How to Run**
1.  Open `Rhino_DOOM_Core.gh` in Grasshopper.
2.  Set the Boolean Toggle to **True**.
3.  **Rip and Tear.** (Move with WASD)

---
*Disclaimer: This is a technical proof-of-concept. Performance depends on your single-core CPU speed. Frame drops are part of the experience.*
