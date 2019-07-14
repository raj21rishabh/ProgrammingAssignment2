#Programming Assignment 
#Solution:
1. How to use these functions for testing the lexical scoping??

1.1 Create an object which will store the contenct of the matrix, his inverse, and functions to access them
> wrapper= makeCacheMatrix();

1.2 Assign the content of the matrix to calculate the inverse to this wrapper
> wrapper$set(matrix(1:4,2,2))

1.3 The object contains the matrix. Call the function above "cacheSolve" which will check if the invese has been calculated and cached previously. Otherwhise will perform these operations.

 Calculate the inverse (1st time) of the matrix included into the wrapper object
 > cacheSolve(wrapper)
       [,1] [,2]
       [1,]   -2  1.5
       [2,]    1 -0.5
       
 The second time it will retrieve it from cache
 > cacheSolve(wrapper)
 getting cached data
       [,1] [,2]
       [1,]   -2  1.5
       [2,]    1 -0.5
