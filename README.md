# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### 1. To Find L and U matrices with LU Decomposition
Step 1: Get the matrix from the user.

Step 2: Using "from scipy.linalg import lu" to import scipy (LU) module.

Step 3: Using "L,U=lu(a)" we can get the matrix of L and U.

Step 4: Print the result matrices (L and U Matrices).

Step 5: End of the Program.


### 2. To Find X matrix with LU Decomposition
Step 1: Get the matrix from the user.

Step 2: Using "from scipy.linalg import lu_factor,lu_solve" to import scipy module for factorization and solving X.

Step 3: Using "lu,piv=lu_factor(a)" 

Step 4: print the result matrix (X matrix)

Step 5: End of the Program.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: K.M.Swetha 
RegisterNumber: 21500844
*/
import numpy as np
import scipy
from scipy.linalg import lu
a=eval(input())
p,L,U=lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by:K.M.Swetha 
RegisterNumber:21500844 
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:
(i):
![lu dec](https://user-images.githubusercontent.com/94228215/147852066-767386bc-8425-4d15-b94a-b01842723365.png)


(ii):

![lu dec2](https://user-images.githubusercontent.com/94228215/147852083-779b79fb-b71b-441c-b3bb-f094201494e8.png)




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

