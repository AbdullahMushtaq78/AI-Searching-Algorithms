# A Star Search Algorithm to solve 8 Puzzle Problems.
- A* is considered one of the best informed searching algorithms because it considers both the heuristic and the actual cost to reach the goal state.
- This means that some heuristic values are already provided to the algorithm. The heuristic values are straight-line distances from the source to the destination.
- But in this problem, we need to make our heuristic function.
# Heuristic Functions:
- Misplaced Tiles:
  - This function calculates how many tiles are displaced from their goal position and return the count of these misplaced tiles.
- Manhattan Distance:
  - This function calculates how many steps each tile needs to take to reach its goal position and then sums up the value for all tiles.
# Algorithm:
![image](https://user-images.githubusercontent.com/96788451/194770086-b3135315-68bd-4f26-acc2-87635c4cd3b1.png)
- This algorithm maintains a priority queue that stores all of the nodes to be explored.
- Along with nodes, each node's (heuristic values + Actual Cost) are stored as a key in Priority Queue.
- First, it inserts the initial state with a (heuristic value + Actual Cost). Then in the while loop, it pops the node with the lowest (heuristic value + Actual Cost).
- Then, it calculates the next moves and their heuristic values and checks if these nodes are already explored or not.
- And then all of these new nodes are pushed into the queue if not explored already.
- And at each iteration, it checks if the current state is the goal state (heuristic values == 0) or not.
- If the current state is the goal state, then it simply traces the moves it took earlier by saving its parent states.
- The main difference between A star and Greedy best-first search algorithms is that A star considers heuristic + actual cost, but greedy best-first search only considers heuristic value.

