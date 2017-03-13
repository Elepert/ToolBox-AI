# AI and Algorithms

### What are the advantages that A star has over breadth-first search? What advantages does A star have over depth-first search?

### Take a look at lines 124-127 of the code. Try commenting and uncommenting lines and running python astar.py to see what values are printed in each cell. Take a screenshot of each example with some lava tiles placed down, and in your own words, explain what f_score, g_score, and h_score are, and why you see those specific values in the screenshot.

### Read the get_open_adj_coords() function and lines 204 to 210 to get an idea of how valid adjacent cells are found. In the current code, valid adjacent cells only include the surrounding cells in the 4 cardinal directions, and moving to any of these cells costs 1 movement point. Add code changing the get_open_adj_coords() function so that surrounding diagonal cells are considered valid adjacent cells and moving to any of these cells costs 3 movement points. This will allow Paul to move diagonally.

### Change the program so that pressing 's' allows you to add swamp tiles. Paul should be able to move through swamp tiles, but they will slow him down! Moving into a swamp tile will cost 3 movement points, so Paul should really avoid moving through swamp tiles unless he has to. A swamp.jpg file has been provided for you in the /images folder. You will probably have to make some changes to the costs in get_open_adj_coords and write your own _add_swamp() function to get swamp tiles to behave correctly.

### Evolve Paul and allow him to jump over lava! Add the ability for Paul to jump one square. This should cost 8 movement points, however. This will involve changing get_open_adj_coords().
