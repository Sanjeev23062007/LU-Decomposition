# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step-1:
Read the elements of augmented matrix into array a and b 
### Step-2:
Calculate elements of L and U
### Step-3:
Print Land U matrix
### Step-4:
Find V by solving LV = B by forwrd substitution
### Step-5:
Find X by solving UX = V by backward substitution
### Step-6:
Print array X as the solution 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Sanjeev A 
RegisterNumber: 212224230246
*/ 

import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Sanjeev A
RegisterNumber: 212224230246
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor(a)
x=lu_solve((lu,piv),b)
print(x)
```

## Output:
![image](https://github.com/user-attachments/assets/b772f758-c731-400e-9a47-3f6de10d280d)
![image](https://github.com/user-attachments/assets/678cbc0b-b75b-4df0-b91c-3e2dcca1076b)



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

