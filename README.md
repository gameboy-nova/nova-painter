<p align="center">
<img src="https://github.com/user-attachments/assets/0ed0e6d8-6d2f-4e7b-a07b-a5dcdaf75809" width="300">
</p>

<h1 align="center"> 
Painter
</h1>

<p align="center">
Move a cursor across the screen and paint pixels using a selectable color palette.
</p>

---
## 🎮 Gameplay Showcase

Here’s a quick look at the game in action:
<p align="center">
<img src="https://github.com/user-attachments/assets/c2f68cc0-8699-4411-ba68-ba5e2c64d7c1" width="500">
</p>

---

### 🕹️ Controls

| Button   | Action                        |
|----------|-------------------------------|
| A_UP     | Move cursor up                |
| A_DOWN   | Move cursor down              |
| A_LEFT   | Move cursor left              |
| A_RIGHT  | Move cursor right             |
| B_UP     | Change selected color         |
| B_DOWN   | Toggle painting mode (on/off) |
| EXIT     | Exit game                     |

---

### 📦 Memory Usage  
- Canvas Grid: **2400 bytes** (40×30 cells, each pixel = 2 bytes)  
- Grid used for:  
  - `GET_COLOR`: Fetch cell color  
  - `STORE_COLOR`: Save drawn color  
- Coordinates are quantized to 8×8 pixel blocks on a 320×240 screen

---

### 🧠 Logic Overview  
The cursor moves across the grid, painting cells when in drawing mode.

---

### 🧩 Game Loop Structure  
1. Move cursor  
2. Paint if drawing mode is active  
3. Draw cursor  

---

### ❌ End Conditions  
- Exit input is received  

---

### 🧪 Notes & Improvements  
- Add color picker UI  
- Add erase and clear-screen functionality
