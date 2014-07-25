# makeCacheMatrix & cacheSolve Test Runs

#### Test aims to showcase the working of both the functions. 

 ```{r}
> # Creating an instance of makeCacheMatrix
> m=makeCacheMatrix()
> # Setting the value of the matrix
> m$set(matrix(1:4,2,2))
> # Getting the value of the matrix in the instance
> m$get()
     [,1] [,2]
[1,]    1    3
[2,]    2    4
> # Returning the inverse of the matrix in the instance
> cacheSolve(m)
no cached data! calculating inverse
     [,1] [,2]
[1,]   -2  1.5
[2,]    1 -0.5
> # No cached value was found. Inverse was computed
> # Checking if inverse is cached
> cacheSolve(m)
getting cached data
     [,1] [,2]
[1,]   -2  1.5
[2,]    1 -0.5

```