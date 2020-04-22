# Kernel dot product function

A CUDA program for computing the dot product of a vector in parallel with each row of a matrix and each thread access consecutive
memory locations (coalescent memory access). The inputs to function will be  
number of rows,number of columns ,a data matrix file ,a vector file (one row) ,cuda device , number of threads

Coalescent memory access :
All the consecutive threads access consecutive memory addresses.





