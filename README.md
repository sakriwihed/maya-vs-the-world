# Maya vs the World 🎮
 
A 2D platformer game written in **C** with **SDL 1.2** on Linux.
Team project from my first year at **ESPRIT (Tunisia), 2023**.

## Features
 
- **Main menu & settings**: animated menu, background music, volume control, fullscreen toggle, custom key bindings
- **1 or 2 players**: both players play on the same keyboard
- **Scrolling background** with camera movement
- **Enemy AI** with three states (waiting → following → attacking) and bounding-box collision
- **Minimap** that shows the player's position in the level
- **Mini-games**: a riddle (enigma) and Tic-Tac-Toe
- **Best scores**, saved to a file and shown as a leaderboard
- **Arduino controller** support over the serial port
## Controls
 
| Action | Player 1 | Player 2 |
|---|---|---|
| Move | ← / → | A / D |
| Jump | Space | W |
| Settings / back | Esc | Esc |
 
## Tech
 
- C (multi-file project, built with a Makefile)
- SDL 1.2, SDL_image, SDL_mixer, SDL_ttf, SDL_gfx
- Serial communication (termios) for the Arduino controller

- 
## Project structure
 
| File | Purpose |
|---|---|
| `main.c` | Game loop and screen handling (menu, settings, game) |
| `menu.c` | Main menu, buttons, settings, audio |
| `player.c` | Player movement, jumping, animation, lives and score |
| `background.c` | Scrolling background and best scores |
| `ennemi.c` | Enemy animation, AI and collision |
| `minimap.c` | Minimap and Tic-Tac-Toe |
| `lot6.c` | Riddle mini-game and key-binding screen |
| `serie.c` | Serial port communication with the Arduino |
 
## Build & run (Linux)
 
```bash
sudo apt install libsdl1.2-dev libsdl-image1.2-dev libsdl-mixer1.2-dev libsdl-ttf2.0-dev libsdl-gfx1.2-dev
make
./prog
```
 
