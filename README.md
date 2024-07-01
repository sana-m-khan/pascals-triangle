# pascals-triangle
~This was a java project that I created as a part of my final for my AP Computer Science class~
Given an integer numRows, return the first numRows of Pascal's triangle.

For this program, I was tasked with returning the first numRows of Pascal's triangle given an integer numRows. I created an ArrayList, holding Integer ArrayLists, which would return the triangle. The most difficult challenge in developing my algorithm was understanding if I wanted to use an equation or use nested for loops to add in the values. I decided to create 2 for loops, with one nested in the other. While researching Pascal's triangle, I came to understand that the first number and outer numbers in each level were all 1. Therefore, I decided to create a firstRow and add it to the triangle before entering the outer for loop because every version of Pascal’s triangle starts with one, and because I did not want the for loop to fail since I use prevRow in the upcoming loop. My outer loop adds another level to the triangle until it is less than numRows, and it resets prevRow and currentRow according to i to keep going through the triangle. Though, I chose to start at one for my outer loop since the method already adds the firstRow to the triangle before entering the loop. Before entering my inner loop, which adds each value in the row, I add 1 to the beginning of the current row since all numbers on the outside of Pascal’s triangle are 1. Then, I enter my inner loop, starting at one. I decided to use a variable, j, to add values to the current row using the explanation given in the project description. This for loop runs until it is less than the numRow it is on, because that method only adds the numbers in the middle of the row before exiting. Since each number is the sum of the 2 numbers above it, I use the .add method to add it and .get from the previous row to add the 2 numbers above the perspective number being added to the current row. After the inner loop exits, I add 1 to the current row again because all numbers on the outside of pascal’s triangle are 1. I decided to add a safety net at the start which would return the empty triangle if numRows is equal to 0. I print out the triangle at the end of the program, because what I return is the same thing that I have been alternating the whole program. I checked this program by alternating the number that I pass into the method for numRows.
