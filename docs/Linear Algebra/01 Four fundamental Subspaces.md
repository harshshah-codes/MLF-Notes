# Four Fundamental Subspaces

In this article, we discuss about the four fundamental subspaces related to a matrix. They are
- Column space
- Row Space
- Null Space
- 

## Column Space $C(A)$
Let a matrix $A$ consists of columns $u_1,u_2,\dots u_n$. Then $C(A) = \text{span}(u_1,u_2,u_3\dots u_n)$

### Solving $Ax=b$ using $C(A)$

$A(x)=b$ is solvable if and only if $b\in C(A)$

Let us look at an example to see how we use the $C(A)$ to solve $Ax=b$


$$
\text{Let }A = \begin{bmatrix} 1\ 1\ 2\newline2\ 1\ 3\newline3\ 1\ 4\newline 4\ 1\ 5 \end{bmatrix}
$$

> Is $Ax=b$ solvable? No, because $C(A)=\text{span}(C_1, C_2)$ and $C_3 = C_1+C_2$  whereas the variables are only $3$. Hence there are $4$ equations and $3$ unknowns and $C(A)$ is a 2-dimensional subspace of $\R^4.$

## Row space
The row space of a matrix $A$ is defined as column space of $A^T$, i.e., $R(A)=C(A^T)$

!!! note

    Column Rank $=$ Row Rank


## Null Space

Null space of a matrix $A$ is defined as $N(A)=\{x|Ax=0\}$

!!! Remember

    If $A$ is invertible matrix, then $N(A) = 0$ and $C(A)$ is the entire space. It so happens that $Ax=b$ has a unique solution $x=A^{-1}b$

!!! tip

    We can also use the Gaussian elimination to find the null space of a matrix $A.$ 
    
### Rank Nullity Theorem

In the gaussian elimination, the number of pivot columns is called the **Rank** of the matrix, i.e., Rank $=$ Dim $(C(A)).$

And the number of free variables is known as **Nulity** of the matrix, i.e., Nullity $=$ Dim $(N(A)).$

Now according to the theorem, if $A$ has $n$ columns, then
$$
n=\text{Rank} + \text{Nullity}
$$

## Left Null Space
The **Left Null Space** of a matrix $A$ is defined as the null space of $A^T.$

$$
\text{Left Null Space}=\{y|A^Ty=0\}=\{y|y^TA=0\}
$$

!!! tip

    Row Space $+$ Left Null Space $=$ Row Space