This project was meant to solve the Tiled Floor programming challenge featured in the 2022 Milwaukee School of Engineering (MSOE) Hackathon located in Wisconsin. The set of questions can be found here : https://faculty-web.msoe.edu/hasker/opcomp/op22/problems2022.pdf

The infamy of this question came from how challenging it was compared to its problem set. The solution guide can be downloaded here : https://faculty-web.msoe.edu/hasker/opcomp/op22/Op2022-solutions.zip which leaves out questions 7-9 including the Tiled Floor problem.

A friend of mine reached out directly to MSOE for answers and wasnt given a proper answer. Most likely this question was not designed to be this challenging, this challenge is exactly what attracted me to trying to solve or learn more about this problem.

The question is described as the following : 

"""<br>
**9. Tiled Floor (40 points)**

Sam recently hired a tile installer to tile a kitchen floor. The floor was supposed to be very colorful with no two adjacent tiles having the same color. Unfortunately, the installer failed to ensure adjacent tiles have different colors. The mortar is still wet, but it is difficult to lift just one tile at a time, so the installer is limited to swapping adjacent tiles. The question is how to exchange adjacent tiles in as few moves as possible so that the floor meets the criteria that no two adjacent tiles have the same color.

A sample input is <br>
**RGR<br>
RPC<br>
GRB<br>
YPG<br>**
Representing the tiles on a three by four floor where R is a red tile, G is green, B is blue, C is cyan, P is purple, and Y is yellow. In general, the input will be a series of lines of R, G, B, C, P, and Y. Each line will have the same length and there will be a maximum of 15 lines with 15 characters in each line. The output is to be an integer representing the number of swaps of adjacent tiles. For this problem, “adjacent” means touching and in the same row or column; for example, the only two tiles are adjacent to the yellow tile in the lower left corner of the above floor: the green tile at the start of the third row and the purple tile in the middle of the fourth row.

The output for the above floor will be<br>
**2**<br>
since the red tile at the start of row 2 can be swapped with the green tile at the start of row three, and then the
red tile in middle of row 3 can be swapped with the blue tile at the end. This gives the arrangement <br>
**RGR<br>
GPC<br>
RBR<br>
YPG<br>**
Other fixes are possible such as exchanging the first two tiles on row 2 to get PRC and then exchanging the middle tiles in rows 3 and 4. Your program does not print the resulting floor arrangement, just the minimum number of tile swaps that must take place. Sometimes it is not possible to fix a floor:<br>
**GGYGP<br>
CGGRG<br>**
This isn’t possible to tile because there are 6 Gs and a floor this size can fit only 5 without two being adjacent. In cases where there is no solution, the output is to be
**not possible<br>**
"""

The raw code and be found in the src folder. The question has remained unsolved without brute forcing all possible board permutations. This code was meant to better understand the patterns hidden in the question with the hopes of discovering an actual solution.
