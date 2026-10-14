# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import os and Import the numpy module to use the built-in functions.
2. Read the input matrix Aand perform LU decomposition to obtain the L and U matrices.
3. Read the right-hand-side matrix B and solve the system AX = B using LU decomposition.
4. Display the L, U and the solution X matrices , then stop the program.

## Program:
(i) To find the L and U matrix
```
Program to find L and U matrix using LU decomposition.
Developed by: SASTHARAJAN P
RegisterNumber: 26009606

import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu

a = np.array(eval(input()))
P,L,U = lu(a)

print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
Program to solve a matrix using LU decomposition.
Developed by: SASTHARAJAN P
RegisterNumber: 26009606

# To print X matrix (solution to the equations)

import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve

a = np.array(eval(input()))
b = np.array(eval(input()))

l, p = lu_factor(a)
x = lu_solve((l,p), b)
print(x)

```

## Output:
<img width="1238" height="841" alt="image" src="https://github.com/user-attachments/assets/55001511-de3c-4de8-8ccc-1495c459669e" />
<img width="1172" height="397" alt="image" src="https://github.com/user-attachments/assets/abb898b1-e924-443e-a582-4e10e92ed114" />

<img width="1207" height="761" alt="image" src="https://github.com/user-attachments/assets/52389e52-0946-4c67-a213-5c6bfaab6e03" />
<img width="1192" height="192" alt="image" src="https://github.com/user-attachments/assets/135e48c9-2b49-47ac-a186-04fb70ebfee5" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

