
# QuizQuest RPG

## Overview
The **RPG Quiz Game** combines RPG-style gameplay with quiz-based combat and decision-making. Players navigate a 20x20 map, encounter enemies, answer questions to attack, shop for upgrades, and face a final boss. The game supports multiple difficulty levels and custom question limits.

---

## Features
- **Exploration**: Navigate a 20x20 map, encountering enemies, shops, and a final boss.
- **Quizzes**: Answer randomized questions from easy, medium, or hard difficulty levels to attack enemies.
- **Combat**: Battle enemies and a final boss using your wits and weapon.
- **Progression**: Gain experience, level up, and upgrade your weapon or health using in-game currency.
- **Customization**: Choose the number of questions to answer and select multiple difficulty levels (easy/medium, medium/hard, etc.).

---

## Gameplay
### Objective
Survive battles, gain experience, and defeat the final boss while answering questions.

### Controls
- Use `W`, `A`, `S`, `D` to move across the map.
- Interact with elements (e.g., enemies, shops, boss) as you encounter them.

---

## Setup
### Prerequisites
- Java Development Kit (JDK) installed.
- Basic knowledge of running Java programs.

### How to Run
1. Save the source code to a file named `RPGQuizGame.java`.
2. Compile the game:
   ```bash
   javac RPGQuizGame.java
   ```
3. Run the game:
   ```bash
   java RPGQuizGame
   ```

---

## Customization
### Adding Questions
Modify the `setupQuestions` method in the code. Each difficulty level has its own question array. Ensure:
- The first option starts with `y` for the correct answer.
- Other options start with `x`.

**Example**:
```java
easyQuestions[0][0] = "What is 2 + 2?";
easyQuestions[0][1] = "y4";
easyQuestions[0][2] = "x3";
easyQuestions[0][3] = "x5";
easyQuestions[0][4] = "x6";
```

### Map Configuration
You can adjust map features (e.g., number of enemies, shops) by modifying these methods:
- `placeEnemies()`
- `placeShops()`
- `placeFinalBoss()`

---

## Rules
1. Correct answers deal damage to enemies or the final boss.
2. Incorrect answers result in losing health.
3. Level up by gaining 100 experience points:
   - Max health increases by 20.
   - Weapon damage remains unaffected unless upgraded at shops.

---

## Key Functions
### `askQuestion()`
- Selects a random question from the chosen difficulty level(s).
- Randomizes the order of answers.
- Deducts from the total question count.

### `shuffleArray()`
- Shuffles the order of multiple-choice answers.

---

## Future Improvements
- Add more complex question logic (e.g., timed responses).
- Support multiplayer mode.
- Expand map and introduce new enemy types.
- Save/load game progress.

---

Enjoy your adventure in the **RPG Quiz Game**! 🎮

Readme made with the assistance of AI
