# r-language
MATRIX ALGEBRA IN R

FONT: https://rpubs.com/adelmofilho/AlgebraMatricial
DATE -> 06-28-21

Adelmo Filho ( adelmo.aguiar.filho@gmail.com )


A simple matrix

M = matrix(data = 1:9, nrow = 3, ncol = 3)
print(M)

    [,1] [,2] [,3]
[1,]    1    4    7
[2,]    2    5    8
[3,]    3    6    9

By default, matrices are arranged by columns, but if you want to arrange in row, you must use "byrow = true" argument

 M = matrix(1:9, nrow=3, ncol=3, byrow=TRUE)
print(M)

     [,1] [,2] [,3]
[1,]    1    2    3
[2,]    4    5    6
[3,]    7    8    9

Working with data
V = c(12, 23, 34, 45, 56, 67)
M = matrix(data = V)
print(M)
     [,1]
[1,]   12
[2,]   23
[3,]   34
[4,]   45
[5,]   56
[6,]   67
--------------------------------------------------------

M = matrix(data = V, nrow=3)
print(M)
     [,1] [,2]
[1,]   12   45
[2,]   23   56
[3,]   34   67
--------------------------------------------------------

 M = matrix(data = V, nrow=4)
Warning message:
In matrix(data = V, nrow = 4) :
  data length [6] is not a sub-multiple or multiple of the number of rows [4]
  
M = matrix(data = V, nrow=2)
print(M)
     [,1] [,2] [,3]
[1,]   12   34   56
[2,]   23   45   67
--------------------------------------------------------

=> MATRIX ADDITION---------------------------------------------------------
M1 = 	|2 5|	M2 =	|5 8|
    	|3 6|	    	|3 2|

To add the matrix in R language you can use the example below
V1 = c(2, 5, 3, 6)
V2 = c(5, 8, 3, 2)

M1 = matrix(data=V1, nrow=2, ncol=2, byrow=TRUE)
M2 = matrix(data=V2, nrow=2, ncol=2, byrow=TRUE)

M1_M2_ADDITION = M1 + M2
print(M1_M2_ADDITION)
--------------------------------------------------------

=> SCALAR MULTIPLICATION---------------------------------------------------

	2 *|2 5| = |2*2 2*5|
	   |3 6|   |2*3 2*6|

multiplication by scalar using R language

V = c(2, 5, 3, 6)

M = matrix(data=V, nrow=2, ncol=2, byrow=TRUE)

print(M)

M_SCALAR = 2*M
print(M_SCALAR)
--------------------------------------------------------
