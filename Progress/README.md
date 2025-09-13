# Valdoria - Development Progress

This section documents the complete development journey of Valdoria, from initial concept to current state. Each milestone includes detailed explanations, blueprint screenshots, and demonstration videos.

## Development Timeline

### 📋 Table of Contents
1. [Current Progress As of Now : 10 Sep 2025](#Current-State-Of-The-Game)
2. [Development Starts : 1 Feb 2025 -- Creation of the Basic Map](#Creation-Of-The-First-Map)
3. [Locomotion and Equipment : 4 Mar 2025](#Locomotion-and-Equipment)
4. [Combat Mechanics](#combat-mechanics)
5. [AI Enemy System](#ai-enemy-system)

---
## Current State Of The Game

### Details
- This Image Depicts the current Game mechanics involved in making the game and it contains:
  <img width="927" height="480" alt="Screenshot 2025-09-13 205435" src="https://github.com/user-attachments/assets/1bd7a525-0505-4b18-ae9e-d9924bf40f78" />
- **BP_Combat_Character**: This is the demo player where i have implemented all other functionality to that character engaging.  
- **Actors**: It Contains all the eqippable items from light sword to greatsword.
- **AI** : This folder contains Behaviour tree, Blackboard, Ai controller which helps me in creating AI enemies.



---
## Creation Of The First Map

### Implementation Overview
In the starting i created a small basic map which will lay out the foundation of this game's story and later into the characters movement mechanic. Everything Connects to Parhelion Tower. 

<img width="989" height="1914" alt="4" src="https://github.com/user-attachments/assets/ed7300bc-99e9-4c10-b466-8b7df137600b" />
 
---

## Locomotion and Equipment

### Implementation Details
- Added basic locomotion
- Creating base equipment(LightSword and GreatSword)
- Sheathing and Unsheating of Weapons 

### Visual Documentation
![Stats Blueprint](Blueprints/stats-system-blueprint.png)
*Character stats management blueprint*

![Stats UI](Screenshots/stats-ui.png)
*In-game stats display interface*

### Video Demonstration
[![Stats Demo](https://img.youtube.com/vi/STATS_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=STATS_VIDEO_ID)
*Character progression and stats in action*

---

## Combat Mechanics



### System Design
Implemented a comprehensive RPG-style character progression system featuring:

- **Health Points (HP)**: Player survivability
- **Mana Points (MP)**: Magical ability resource
- **Strength**: Physical damage modifier
- **Agility**: Movement speed and dodge effectiveness
- **Intelligence**: Magical damage and mana capacity

### Implementation Details
Created a custom Character Stats Component that handles:
- Stat calculation and modifiers
- Level-up progression curves
- UI integration for real-time display
- Save/load functionality for character persistence

### Visual Documentation
![Stats Blueprint](Blueprints/stats-system-blueprint.png)
*Character stats management blueprint*

![Stats UI](Screenshots/stats-ui.png)
*In-game stats display interface*

### Video Demonstration
[![Stats Demo](https://img.youtube.com/vi/STATS_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=STATS_VIDEO_ID)
*Character progression and stats in action*

### Combat System Overview
Developed an engaging hack-and-slash combat system featuring:

- **Combo Attacks**: Chained attack sequences
- **Dodge Mechanics**: I-frame evasion system
- **Damage Calculation**: Stat-based damage formulas
- **Hit Detection**: Precise collision detection
- **Visual Effects**: Impact particles and screen shake

### Technical Implementation
- Custom Combat Component for attack logic
- Animation Montages for attack sequences
- Hit-box collision detection using sphere traces
- Damage interface for consistent damage application

### Visual Documentation
![Combat Blueprint](Blueprints/combat-system-blueprint.png)
*Main combat logic implementation*

![Hit Detection](Blueprints/hit-detection-blueprint.png)
*Damage calculation and hit detection system*

### Video Demonstration
[![Combat Demo](https://img.youtube.com/vi/COMBAT_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=COMBAT_VIDEO_ID)
*Combat system showcase*

**Combat Features:**
- 3-hit combo system
- Critical hit mechanics
- Status effects (planned)
- Weapon variety (in development)

---

## AI Enemy System

### AI Architecture
Implemented intelligent enemy behavior using Unreal Engine 5's behavior tree system:

- **State Machine**: Idle, Patrol, Chase, Attack, Death states
- **Pathfinding**: Navigation mesh integration
- **Detection System**: Line-of-sight and proximity detection
- **Combat AI**: Attack patterns and defensive behaviors

### Behavior Implementation
- Behavior Tree for decision making
- Blackboard for AI memory and communication
- Custom AI Controller for enemy logic
- Pawn Sensing Component for player detection

### Visual Documentation
![AI Behavior Tree](Blueprints/ai-behavior-tree.png)
*Enemy AI behavior tree structure*

![AI Blueprint](Blueprints/ai-controller-blueprint.png)
*AI Controller implementation*

### Video Demonstration
[![AI Demo](https://img.youtube.com/vi/AI_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=AI_VIDEO_ID)
*Enemy AI behavior showcase*

**AI Features:**
- Multiple enemy types with unique behaviors
- Group coordination (basic implementation)
- Dynamic difficulty adjustment
- Boss AI with complex attack patterns

---

## Current Status & Next Steps

### Completed ✅
- Basic character movement and controls
- Character stats and progression system  
- Core combat mechanics
- Basic AI enemy implementation

### In Progress 🔄
- Boss fight mechanics
- Advanced AI behaviors
- Level design and environments
- Audio integration

### Planned 📋
- Inventory and equipment system
- Magic/spell system
- Quest system
- Save/load functionality
- UI/UX improvements

---

## Development Tools & Resources
- **Engine**: Unreal Engine 5.1
- **Programming**: C++ and Blueprints
- **Art Assets**: Fab Marketplace + Custom assets
- **Version Control**: GitHub
- **IDE**: Visual Studio 2022

**Last Updated**: [Current Date]
