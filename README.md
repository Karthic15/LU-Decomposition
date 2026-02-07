# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Start the program
2. Import the necessary libraries(numpy,scipy.linalg)
3. Define the matrix using numpy
3. Use lu(),lu_solve(),lu_factor() to get the solutions
4. End the program 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: KARTHIC V
RegisterNumber: 212225240068
*/

import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: KARTHIC V
RegisterNumber: 212225240068
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

<img width="1239" height="811" alt="Screenshot 2026-02-07 092927" src="https://github.com/user-attachments/assets/241cf4a9-89b0-4554-b095-cad023e6f6cd" />
<img width="1250" height="612" alt="Screenshot 2026-02-07 092943" src="https://github.com/user-attachments/assets/508ab3a1-0649-4354-af3a-f8d167aac1d4" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

