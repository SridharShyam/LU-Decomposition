# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm:
1. Import the lu function from scipy.linalg for LU decomposition.
2. Convert the input string to a numpy array using the eval() function.
3. Use the lu() function to decompose the matrix A into P,and U.
4. Print the L matrix and U matrix.

## Program:
(i) To find the L and U matrix:

```
'''Program to find L and U matrix using LU decomposition.
Developed by: SHYAM S
RegisterNumber: 23012478
'''

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```

(ii) To find the LU Decomposition of a matrix:

```
'''Program to solve a matrix using LU decomposition.
Developed by: SHYAM S
RegisterNumber: 23012478 
'''

import numpy as np
from scipy.linalg import lu_factor, lu_solve
A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
x = lu_solve((lu, piv),b)
print(x)

```

## Output:
![Alt text](<Screenshot 2023-12-29 204604.png>)
![Alt text](<Screenshot 2023-12-29 204624.png>)
## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

