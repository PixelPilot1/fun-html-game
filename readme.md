# Adventure Game

A text-based adventure game where players fight goblins, explore caves, and upgrade weapons and armor as they progress through an endless series of levels. Players can also save and load their game progress with save codes.

## Features

### Core Gameplay
- **Goblin Battles**: Encounter goblins and other enemies as you travel through different levels.
  - **Goblin HP**: Varies by goblin type (normal goblins, top goblins).
  - **Combat Options**: Players can choose to attack, defend, or heal during combat.
  - **Health Bars**: Both the player and enemies have health bars that update in real-time during combat.

- **Defend Mechanic**: When defending:
  - Players deal **5 damage** to the enemy.
  - The enemy deals **0 damage** to the player.

- **Random Scenarios**: Encounter goblins or other events randomly as you progress through levels 1-20, with harder enemies from level 21 onward.

### Shop System
- **Shop**: Players can purchase healing potions, weapons, and armor at regular intervals (every 5-20 levels).
  - **Potions**: Buy healing potions (heal 50 HP) or ultra healing potions (heal 100 HP).
  - **Weapons**: Upgrade your sword to deal more damage.
    - **Wood Sword**: 5 gold, deals 5 damage.
    - **Stone Sword**: 20 gold, deals 10 damage.
    - **Iron Sword**: 50 gold, deals 20 damage.
    - **Gold Sword**: 100 gold, deals 50 damage.
    - **Platinum Sword**: 200 gold, deals 100 damage.
    - **Diamond Sword**: 500 gold, deals 200 damage.
    - **Obsidian Sword**: 1000 gold, deals 500 damage.
  - **Armor**: Upgrade your armor to increase defense.
    - **Leather Armor**: 10 gold, gives 20 armor points.
    - **Chain Armor**: 20 gold, gives 30 armor points.
    - **Steel Armor**: 50 gold, gives 50 armor points.
    - **Gold Armor**: 100 gold, gives 75 armor points.
    - **Diamond Armor**: 200 gold, gives 100 armor points.
    - **Obsidian Armor**: 500 gold, gives 200 armor points.

### Player Stats and Progression
- **Stats Screen**: Players can view their current stats (level, health, attack, defense, sword damage, armor points, healing potions, gold) at any time.
- **Level Progression**: Players advance through levels by defeating enemies and surviving random events.
  - The level increases automatically after each scenario or battle.
  - Levels 21-50 feature stronger enemies, including **Top Goblins** with 200 HP and 20 damage per attack.
  
### Save and Load System
- **Save Game**: Players can save their progress at any time by generating a save code.
  - The game state (player stats, level, enemy stats) is encoded into a base64 string.
  - Players can copy the save code and resume the game later.
  
- **Load Game**: Players can paste a save code to load a previously saved game state.
  - The save code restores the player’s stats, level, and progress.
  
### Randomized Events
- **Randomized Goblin Encounters**: Players face random goblin encounters and shop intervals as they progress through the game.
- **Top Goblin**: Appears three times between levels 21 and 50, with 200 HP and 50 gold reward on defeat.

### Healing System
- **Healing Potions**: Players can buy and use healing potions during combat.
  - Normal healing potions heal 50 HP.
  - Ultra healing potions heal 100 HP.

### Combat System
- **Attack**: Standard combat option where players deal damage to the enemy based on their sword's damage.
- **Heal**: Players can use healing potions to restore health during combat.
- **Defend**: Reduces damage taken from the enemy and deals damage back to the enemy.
