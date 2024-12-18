WannaCry Game Project

## Overview

**WannaCry** is a top-down 2D recreation of the game 'hot potato'. In this game, players aim to avoid infection from a virus. If infected, the player can pass the virus on to another participant on the map. The objective is to maximize the time without the virus while minimizing the time in which the player has the virus. The game incorporates various AI methods to create intelligent, competitive computer-controlled opponents that provide challenging gameplay without requiring additional advantages or difficulties.

### Key Features

- **Game Mechanics**: Players can dash, teleport, or use terrain to evade or catch opponents. Items scattered around the map offer temporary advantages.
- **AI Integration**: Bots use AI algorithms to compete against players, employing tools and abilities effectively to create compelling challenges.
- **Score-Based System**: Players are scored based on infection time and last player to be infected. The leaderboard reflects the longest time evaded from the virus.
- **Technology Stack**: The game uses Java and Python with Gradle for handling dependencies.

## Disclaimer

Please note that the source code for this project was lost after graduation, as I no longer have access to university computers. However, this documentation and presentation provide a comprehensive overview of the game. Additionally, some videos may have been recovered to showcase how the game worked during development.

---

## Assumptions

1. JDK 11+ and Python 3+ are required.
2. Gradle will manage project dependencies.

---

## Requirements

### Functional Requirements

- **Players**: 
  - At least one controllable player.
  - Movement using W, A, S, D or arrow keys.
  - Ability to pass infection and avoid non-traversable tiles.
  - Use of special items via hot-keys.
  
- **Bots**:
  - At least two functional bots.
  - Bots operate within map bounds and do not walk on non-traversable tiles.
  - Bot behaviors controlled by respective AI algorithms.

- **Map**:
  - Top-down grid view with collision physics and strategic gameplay elements.
  - Items spawn randomly for player advantage or disadvantage.
  
- **Audio**: 
  - Background music and sound effects adjustable by the player.

- **Items**:
  - Power-ups include Freeze, Immunity, Quarantine, Silence Arrow, and Time Extender with varying impacts on gameplay.

- **Game Basics**:
  - Support for multiple players and bots.
  - Restart and quit functionalities during gameplay.
  - Developer mode for AI-only gameplay.

### Non-Functional Requirements

- Customizable player sprites ([C]).
- Multiple maps for player choice ([C]).
- Ultimate abilities with extended charge times ([C]).
- State of teleport and item cooldowns ([C]).

---

## Technical Details

- **Client-Server Model**: Python for the client and Java for the server.
- **Socket Communication**: Seamless interaction between client and server.
- **Scoring System**: Real-time scores, infection deduction, and bonus points for specific actions.

---

