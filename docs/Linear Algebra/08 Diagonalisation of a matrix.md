# Diagnolization of a matrix

Let us consider a matrix $A,$ and there exists an invertible matrix $S,$ such that $S^{-1}AS=B,$ where $B$ is a diagonal matrix. Then $A$ is said to be diagonalizable.

<!-- TODO Start -->
## Relation between Diagonalization and EigenVectors
- Claim: If eigenvalues are distinct then eigenvectors are linearly independent
<!-- TODO End -->

## Observations
1. For a given matrix $A,$ $S$ is not unique. This is because the eigenvectors can be scaled by any factor.
2. Using the power property from [eigenvectors and eigenvalues](./07%20EigenValues%20and%20EigenVectors/#some-important-properties), we can get $S^{-1}A^kS=B^k$
3. Not all matrices are diagonalisable.

## A quick tip
If you ponder upon the process, you can see that you $S$ is a set of all the eigen vectors, i.e., $S=\begin{bmatrix}x_1\ x_2\ x_3\ ...\ x_n\end{bmatrix}$ 

And $B$ is just a diagonal matrix with all its diagonal elements as eigen values, i.e., $B=\lambda I,$ where $\lambda=[\lambda_1\ \lambda_2\dots\ \lambda_n],$ where $\lambda_1$ is the eigen value corresponding to eigen vector $x_1$ and so on.