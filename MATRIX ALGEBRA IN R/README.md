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