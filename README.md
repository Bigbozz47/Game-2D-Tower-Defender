# Game 2D Tower Defender
This project is a 2D Tower Defender game developed in Java, featuring various game states,
multiple enemy types, different towers, and core tower defense mechanics. Players must
strategically place towers to defend against waves of enemies, manage their gold, and protect
their lives.
## Features
- **Multiple Game States:**
 - **Menu:** Start the game, access settings, or exit.
 - **Playing:** Core gameplay where players defend against enemy waves.
 - **Editing:** A level editor to create and modify game maps, including path points.
 - **Settings:** Adjust game options.
 - **Game Over:** Displayed when the player runs out of lives, with options to replay or
 return to the menu.
- **Dynamic Gameplay:**
 - **Wave-based Enemy Spawning:** Enemies spawn in predefined waves with increasing
 difficulty.
 - **Enemy Movement:** Enemies follow a predefined path across the map.
 - **Tower Placement:** Players can place towers on grass tiles to attack approaching
 enemies.
 - **Projectile System:** Towers fire projectiles (arrows, bombs, chains) at enemies.
 - **Gold Economy:** Earn gold by defeating enemies and use it to build or upgrade
 towers.
 - **Tower Upgrades:** Improve tower damage, range, and cooldown.
 - **Selling Towers:** Regain some gold by selling placed towers.
 - **Lives System:** Lose a life if an enemy reaches the end point. The game ends when
 lives reach zero.
- **Diverse Entities:**
 - **Towers:** Archer, Cannon, and Wizard, each with unique attack types and properties.
 - **Enemies:** Orc, Bat, Knight, and Wolf, with varying health, speed, and rewards.
- **Map Interaction:**
 - **Tile Types:** Grass, Water, and Road tiles.
 - **Level Loading/Saving:** Levels are loaded from and saved to text files, allowing for
 custom map creation.
## How to Play
1. **Start the Game:** Run the Game.java file.
2. **Main Menu:** From the main menu, you can choose to "Play", "Edit" a level, adjust
 "Settings", or "Quit".
3. **Playing Mode:**
 - Enemies will appear from a designated start point and move towards an end point.
 - Click on the action bar at the bottom to select a tower.
 - Click on an empty grass tile on the map to place the selected tower.
 - Towers will automatically attack enemies within their range.
 - Monitor your gold and lives.
 - Click on a placed tower to view its stats and options to "Sell" or "Upgrade" it.
 - Press the "Pause" button to pause or unpause the game.
 - If all lives are lost, the game ends, and you will be directed to the Game Over screen.
4. **Editing Mode:**
 - Select different tile types (grass, water, roads) from the toolbar to design your own
 levels.
 - Set the start and end points for enemy paths.
 - Save your custom level for future play.
## Technologies Used
- **Java:** The primary programming language.
- **Swing:** Used for the graphical user interface (GUI) components.
## Project Structure
The project is organized into several packages:
- **main:** Contains the core game logic, including the main Game class, GameScreen for
 rendering, and GameStates enum.
- **scenes:** Manages different game screens like Menu, Playing, Editing, Settings, and
 GameOver.
- **managers:** Handles various game elements such as EnemyManager, ProjectileManager,
 TileManager, TowerManager, and WaveManager.
- **objects:** Defines the entities within the game, including Enemy, Tower, Projectile,
 Tile, and PathPoint.
- **enemies:** Specific implementations of enemy types (e.g., Bat, Knight, Orc, Wolf).
- **events:** Contains event-related classes, such as Wave for defining enemy waves.
- **ui:** Provides user interface components like ActionBar, MyButton, and Toolbar.
- **inputs:** Handles user input from keyboard (KeyboardListener) and mouse
 (MyMouseListener).
- **helpz:** Utility classes for constants (Constants), image manipulation (ImgFix), loading and
 saving data (LoadSave), and general utilities (Utilz).
## Getting Started
To run this project:
1. **Clone the Repository:**
 ```bash
 git clone https://github.com/bigbozz47/game-2d-tower-defender.git
 ```
2. **Navigate to the Project Directory:**
 ```bash
 cd game-2d-tower-defender/Game-2D-Tower-Defender-21537f18b1a914e047408e9b3bf76
 ```
3. **Compile the Java Files:**
 You can compile the Java source files using a Java Development Kit (JDK). If you are in
 the src directory, you can compile with:
 ```bash
 javac main/Game.java
 ```
 Or from the root of the cloned repository:
 ```bash
 javac src/main/Game.java -d bin
 ```
4. **Run the Game:**
 From the bin directory:
 ```bash
 java main.Game
 ```
## Credits
This project was developed by bigbozz47.