# Maze-Path-Finder
Code to find the most efficient path through a maze


This program incorporates Dijkstras Algorithm to find the quickest way through a maze. This is achieved by creating a dictionary of current nodes in the maze, recording their steps, explored status and distance to the end. At each node, the algorithm searches around, adding each to its node dictionary and marking the current node as "explored". 
The program then searches the node dictionary to find the unexplored node with lowest steps, choosing to explore this next. This process continues until reaching the end node, where the program backpropogates to find the fastest route to this node, effectively finding the most efficient path through the maze.


The maze is loaded via an excel, which has "1" for a wall and "0" as a path. The file "maze_input.csv" shows an example. This must have straight edges, with the top row and bottom row only containing one path, in order to have a start and end. The file "maze_input (pretty).xlsx" is an easy way to build this maze, with conditional formatting shows walls and path. This should be built in here then copied into the "maze_input.csv" file.

For the output, the file "maze_output.csv" has the maze and the fastest path shown through as a "2", with the same "1" for a wall and "0" as a path. Again, copying this into "maze_output (pretty).xlsx" can use conditional formatting to show the path in green for the visual effect.

------------------------
Dependencies
-

-The maze excel files must be stored in your local directory, as the code changes the directory to the correct place and finds the mazes in this place 
