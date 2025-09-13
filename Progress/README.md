# Valdoria - Development Progress

This section documents the complete development journey of Valdoria, from initial concept to current state. Each milestone includes detailed explanations, blueprint screenshots, and demonstration videos.

## Development Timeline

### 📋 Table of Contents
1. [Current Progress As of Now](#Current-State-Of-The-Game)
2. [Development Starts : Creation of the Basic Map](#Creation-Of-The-First-Map)
3. [Locomotion and Equipment](#Locomotion-and-Equipment)
4. [Basic Combat](#Basic-Combat)
5. [Advance Combat](#Advance-Combat)
6. [AI Enemy System](#ai-enemy-system)

---
## Current State Of The Game

### Details
- This folder contains all the foundational gameplay modules and assets for Valdoria in Unreal Engine 5, such as actors, AI logic, animation events, components, damage systems, enums, interfaces, structs, and user interface code. Each directory organizes the project's scripts and assets by their function, making it easy to manage complex gameplay systems, communication, and visual feedback.
- This structure lets developers rapidly build, update, and debug unique features by keeping related gameplay logic, asset types, and framework code separated for clarity and efficient workflow.
<img width="927" height="480" alt="Screenshot 2025-09-13 205435" src="https://github.com/user-attachments/assets/1bd7a525-0505-4b18-ae9e-d9924bf40f78" />

- **BP_Combat_Character**: This is the demo player where i have implemented all other functionality to that character engaging.  
- **Actors**: Contains all core in-game objects, such as interactive items like LightSword and Greatsword that can be placed or spawned in the level.
- **AI** : Stores artificial intelligence logic including enemy behavior, pathfinding blueprints, and behavior trees, Blackboard, AI controller and a Boss_Enemy which uses all these concepts.
- **AnimNotifies** : Holds animation notifications used to trigger in-game events (like Attach_Weapon, Collision_Trace, iFrames, Reset_Combat, Rotate_Character and Toggle_Combat) at precise points within animation sequences.
- **Components** : Includes reusable modular features (like State_Manager, Stats, Targetting, Collision and Combat Coponents) that can be attached to multiple actors to add functionality.
- **Damage Types** : Contains Stun and damage types like low and heavy.
- **Enums** : Stores enumerations that define a fixed set of named constants (such as movement states, weapon types, or AI statuses) for use in logic and blueprints.
- **Interfaces** : Contains blueprint or code interfaces used to establish consistent communication rules between different actors or components.
- **Structs and UI** : Structs Holds user-defined data structures organizing related variables (like player stats) for easy management and blueprint access whereas UI Contains user interface assets such as HUD elements, widgets, and interface blueprints for in-game displays and player interaction.
<img width="918" height="525" alt="Screenshot 2025-09-13 205448" src="https://github.com/user-attachments/assets/714dc928-946a-4ec7-945b-9ac80ffdc82d" />
<img width="928" height="521" alt="Screenshot 2025-09-13 205500" src="https://github.com/user-attachments/assets/7afc8ba8-bbd5-4f53-b966-4c996474fa1f" />
<img width="925" height="513" alt="Screenshot 2025-09-13 205510" src="https://github.com/user-attachments/assets/11810fb0-9ba6-474e-9d66-0d34aa472918" />
<img width="916" height="518" alt="Screenshot 2025-09-13 205518" src="https://github.com/user-attachments/assets/66d5712a-0894-4b17-9e10-7a46948c1874" />
<img width="919" height="517" alt="Screenshot 2025-09-13 205527" src="https://github.com/user-attachments/assets/17f67a37-892c-4974-955e-871774909ac0" />
<img width="923" height="524" alt="Screenshot 2025-09-13 205534" src="https://github.com/user-attachments/assets/07e1391d-6a8c-4da5-b52a-a2fc01ef8b8b" />
<img width="914" height="526" alt="Screenshot 2025-09-13 205542" src="https://github.com/user-attachments/assets/e29fb213-3089-484a-9258-5c6784771294" />
<img width="920" height="523" alt="Screenshot 2025-09-13 205552" src="https://github.com/user-attachments/assets/73d0cbd8-e2f0-4716-bb6a-d41f7f8799f8" />
<img width="924" height="521" alt="Screenshot 2025-09-13 205607" src="https://github.com/user-attachments/assets/b04c701a-90ac-4570-aa6d-4f6dbeb3415b" />

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
- All of these are made using basic If else conditions.

### Visual Documentation
<img width="1419" height="695" alt="Screenshot 2025-09-13 213755" src="https://github.com/user-attachments/assets/90549f00-a339-404e-8070-cc54a5cb3eb0" />
<img width="1893" height="734" alt="Screenshot 2025-09-13 213852" src="https://github.com/user-attachments/assets/5c0d84ac-e74f-4d54-b0b2-903dea519982" />
*Character Interaction and Combat Toggling blueprint*

### Video Demonstration
<iframe src="https://www.linkedin.com/embed/feed/update/urn:li:ugcPost:7303810712391348225?compact=1" height="399" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>  

*Click on the link for Visual Demonstration*

---

## Basic Combat

### Implementation Details
- Added the attack Animations for the LightSword
- Directional Dodge
- Combat Reset
- Added a hit reaction and sound system for attacking

### Visual Documentation
<img width="1278" height="762" alt="Screenshot 2025-09-13 220020" src="https://github.com/user-attachments/assets/b03fa231-efe8-40c4-af0f-bd3f7b442bb8" />
<img width="1666" height="383" alt="Screenshot 2025-09-13 220110" src="https://github.com/user-attachments/assets/2bdc6b7d-e151-4607-86f0-b7cc22623b53" />
<img width="1707" height="724" alt="Screenshot 2025-09-13 220128" src="https://github.com/user-attachments/assets/4046a3cd-1231-4050-9d85-674214a5af5c" />
<img width="1788" height="448" alt="Screenshot 2025-09-13 220428" src="https://github.com/user-attachments/assets/0fa14ed4-1743-4454-bf2d-a9f8fe8886fe" />
<img width="1292" height="760" alt="Screenshot 2025-09-13 220514" src="https://github.com/user-attachments/assets/5c86854d-4b0d-48bc-91c0-81f07494f5d5" />

### Video Demonstration
<iframe src="https://www.linkedin.com/embed/feed/update/urn:li:ugcPost:7303812183438557203?compact=1" height="399" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>

*Click on the link for visual demonstration*

---
## Advance Combat

### Implementation Details
- Added a State Manager System that will remove the individual "if else" conditions and act on the basis of active actions. With the help of This , we can adjust the animations and Stats individually on each weapon.
- Added The Different Actions(Enumerations) for which the State Manager System will work.
1. Stats [None, Health, Stamina, Armor]
2. Character States 
[Nothing, Attacking, Dodging, General_Action_State, Dead, Disabled]
3. Character Actions
[Nothing, GeneralAction, LightAttacks, Dodge, Enter_Combat, Exit_Combat, SprintingAttack, HeavyAttack]
4. Movement Speed Mode
[Walking, Jogging, Sprinting]
- Targeting System
- Finally Updating the whole game mechanic to Game Tags

### Why Game Tags ?

First i have created the project on basic boolean variables and functions , then with enumerators and finally with Gameplay Tags.

1.Using Booleans and Functions
▪️ Defining game logic with booleans and functions keeps development simple and easy to debug. It provides a straightforward way to implement mechanics without complex data structures.
▪️ Booleans are easy to implement but become messy as complexity increases. Managing multiple conditions with booleans can quickly lead to confusing and error-prone logic
2.Enumerators (Enums) → Better than Booleans
▪️ Enums improve organization by replacing multiple booleans with a single variable that holds different states. This prevents conflicting conditions and makes code more readable and scalable.
▪️ Why Enums are better than Booleans?
🔸 Prevents multiple conflicting states (e.g., instead of isJumping, isRunning, isAttacking, use a single CharacterState).
🔸 Makes debugging easier by having defined states instead of multiple independent flags.
3.Updating with Gameplay Tags
▪️ Gameplay Tags allow flexible, data-driven logic by assigning tags to objects and actions. This system is highly scalable and integrates well with Unreal’s ability system.
▪️ Gameplay Tags outperform both booleans and enums by allowing dynamic, data-driven logic. Unlike enums, tags support multiple conditions at once and can be modified at runtime without code changes.
▪️ Why Tags are better than Enums and Booleans?
🔸 More flexible than enums as multiple tags can be assigned dynamically.
Reduces hardcoded logic, making the system modular and easier to extend.
🔸 Ideal for complex mechanics like ability systems, buffs, and AI behaviors.

### Visual Documentation
<img width="800" height="403" alt="image" src="https://github.com/user-attachments/assets/623b520c-096a-4c00-a8f4-1fd98c93a1ef" />



### Video Demonstration
<iframe src="https://www.linkedin.com/embed/feed/update/urn:li:ugcPost:7303812183438557203?compact=1" height="399" width="504" frameborder="0" allowfullscreen="" title="Embedded post"></iframe>

*Click on the link for visual demonstration*

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
