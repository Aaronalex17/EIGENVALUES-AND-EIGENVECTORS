# EIGENVALUES-AND-EIGENVECTORS
## Aim:
To write a python program to find the Eigenvalues and Eigen Vectors
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Start with the Matrix:
Let 
𝐴
A be a square matrix of size 
𝑛
×
𝑛
n×n.
2. Compute the Characteristic Equation:
To find the eigenvalues, compute the characteristic equation:
det
(
𝐴
−
𝜆
𝐼
)
=
0
det(A−λI)=0
where:

𝜆
λ is the eigenvalue.
𝐼
I is the identity matrix of the same size as 
𝐴
A.
det
(
𝐴
−
𝜆
𝐼
)
det(A−λI) is the determinant of the matrix 
𝐴
−
𝜆
𝐼
A−λI.
This will give you a polynomial equation in 
𝜆
λ, called the characteristic polynomial.

3. Solve the Characteristic Equation:
Solve the characteristic polynomial 
det
(
𝐴
−
𝜆
𝐼
)
=
0
det(A−λI)=0 for 
𝜆
λ.
The solutions to this equation are the eigenvalues of the matrix 
𝐴
A.
4. Find the Eigenvectors:
For each eigenvalue 
𝜆
𝑖
λ 
i
​
 , find the corresponding eigenvector 
𝑣
𝑖
v 
i
​
  by solving the system of linear equations:
(
𝐴
−
𝜆
𝑖
𝐼
)
𝑣
𝑖
=
0
(A−λ 
i
​
 I)v 
i
​
 =0
This is a homogeneous system of linear equations, and the non-trivial solutions (i.e., eigenvectors) form a null space for the matrix 
𝐴
−
𝜆
𝑖
𝐼
A−λ 
i
​
 I.
Solve this system (using Gaussian elimination or other methods) to find the eigenvectors corresponding to each eigenvalue.
5. Return the Eigenvalues and Eigenvectors:
After solving for the eigenvalues and corresponding eigenvectors, output the results:
A list of eigenvalues.
A list of eigenvectors corresponding to each eigenvalue.


## Program:
```
import numpy as np
a= np.array([[2,-3,0],[2,-5,0],[0,0,3]])
values,vectors=np.linalg.eig(a)
print('Eigen values are {} and Eigen Vectors are {} '.format(values,vectors))
 
```

## Output:
![Screenshot (45)](https://github.com/user-attachments/assets/ded027f8-d75f-4af7-a1c0-5c492149a5c6)


## Result:
Thus the Eigenvalue and Eigenvector is successfully solved using python program
