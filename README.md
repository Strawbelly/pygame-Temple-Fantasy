# Temple Fantasy

**Temple Fantasy** is a turn-based tactical game built with **Python and Pygame**, featuring strategic team composition, character-specific abilities, AI-controlled opponents, and pixel-art combat animations.

Players assemble a team of three characters and battle through an ancient temple, combining attacks, defensive actions, and special abilities to defeat the opposing AI team.

## 🎮 Game Overview

Temple Fantasy combines turn-based combat with character-based strategy. Players choose **3 out of 6 available units**, each belonging to one of three classes:

* ⚔️ **Warriors** — High-damage offensive units
* 🛡️ **Tanks** — High-HP defensive and support units
* 🔮 **Wizards** — Healing, status effects, and utility abilities

The remaining three characters automatically form the AI-controlled team. Each character has unique attributes and a special ability, encouraging players to consider team composition, turn order, cooldowns, and combat status effects.

---

## 🛠️ Tech Stack

* **Language:** Python
* **Game Framework:** Pygame
* **Game Systems:** Turn-based combat, character abilities, cooldown and status-effect management
* **AI:** Computer-controlled opponent with automated unit actions and target selection
* **UI & Media:** Custom pixel-art interfaces, sprite animations, sound effects, and interactive controls

---

## 🕹️ Game Interfaces

### 1. Main Menu

The main menu allows players to **start or exit the game**. Interactive buttons provide visual hover effects and sound feedback.

<img width="992" alt="main menu" src="https://github.com/user-attachments/assets/7673b6d6-5d0d-4ae5-94d0-48a390b2a1ad" />

### 2. Unit Selection

Players build their team before entering battle.

* Choose **3 units from 6 available characters**.
* Characters are divided into **Warrior, Tank, and Wizard** classes.
* Character selection includes interactive sound feedback.
* Once three characters are selected, the remaining characters are automatically assigned to the AI team.
* The game then transitions directly into the battle interface.

<img width="993" alt="unit selection" src="https://github.com/user-attachments/assets/50370557-e607-4c2b-9f19-1deaa0b50c96" />

### 3. Battle Interface

The battle interface displays the player's team on the left and the AI-controlled team on the right.

Key interface components include:

* **Status Bars** — Display each unit's HP and special-ability cooldown.
* **Action Message Box** — Shows available actions, target-selection prompts, combat events, AI actions, and alerts.
* **Round Counter** — Tracks combat progression as units perform actions.
* **Current Unit Indicator** — Identifies the character whose action is currently being selected.
* **Combat Animations** — Characters have dedicated attack, special-ability, damage, and defeat animations.
* **Sound Effects** — Actions such as attacks, abilities, defense, damage, and character defeat include audio feedback.

<img width="994" alt="battle interface1" src="https://github.com/user-attachments/assets/331afef3-b5f5-41a4-bf9d-f4f8d0a0d01a" />

<img width="997" alt="battle interface2" src="https://github.com/user-attachments/assets/8df9f11d-f930-4efa-b3bf-c72da1cd3fe1" />

### 4. End Scene

When the battle ends, the game displays the final result and allows players to either **restart or exit**.

Restarting returns the player directly to the unit-selection interface for a new battle. The interface also includes interactive hover animations and sound effects.

<img width="993" alt="end scene1" src="https://github.com/user-attachments/assets/f3e9cfe6-5dc7-4653-9cdb-1c861270d0e1" />

<img width="997" alt="end scene2" src="https://github.com/user-attachments/assets/3b9a92fc-e442-47f4-8959-ea9d4f395a1e" />

---

## ⚔️ Combat Mechanics

### Turn System

Combat follows an alternating turn-based system between the player's team and the AI team.

* Player and AI units alternate actions.
* Each active unit performs **one action per turn**.
* Turn order is determined by team composition.
* Defeated units are removed from the active turn queue while the relative order of remaining units is preserved.
* Combat continues until one team has no surviving units.

### Available Actions

Each unit can choose from three primary actions:

**Attack**
Deals damage to a selected enemy unit.

**Defend**
Reduces incoming damage for one turn.

**Special Ability**
Performs a character-specific action after its cooldown requirement has been satisfied.

---

## ✨ Character Abilities

| Character     | Class   | Special Ability | Effect                                             |
| ------------- | ------- | --------------- | -------------------------------------------------- |
| **Warrior 1** | Warrior | Double Attack   | Performs a powerful double attack against an enemy |
| **Warrior 2** | Warrior | AOE Attack      | Deals damage to every member of the opposing team  |
| **Tank 1**    | Tank    | Fortify         | Temporarily increases the entire team's defense    |
| **Tank 2**    | Tank    | Shield          | Permanently increases an ally's defense            |
| **Wizard 1**  | Wizard  | Restore HP      | Restores health to the entire team                 |
| **Wizard 2**  | Wizard  | Poison          | Applies continuous damage to a selected enemy      |

---

## 📊 Character & Battle Status

### HP

Each character has an **HP bar** representing their remaining health. A unit is defeated and removed from combat when its HP reaches zero.

### Special Ability Cooldown

Each character has a **CD bar** representing the availability of their special ability.

After using a special ability, the cooldown resets. The ability becomes available again after the character completes **two rounds of Attack or Defend actions**.

### Poison Status

Characters affected by poison display a **poison status icon** above their sprite and continuously lose HP while the effect remains active.

### Current Unit Indicator

A **white arrow** at the bottom of the battle interface identifies the unit currently waiting for the player's action.

---

## 🏆 Win & Loss Conditions

**Victory**
The player wins when all AI-controlled units have been defeated.

**Defeat**
The player loses when all player-controlled units have been defeated.

The corresponding victory or defeat scene is displayed when either condition is reached.

---

## 👥 Contributors

### Developers

**Hewen Shen**
[LinkedIn](https://www.linkedin.com/in/hewen-shen-b94a26334/) · [Email](mailto:hewenshen0408@gmail.com)

**Lu Zhang**

**Xinyi Zhang**

### UI Designer

**Mengmeng Lu**
[Email](mailto:luumengmeng@163.com)
