# Jacobi_Guass
Solving linear equations with iterative algorithms in Python 

## the Jacobi Method 
Determines solutions of a strictly dominant system of linear equations. 
Each diagonal element is solved for, and an approximate value is plugged in. 
The process then iterates until it converges. 

$Ax = b$

$A = D$ (diagonal) $+ L$ (Lower Triangular) $+ U$ (Upper Triangular)

Solution Iteration: $x^{k+1}=D^{-1}\left(b-\left(L+U\right)x^{k}\right)$ 

## the Gauss Seidel Method 
Though this method can be applied to any metric with non-zero elements on the diagonals, 
convergence is only guaranteed if the the matrix is strictly diagonally dominant (similar to the Jacobi Method). 
Also known as the ‘Liebmann Method’ or the ‘Method of Successive Displacement’. 

$Ax = b \Rightarrow L^{’}x = b - Ux \Rightarrow$ 

(Solution Iteration) $L^{’} x^{k+1} = b - Ux^{k} \Rightarrow x^{k+1} = L^{’-1} \left(b - Ux^{k}\right)$ 

## .txt files 
Matrices have been provided as .txt files for testing. In the line
```
file = open(“5mat3.txt”)
```
simply replace 5mat3.txt with any of the given matrices you wish to test. Only input one matrix at a time. 

Some of the matrices are incompatible with one or both methods for the purpose of testing. It might have non-zero elements on the diagonals, or may not be symmetric or positive definite. 
