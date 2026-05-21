# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. The program uses the scipy.linalg library to perform LU decomposition.
2. The matrix is defined as a NumPy array using np.array().
3. The lu() function decomposes the matrix into a Lower triangular matrix (L), an Upper triangular matrix (U), and a Permutation matrix (P).
4. The matrices L, U, and P are displayed to verify the LU decomposition of the given matrix.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: bharath s
RegisterNumber: 212225230031
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,L,U=lu(a)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: bharath s
RegisterNumber: 212225230031
'''

# To print X matrix (solution to the equations)
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor, lu_solve
a=eval(input())
b=eval(input())
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)

```

## Output:
<img width="850" height="494" alt="image" src="https://github.com/user-attachments/assets/3cd0a198-67f3-4ae1-b3d7-666fea32c845" />
<img width="859" height="230" alt="image" src="https://github.com/user-attachments/assets/79c785b8-1317-4291-b096-56015595785b" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

