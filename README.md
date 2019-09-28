# CS591L1_Project_1

Include in the README a one-paragraph overview (5-7 sentences at least) describing the goal 
of your project and your approach. Include references to relevant concepts and terminology 
from the course as appropriate when describing your project.

Within this project, I am analyzing a subset of python that is used with the numpy library. The goal of my project was to figure out which constructs of python that I wanted to deal with, as seen in the BNF Notation.
I then use a decorator to check if a function has valid syntax (using only constructs that I deal with). To do this, I visited nodes within the AST of the program to determine if the individual parts of the program are within my subset of python and ultimately returned true or false.
The last part of the project, I analyze and transform code that uses numpy arrays. For the first, I visited nodes and instead of returning true or false, I look for the dimensions of np arrays and return them. I then go on to figure out which np arrays are being mulitiplied together to determine the size of a resulting np array from matrix multiplication.
Then the final part is taking a piece of python code and optimizing it by changing np.matmul (for matrix multiplication) to np.dot to optimize the code.