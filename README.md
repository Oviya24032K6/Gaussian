# Gaussian Elimination

## AIM:
To write a program to find the solution of a matrix using Gaussian Elimination.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Interchange and equation (or ).
2. Divide the equation by (or ).
3. Add times the equation to the equation (or ). Add times the equation to the equation (or ).
4. Multiply the equation by (or ).

## Program:
```
/*
Program to find the solution of a matrix using Gaussian Elimination.
Developed by: OVIYA P
RegisterNumber: 23013207

import sys
import numpy as np
n=int(input())
matrix=np.zeros((n,n+1))
x=np.zeros(n)
for i in range(n):
    for j in range(n+1):
        matrix[i][j]=int(input())
for i in range(n):
    if matrix[i][i]==0.0:
        sys.exit("Divided by zero error")
    for j in range(i+1,n):
        ratio=matrix[j][i]/matrix[i][i]
        for k in range(n+1):
            matrix[j][k]=matrix[j][k]-ratio*matrix[i][k]
x[n-1]=matrix[n-1][n]/matrix[n-1][n-1]
for i in range(n-2,-1,-1):
    x[i]=matrix[i][n]
    for j in range(i+1,n):
        x[i]=x[i]-matrix[i][j]*x[j]
    x[i]=x[i]/matrix[i][i]
for i in range(n):
    print("X%d = %0.2f"%(i,x[i]),end=" ")
    

*/
```

## Output:

![output](https://github.com/Oviya24032K6/Gaussian/assets/147139999/3e9d8734-aa67-4fdb-b3db-3801342741e2)



## Result:
Thus the program to find the solution of a matrix using Gaussian Elimination is written and verified using python programming.

