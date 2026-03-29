#  Campus Navigation: The "Maze Solver" Agent

###  The Problem

Imagine you are at the **Hostel (S)** and need to get to the **AI Lab (G)** for a morning class. The campus isn't just an empty field—there are buildings, walls, and restricted zones (**\#**) in your path.

I built this Python-based "Problem-Solving Agent" to figure out the best way to navigate a 7x7 grid using two different types of "AI brains": **BFS** (Uninformed) and **A**\* (Informed).

###  How the Agent "Thinks"

| Algorithm | The Strategy | My Observation |
| :--- | :--- | :--- |
| **BFS** | "The Blind Wanderer" | It checks every single direction equally. It's guaranteed to find the shortest path, but it wastes a lot of energy looking at walls. |
| **A* Search*\* | "The Smart Navigator" | It uses a **Heuristic (Manhattan Distance)** to "sense" where the Goal is. It's much more efficient because it focuses on moving toward the target. |

-----

###  Real-World Results

When I ran the code on my campus map, here is how the agent performed:

  * **Path Found:** Yes (19 steps total).
  * **Efficiency Win:** While BFS had to "look" at **24** different coordinates, A\* found the same path by only checking **\~21** spots.
  * **The Math:** A\* uses the evaluation function **f(n) = g(n) + h(n)** to stay on track.

###  Project Structure

  * `src/solver.py`: The core logic for the BFS and A\* algorithms.
  * `.gitignore`: Keeps the repository clean by hiding temporary `__pycache__` files.

###  How to Run the Solver

To test the agent on your own machine, follow these steps:

1.  **Run the Script:**
    Execute the main solver file from your terminal:
    ```bash
    python src/solver.py
    ```
2.  **Interpret the Map:**
      * **S** = Hostel (Start)
      * **G** = AI Lab (Goal)
      * **\#** = Buildings (Obstacles)
      * **\*** = The path discovered by the AI\!


**Created by:** Dhairya Jaiswal (25BAI10441)  
**Course:** B.Tech in Artificial Intelligence & Machine Learning  
<img width="870" height="732" alt="image" src="https://github.com/user-attachments/assets/d57e8b83-ef93-4600-a38d-420664ba94f7" />

<img width="870" height="687" alt="image" src="https://github.com/user-attachments/assets/aa31d624-d996-4e1f-a30d-565d29838bdb" />

<img width="869" height="494" alt="image" src="https://github.com/user-attachments/assets/9232e3f5-5082-4643-aa85-fad7ba37f8a1" />
