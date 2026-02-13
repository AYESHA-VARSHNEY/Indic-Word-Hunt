# Indic Word Search Solver 🔍🇮🇳

## 📌 Project Overview
**Indic Word Search Solver** is a Java-based desktop application designed to generate and solve word search puzzles in Indic languages (specifically Hindi). The project addresses the complexity of rendering and searching for words in regional scripts, providing an interactive GUI-based gaming experience.

## ✨ Key Features
- **Dynamic Grid Generation:** Uses a **Backtracking Algorithm** to place words randomly in a grid without overlaps or conflicts.
- **Multilingual Support:** Specifically optimized for Hindi characters and vocabulary.
- **Difficulty Levels:** Supports Easy, Medium, and Hard modes, adjusting the grid size and word complexity.
- **Database Integration:** Uses **SQLite** to manage and fetch a diverse set of words and store high scores.
- **Interactive GUI:** Built with **Java Swing**, featuring real-time score tracking, hints, and a reset option.

## 📂 Repository Structure
- `wss.java`: The main source code containing the game logic and GUI implementation.
- `data.db`: SQLite database file (if available) containing the word list.
- `PROJECT_REPORT.pdf`: Detailed documentation of the project development.
- `PROJECT_PRESENTATION_SRS.pdf`: Software Requirements Specification and analysis.

## 🛠️ Technical Stack
- **Language:** Java
- **Framework:** Java Swing (GUI)
- **Algorithm:** Backtracking (for word placement)
- **Database:** SQLite (JDBC)
- **Development Tool:** IntelliJ IDEA / Eclipse

## 🚀 How to Run
1. Clone the repository.
2. Ensure you have **JDK 8+** installed.
3. Add the **SQLite JDBC Driver** to your project classpath.
4. Update the `dbPath` in `wss.java` to point to your local `data.db` file.
5. Compile and run `WordGuessingGameGUI`.

## 🧠 Methodology (Analysis Model)
1. **Grid Generation:** The system ensures no two words occupy the same cell unless they share a character.
2. **Word Search Algorithm:** Validates user selections against the generated grid in real-time.
3. **Score Calculation:** Calculated based on the number of words found and the time taken.
