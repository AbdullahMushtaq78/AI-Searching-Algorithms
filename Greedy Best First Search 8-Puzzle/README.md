# Greedy Best First Search or Best First Search to solve 8 Puzzle problems.
- Greedy Best First Search is an informed searching algorithm. <br/>
- This means that there are some heuristic values already provided to the algorithm. The heuristic values are straight-line distances from the source to the destination. <br/>
- But in this problem, we need to make our heuristic function.
## Heuristic Functions:
- Misplaced Tiles:
  - This function calculates how many tiles are displaced from their goal position and return the count of these misplaced tiles.
- Manhattan Distance:
  - This function calculates how many steps each tile needs to take to reach its goal position and then sums up the value for all tiles.
## Algorithm:
![image](https://user-images.githubusercontent.com/96788451/194769568-3302703e-cc09-4189-8c7a-fdf093196988.png)
- This algorithm maintains a priority queue that stores all of the nodes to be explored.
- Along with nodes, the heuristic values of each node are stored as a key in Priority Queue.
- First, it inserts the initial state with a heuristic value. Then in the while loop, it pops the node with the lowest heuristic value.
- Then, it calculates the next moves and their heuristic values and checks if these nodes are already explored or not.
- And then all of these new nodes are pushed into the queue if not explored already.
- And at each iteration, it checks if the current state is the goal state (heuristic values == 0) or not.
- If the current state is the goal state, then it simply traces the moves it took earlier by saving its parent states. 

