# Maze solver

>  The project is to build a program that run the command -Line tool.A maze in the form of matrix will be given in the form of 1's and 0's ,where   1 is represent as open path and 0 is represent as blocked path.The goal is to find the path between source to destination int the maze.otherwise return "-1" that indicate no path exist between source to destination.

## Concept used-

1. File handling

2. Backtracking


### Approach

1. The maze is given NxN matrix we have to find the path from source to destination.There are some cell which are blocked means we cannot enter into those cells.Whenever we move to cell in amze,mark that particular solution matrix.At the end print the solution matrix.Ifwe reach at the
destination print the solution matrix.Otherwise mark "-1".

2. From a recursive function,which will follow a path and check if the path reaches the destination or not.If the path does not reach the destination then backtrack and try other paths.

3. If none of the above solution works then backtrack and mark the current sellas 0.It is important to check the previous direction in which the we have to moved because if we will move in the opposite direction its previous direction then we might end up in the infinite loop.

#### Instruction to run the project

1. Open a file inputfile,txt in write mode.Take the input for the order of the input matrix.Close the file.Again open the inputfile.txt in read mode .Close the file.Again open the inputfile.txt in append mode .Close the file.Again open the inputfile.txt in read mode .Close the file.

2. Open the outputfile.txt in write mode.
3.Open the github 
4.From github repo copy the code to the python editor and save the file in certai folder.
5.In the editor terminal set the path to the program where your code is save.
6.Execute the code file by writing :python maze1.py -i inputfile.txt -o outputfile.txt
7.After passing the file names give the matrix size =n (can be any number suppose 4)
8.  Type n row in terminal 1 0 1 1
                           1 0 1 1
                           1 1 0 1
                           1 1 1 1
9. This will also write in the inputfile.txt
10.The output will be write in the outfile.txt 1 1 0 0
                                               0 1 0 0
                                               0 1 0 0
                                               0 1 1 1
    