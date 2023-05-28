# A* Algorithm Visualization 
#### Created a visualization of how A* algorithms work in the background to explore only necessary neighbors to get the optimal path.
#### To understand the basics of this algorithm with another example you can look at this repository of mine [![](https://img.shields.io/badge/-A*%20Search%208--Puzzle-orange?style=plastic&logo=github)](https://github.com/AbdullahMushtaq78/AI-Searching-Algorithms/tree/main/A%20Star%20Search%208-Puzzle)
#### By using the Pygames library in Python created an interactive visualization where:
- First-click will place the Starting Node in Orange color.
- Second-click on the box will place the Goal/End Node in Turquoise color.
- All the next clicks will create barriers in the grid.
- The user can press right-click to reset the box.
- Press the Space key to start the algorithm with visualization.
- Press 'c' to reset the canvas and start over again.
## Example of the algorithm running:
![A_Star_Visualization](https://github.com/AbdullahMushtaq78/AI-Searching-Algorithms/assets/96788451/b42baa92-37c5-48df-8ec0-af719b9e3769)
#### Components of visualization:
In this algo, we keep track of open and closed cells/neighbors that we have visited and are no longer usable for further calculation.
- The Orange color indicates the starting cell. 🟧
- The Green cells represent the neighbors which are in Open Priority Queue and we can visit and explore them further if needed. 🟩
- The Red cells represent that these cells/neighbors are explored completely by the algorithm and are no longer in Open Priority Queue. 🟥
- The Turquoise color represents the ending/destination/goal cell. 🟦
- The Purple line represents the optimal path that the algorithm has founded. 🟪
#### Updates:
- Added some new Heuristic Functions:
  - Euclidean Distance
  - Manhattan Distance
  - Chebyshev Distance

- Users can pass "euclidean", "manhattan", and "chebyshev" as distance_type parameters in the Algorithm function.
- Users can also change the number of rows and columns in the grid for creating more dense or lightweight scenarios.
