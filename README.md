# Temple Fantasy 2024
- ## ***Game Overview***
Turn-based tactics meet mysterious ruins in this pixel art adventure where players command a team of three unique warriors in strategic combat. 
Set in an ancient temple where sacred stones are entangled by vines, players must defeat their AI opponents through strategic unit selection, tactical positioning, and special ability management.
- ## ***Game Interfaces***
### 1. Main Menu:
Players can choose to start the game or exit the game. When the mouse hovers over the "Start" or "Exit" button, the button will have dynamic effects and bubble sound effects. 

<img width="992" alt="main menu" src="https://github.com/user-attachments/assets/7673b6d6-5d0d-4ae5-94d0-48a390b2a1ad" />

### 2. Unit Selection:
- Units are divided into three classes: ***Warriors***, ***Tanks***, and ***Wizards***.  
- Players can choose 3 units from 6 available character types. When the mouse clicks on the surface of a unit, there will be a knocking sound effect on the surface.  
- When the player has selected 3 characters, the AI automatically receives the remaining 3 units. The game automatically enters the battle interface.

<img width="993" alt="unit selection" src="https://github.com/user-attachments/assets/50370557-e607-4c2b-9f19-1deaa0b50c96" />

### 3. Battle Interface:
*After selecting the game units and entering the battle screen, the left side is the player team and the right side is the AI team.*
- **Status Bar**: Status bars at the top displaying ***HP (health points)*** and ***CD (special ability cooldown time)*** associated with each unit.
- **Action Message Box**: Action message box at the left middle displaying Action or target selection request, player’s unit actions, AI’s unit actions and some potential alerts.
- **Round Counter**: The counter is used to record the rounds of the game. Each time a unit performs an action, the counter will increase by 1.
- **Unit Animation**: Each player's unit will have its own animation and sound effects when performing attack and special ability. The attacked unit will have a hurt animation effect. When the unit dies, there will be a falling animation effect and sound effect. The defend skill has a unified sound effect.

<img width="994" alt="battle interface1" src="https://github.com/user-attachments/assets/331afef3-b5f5-41a4-bf9d-f4f8d0a0d01a" />

<img width="997" alt="battle interface2" src="https://github.com/user-attachments/assets/8df9f11d-f930-4efa-b3bf-c72da1cd3fe1" />

### 4. End Scene: 
- Players can choose to restart the game or exit the game. When players choose to restart the game, they will automatically enter the unit selection interface and restart the game.
- When the mouse hovers over the ***"Restart"*** or ***"Exit"*** button, the button will have dynamic effects and bubble sound effects.

<img width="993" alt="end scene1" src="https://github.com/user-attachments/assets/f3e9cfe6-5dc7-4653-9cdb-1c861270d0e1" />

<img width="997" alt="end scene2" src="https://github.com/user-attachments/assets/3b9a92fc-e442-47f4-8959-ea9d4f395a1e" />

- ## ***Combat Mechanics***
### 1. Turn System
- Units from both teams take turns to act
- Player Unit 1 makes an action first, then AI Unit 1 makes an action, and so on…
- When a Unit dies, it is removed from the queue and its relative order in the queue remains unchanged.
- Turn order is determined by team composition
- Each unit can perform one action per turn
### 2. Character Available Actions

**Attack**: Deal damage to one enemy  

**Defend**: Reduce incoming damage for one turn

**Special Ability**: Unique action with a cooldown time

***Each unit has different special abilities:***
- ***Warrior1***: Double Attack, with double high attack power.
- ***Warrior2***: AOE (Area of Effect), can cause damage to every member of the opponent's team.
- ***Tank1***: High HP and Fortify, can enhance team defense for one turn.
- ***Tank2***: High HP and Shield, can permanently increase an ally's defense.
- ***Wizard1***: Restore HP, can increase the health points of the entire team
- ***Wizard2***: Poison Enemy, each use can poison one enemy, causing continuous damage.
### 3. Character Attributes
- **HP Bar**: Showing unit health. Unit dies when health points reach 0
- **CD Bar**: Indicating special ability cooldown. When the unit's CD bar is full, the unit can choose to use a special ability. The CD Bar will be fully refilled after the unit performs 2 rounds of attack or defense, which means the cooldown of the special ability has ended.
- **Poison Status Indicator**: When a unit is poisoned, a poison icon will light up above its head, and the unit's health will continue to decrease.
- **Current unit indicator arrow**: The white arrow at the bottom of the screen indicates the unit whose action is waiting to be selected.
- ## ***Final Results***
- **Win condition**: The player wins when the player eliminates all enemy units, and the interface will display victory information to the player.
- **Loss condition**: The player loses when the player loses all units, and the interface will display defeat information to the play
- ## ***Author***
[Hewen Shen](https://www.linkedin.com/in/hewen-shen-b94a26334/)

Lu Zhang

Xinyi Zhang

Mengmeng Lu
