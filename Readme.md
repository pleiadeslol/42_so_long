
# So Long - A Simple 2D Game

**So Long** is a beginner-friendly 2D game project designed to help developers explore basic computer graphics, game mechanics, and event handling using the **MiniLibX** library.

## 🚀 Project Overview

In this game, the player navigates a map, collects items, and reaches an exit while following specific gameplay mechanics. The project emphasizes creating a smooth graphical experience and validating user inputs and map configurations.

## 🛠️ Features

### Gameplay
- Navigate a 2D map using **W**, **A**, **S**, **D** keys (or arrows/ZQSD).
- Collect all collectibles on the map.
- Find the shortest path to the exit.
- Avoid obstacles and walls.
- Display the move count in the terminal after every action.

### Graphics
- Implemented using the **MiniLibX** library.
- Displays a 2D top-down or profile view of the game world.
- Smooth window management:
  - Press **ESC** or close the window to quit cleanly.

### Map Configuration
- Maps are defined in `.ber` files and consist of:
  - `0`: Empty space
  - `1`: Wall
  - `C`: Collectible
  - `E`: Exit
  - `P`: Player’s starting position
- Map validation includes:
  - Ensuring a rectangular shape.
  - Verifying it is surrounded by walls.
  - Checking for at least one `P`, one `C`, and one `E`.
  - Confirming a valid path exists.

### Example Map
```text
111111
1P0C01
100001
1C0E01
111111
```

## 🔧 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/pleiadeslol/42_so_long.git
   cd 42_so_long
   ```
2. Compile the game:
   ```bash
   make
   ```
3. Run the game with a `.ber` map file:
   ```bash
   ./42_so_long path/to/map.ber
   ```

## 🔎 Map Requirements
- The map must contain:
  - At least one **exit (E)**.
  - At least one **collectible (C)**.
  - One **player starting position (P)**.
- The map must be surrounded by walls (`1`) and must be rectangular.
- Any misconfiguration in the map file should result in an error message and program termination.

## 🧪 Testing
- Use valid and invalid `.ber` map files to test functionality.
- Ensure invalid configurations (e.g., missing components, non-rectangular maps) display appropriate error messages.
- Test smooth gameplay and edge cases like maps with minimal collectibles or large dimensions.

## 📜 Notes
- Created as part of the 42 curriculum.
- Focuses on foundational graphics and game design skills.
- A great stepping stone for more advanced graphic projects.

---

Happy coding and enjoy building your game! 🎮
