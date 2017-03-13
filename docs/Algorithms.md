# AI and Algorithms

### What are the advantages that A star has over breadth-first search? What advantages does A star have over depth-first search?

### Take a look at lines 124-127 of the code. Try commenting and uncommenting lines and running python astar.py to see what values are printed in each cell. Take a screenshot of each example with some lava tiles placed down, and in your own words, explain what f_score, g_score, and h_score are, and why you see those specific values in the screenshot.

g_score shows the number of the tile in terms of the path. For example a tile with the number 20 would be the 20th tile on the path chosen. The tiles that are not selected green shows the number it has along another longer path.
*Below: Example of g_score*
<img src="https://raw.githubusercontent.com/Elepert/ToolBox-AI/master/images/g_cost.png" alt="" width="200" />

h_score shows how far away the tile is from the cake in diagonals. The diagonal furthest away from the cake is Paul's face or number 18, second furthest is the two tiles next to him, so they're 17 away from the cake, etc...
*Below: Example of h_score*
<img src="https://raw.githubusercontent.com/Elepert/ToolBox-AI/master/images/h_cost.png" alt="" width="200"/>

f_score shows the sum of g_score and h_score. It adds how far away the tile is from the cake, as well as how far along the path Paul is.
*Below: Example of f_score*
<img src="https://raw.githubusercontent.com/Elepert/ToolBox-AI/master/images/f_cost.png" alt="" width="200"/>

### Read the get_open_adj_coords() function and lines 204 to 210 to get an idea of how valid adjacent cells are found. In the current code, valid adjacent cells only include the surrounding cells in the 4 cardinal directions, and moving to any of these cells costs 1 movement point. Add code changing the get_open_adj_coords() function so that surrounding diagonal cells are considered valid adjacent cells and moving to any of these cells costs 3 movement points. This will allow Paul to move diagonally.

### Change the program so that pressing 's' allows you to add swamp tiles. Paul should be able to move through swamp tiles, but they will slow him down! Moving into a swamp tile will cost 3 movement points, so Paul should really avoid moving through swamp tiles unless he has to. A swamp.jpg file has been provided for you in the /images folder. You will probably have to make some changes to the costs in get_open_adj_coords and write your own _add_swamp() function to get swamp tiles to behave correctly.

### Evolve Paul and allow him to jump over lava! Add the ability for Paul to jump one square. This should cost 8 movement points, however. This will involve changing get_open_adj_coords().
