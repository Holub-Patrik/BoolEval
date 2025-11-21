# Boolean Expression Evaluator
Final implementation is in rec_solver.
I've gone through many attempts and implementations but in the end I've landed
at a recursive regex based parser implemented in rust. The implementation supports equations with up to 128 variable
as the program uses i128 for efficient and quick lookup of boolean values. 

A boolean equation evaluator. 

((a <=> b) ^ (c => (c | d))), [ a=1 ; b=0 ]

For this equation it should print out a table of all possibilities using a=1 and b=0 as fixed values and test all the other ones
It should also be able to print a simple table for n variables.
So given the number 6 it should print 

0 | 0 | 0 | 0 | 0 | 0\
0 | 0 | 0 | 0 | 0 | 1\
0 | 0 | 0 | 0 | 1 | 0\
.\
.\
.\

