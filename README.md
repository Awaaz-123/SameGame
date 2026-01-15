A competitive color match-out puzzle game powered by Artificial Intelligence.*

---
Project Description

 A Java-based implementation of the classic SameGame puzzle, enhanced with an **AI agent** that autonomously selects optimal moves.

Unlike traditional player-controlled versions, this project showcases **AI-driven gameplay**, where the system analyzes the board, decides which group of blocks to remove, and plays until no valid moves remain. The focus is on **logic, reasoning, and optimization**, not reflexes.



--- Key Idea

The AI opponent uses **Answer Set Programming (ASP)** via the **EmbASP framework** and the **DLV2 solver** to:

* Analyze the current board state
* Identify removable clusters
* Choose the most rewarding move
* Continue playing until the game ends

This makes the project ideal for **AI, logic programming, and declarative problem-solving demonstrations**.

--- Features

* Fully automated **AI gameplay**
* Classic SameGame rules (gravity + column shifting)
* Dynamic scoring system
* Java Swing–based visual board rendering
* Integration with **ASP (DLV2)** for intelligent decision-making
* Clean separation between:

  * Game state
  * AI logic
  * UI rendering

--- Game Rules

* The board is a **10 × 20 grid** of colored blocks
* A move is valid if **two or more adjacent blocks** (horizontal or vertical) share the same color
* Single blocks **cannot be removed**
* After removal:

  * Blocks fall downward (gravity)
  * Empty columns shift left
* The game ends when **no more valid moves** are possible

--- Scoring System

 Score is calculated as:
(score) = (blocks_removed - 1)^2


* Larger clusters give higher rewards
* Final score is displayed when the game ends


--- How to Run

1. Ensure Java (JDK 8 or above) is installed
2. Add EmbASP libraries to the project
3. Place the DLV2 solver inside the `lib/` directory
4. Run:

bash
java MainClass

5. The AI will automatically start playing and the board will update visually

--- Educational Value

This project demonstrates:

* Declarative AI using logic programming
* Game state modeling with facts and rules
* Integration of AI solvers with imperative languages
* Practical use of **ASP in games**

Perfect for:

* AI coursework
* Logic programming labs
* University mini / major projects
* Research demos

--- Future Enhancements

* Player vs AI interactive mode
* Difficulty levels for AI
* Move-by-move visualization
* Statistics and replay system
* Online competitive mode

=================================================================
