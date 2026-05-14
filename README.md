# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Start the program. 

2.Import the necessary libraries(numpy,scipy.linalg). 

3.Define the matrix using numpy.

4.Use lu(),lu_solve(),lu_factor() to get the solutions 5.End the program.

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: SRI VIJAY VARSHAN G
RegisterNumber: 212225240157
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)

/*
Program to find the L and U matrix.
Developed by: SRI VIJAY VARSHAN G
RegisterNumber: 212225240157
*/
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: SRI VIJAY VARSHAN G
RegisterNumber: 212225240157
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)

/*
Program to find the LU Decomposition of a matrix.
Developed by: SRI VIJAY VARSHAN G
RegisterNumber: 212225240157
*/
```

## Output:
<img width="1235" height="575" alt="WhatsApp Image 2026-05-14 at 8 12 55 PM" src="https://github.com/user-attachments/assets/547ba19d-05ef-4e68-afb5-1eca76160495" />
<img width="1232" height="293" alt="WhatsApp Image 2026-05-14 at 8 12 22 PM" src="https://github.com/user-attachments/assets/3958d244-17d3-4889-a294-7c977922c728" />




## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

