<div align="center">

# 🫧 Dr. Bubble

**A retro-style arcade Bubble Shooter game built with pure Java.**

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Platform](https://img.shields.io/badge/Platform-Cross--Platform-blue?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

</div>

---

## 📖 Overview

**Dr. Bubble** is an arcade game inspired by the classic *Bubble Shooter*. Aim the cannon, match colored bubbles, and clear the board across multiple customizable levels.

This project was developed in Java, demonstrating core Object-Oriented Programming (OOP) concepts, a custom game-loop, and dynamic state management.

---

## ✨ Key Features

- 🎯 **Classic Arcade Mechanics:** Accurate trajectory calculations, bubble collision detection, and chain popping.
- 🎨 **Customizable Gameplay:** Personalize cannon skins, background themes, and player profiles from the in-game settings.
- 💾 **Persistent Settings:** Game audio levels, keybindings, and preferences are automatically saved locally.
- 🛠️ **Extensible Level Design:** Modular architecture allows new levels and custom worlds to be added easily.

---

## 🎮 Controls

| Action | Default Key / Input |
| :--- | :--- |
| **Aim Up** | `^` (Up Arrow) |
| **Aim Down** | `v` (Down Arrow) |
| **Fire Bubble** | `Left Mouse Click` |
| **Select / Confirm** | `Enter` |
| **Pause Menu** | `Esc` |

---

## 🚀 Getting Started

### Prerequisites
- [Java Development Kit (JDK) 8 or higher](https://www.oracle.com/java/technologies/downloads/) installed.

### Run the pre-built JAR
You can play immediately without compiling the source code:

```bash
# Clone the repository
git clone https://github.com/BillyErMago/Dr.Bubble.git
cd Dr.Bubble

# Run the executable JAR
java -jar Dr.Bubble.jar
```

*Note: On the first launch, a local preferences file will be generated automatically to store your default audio settings and bindings.*

---

## 🛠️ How to Add New Levels

The project uses a custom `GameStateManager` to manage game states and assets:

1. Create a new `.java` level class inside `src/` following the existing level structure.
2. Register the new state in `GameStateManager.java`.
3. Link the respective background and cannon asset paths:
   ```java
   // Example mapping in GameStateManager
   bgPath = "Resources/backgrounds/level_X.png";
   cannonPath = "Resources/cannons/cannon_X.png";
   ```

---

## 👤 Author

- **Billal Nadi** - [BillyErMago](https://github.com/BillyErMago)
```
