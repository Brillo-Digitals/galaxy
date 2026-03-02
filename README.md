# Galaxy Kivy Game

Simple “space runner” style game built with Python and Kivy.

---

## 🚀 Overview

**Galaxy** is a small Kivy-based game where you pilot a ship through a scrolling field of tiles.  
Avoid obstacles and rack up your score!  
The project includes:

- `galaxy.py`, `menu.py`, and helper modules (`transform.py`, `user_actions.py`)
- Kivy layout files: `galaxy.kv` and `menu.kv`
- Assets under `audio/`, `images/`, `fonts/` and a high‑score CSV (`data/hs.csv`)

---

## 🛠️ Requirements

- Python 3.7+  
- [Kivy](https://kivy.org/) (tested with 2.x)  
- No external dependencies beyond the standard library  

Install Kivy in your virtual environment:

```bash
python -m pip install kivy
```

---

## ▶️ Running the Game

From the project root (`c:\Python Projects\kivy_games\galaxy`):

```bash
python galaxy.py
```

The main window shows a menu; press **START** (or use keyboard/mouse) to begin.

### Controls

- **Desktop**: arrow keys or touch  
- **Mobile**: touch on left/right half of screen

---

## 📁 Project Structure

```
galaxy/
├── galaxy.py        # main application logic
├── menu.py          # menu screen logic
├── transform.py     # helper for 3D‑style projection
├── user_actions.py  # input handling
├── *.kv             # Kivy layout files
├── audio/           # sound effects/music
├── images/          # graphical assets
├── fonts/           # custom fonts
├── data/hs.csv      # high‑score storage
```

---

## 💡 Notes

- Sound is handled via `kivy.core.audio.SoundLoader`.
- High scores are stored in `data/hs.csv`.
- Game‑over/restart logic included.
- The layout files define visual elements and bind to properties in Python.

---

## 📦 Packaging & Distribution

Package with tools like `pyinstaller` if you need an executable:

```bash
pyinstaller --onefile galaxy.py
```

Be sure to bundle `.kv` files and the `audio`, `images`, `fonts`, and `data` directories.

---

## ✨ Contribution

Feel free to fork, enhance graphics, add levels, or port to mobile!

---

*Have fun flying through the galaxy!* 🌌
