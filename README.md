# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### 5(A):
### Step 1:Import the required NumPy and SciPy libraries.
### Step 2:Get the input matrix from the user.
### Step 3:Use the lu() function to decompose the matrix into lower triangular (L) and upper triangular (U) matrices.
### Step 4:Display the L and U matrices as the output.
### 5(B)
### Step 1:Import the required NumPy and SciPy libraries.
### Step 2:Define the coefficient matrix \(A\) and the constant matrix \(B\).
### Step 3:Perform LU decomposition to split matrix \(A\) into lower triangular (L) and upper triangular (U) matrices.
### Step 4:Solve the equations using the L and U matrices and display the solution.
## Program:
(i) To find the L and U matrix
```

import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as n
from scipy.linalg import lu
a=n.array(eval(input()))
p,l,u=lu(a)
print(l)
print(u)

```
(ii) To find the LU Decomposition of a matrix
```
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
```

## Output:
<img width="1507" height="729" alt="image" src="https://github.com/user-attachments/assets/6ba0341a-7b70-4fe3-a4ce-8630c2ad271d" />

<img width="1506" height="731" alt="image" src="https://github.com/user-attachments/assets/92ca56ff-8bf9-4709-8e36-f2cf91acb096" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

