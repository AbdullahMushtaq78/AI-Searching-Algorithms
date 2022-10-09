# Hill Climbing is one of the most used algorithms to solve Sudoku puzzles.
- This algorithm can solve the 4x4 board of Sudoku, but you can always change the board's dimensions by changing the dim variable at the start of the code.
- The Starting state of Sudoku is also predefined, but at the start of the algorithm, the user has the choice of entering his board values.
```
dim = 4
sudoku = np.array([
                [1,2,3,4],
                [1,2,3,4],
                [1,2,3,4],
                [1,2,3,4]]) 
```

# The Heuristic function used for this problem is:
  - Calculate All the non-unique values in each row + Calculate All the non-unique values in each column + Calculate All the non-unique values in Box of 2by2.
# Next Move:
  - This function generates all the next possible moves and returns them in a list.
# Hill Climb Algo:
![Pseudo Code of Hill Climb Algo](https://user-images.githubusercontent.com/96788451/194767565-bbaee569-f018-44a9-85cf-97190a862631.png)
  - This Algorithm uses this same technique of generating all the next possible moves and selecting the next based on the heuristic value of each state.
  - The state whose heuristic values are lower than the current state's is now the current state. 
  - This loops will keep on running until the goal state (heuristic == 0) is not achieved.
