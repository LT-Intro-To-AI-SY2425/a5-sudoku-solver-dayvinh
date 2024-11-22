# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?
The Depth-First Search will be preferable generally when it comes to sudoku puzzles as it can be more efficient to explore a singular pathway in detail rather than briefly explore each pathway until a solution is reached in which a BFS algorithm would be preferred in a puzzle that involves more different posisbilities as a breadth-first search is more likely to come to a solution in lesser iterations.



2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?
Using a stack for DFS impacted the algorithm by forcing operations to execute based on recent additions to the algorithm rather than executing operations that were added first to the data queue. Because of this, an algorithm will perform differently based on how the user desires to sort their data and what order they wish for it to be carried out. Alternative data structures that could be used to achieve the same objective are linked lists and arrays which both store dtaa in a orderly fashion where arrays allow for particular elements of choice to be selected and linked list performs in a similar method, but instead allows for manipulation of the data.



3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?
The Sudoku solver can be extended for larer puzzles or different types of grid based logic games by either increasing the maximum value of spaces in each role and column by the desired amount rather than 9 or possibly decreasing the board size for a game like 8 picture puzzle. The lessons learned from this assignment can be applied to real-world problem-solving because this assignment fosters the idea of creating a base, in this case the board and creating algorithms to fill it with appropiate values based on the goal which can be applied to other problems that require automation of a task.