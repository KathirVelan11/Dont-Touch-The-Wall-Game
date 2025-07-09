# 🧱 Don't Touch the Wall 

A multi-level 2D game built entirely using the Jack language.

## 🎮 Game Description
"Don't Touch the Wall" is a simple reflex game where players navigate a character through a narrow path without colliding with walls. Each level increases in difficulty, and there's a special two-player mode.

### Game Features:
- **Level 1**: Basic maze with three inner walls and outer borders
- **Level 2**: More complex maze with 21 walls, requiring precise navigation
- **Level 3**: Advanced maze with 42 walls, testing player skill
- **Two-Player Mode**: Competitive mode where two players navigate the same maze simultaneously
- **Collision Detection**: Real-time checking for ball-wall collisions, displaying an error message and allowing restarts

---

## 📦 Project Structure

| File                  | Description                                                                  |
|-----------------------|------------------------------------------------------------------------------|
| `Main.jack`           | Entry point. Manages game flow, level transitions, and mode selection.       |
| `Circle.jack`         | Handles the player's ball: drawing, movement, and position tracking.         |
| `CircleWall.jack`     | Wall objects used to construct maze boundaries and obstacles.                |
| `CircleGame.jack`     | Level 1 logic: basic maze and collision detection.                           |
| `CircleGameTwo.jack`  | Level 2 logic: intermediate maze layout.                                     |
| `CircleGameThree.jack`| Level 3 logic: advanced maze with 42 walls.                                  |
| `TwoPlayerGame.jack`  | Two-player mode logic and control handling.                                  |

---



## ⚙️ How to Run

### 1. Setup Nand2Tetris Tools
- Download and unzip the official [Nand2Tetris tools](https://www.nand2tetris.org/software).
- Go to the `tools/` folder.
- Launch `VMEmulator.bat` (Windows) or `VMEmulator.sh` (macOS/Linux).

### 2. Clone and Compile

```bash
git clone https://github.com/your-username/dont-touch-the-wall.git
```

### 3. Compile Jack Files

- Open the terminal in your project directory.
- Compile all `.jack` files using the Jack compiler.  
  If you are using the Nand2Tetris JackCompiler tool, you can run:
  ```bash
  # For a single file
  JackCompiler.sh Main.jack

  # Or for all files in the directory
  JackCompiler.sh .
- If any errors are shown in the terminal while compiling, try to resolve them before proceeding.

### 4. Launch the VM Emulator

- Open the VM Emulator (`VMEmulator.bat` or `VMEmulator.sh`).
- In the emulator:
  1. Click **File → Load Program**
  2. Select the folder containing **all your compiled `.vm` files**
  3. Click **Run → Normal** to start the game

---

## 💡 Important Tips

- **You must compile `.jack` files before running `.vm` files.**
- **Don't load individual `.vm` files—always load the whole folder.**
- **Ensure all compiled files are in the same directory.**

---

## 🤝 Want to Help?
Fork the repo and send a pull request with any improvements!
