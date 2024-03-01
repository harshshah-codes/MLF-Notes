# Orthogonal Vectors and Subspaces

## Length of a vector
Let a vector $x$ be defined such that $x\in\R^n$
$$
\text{Length of vector }x=||x||=\sqrt{x_1^2+x_2^2+...x_n^2}
$$

## Orthogonality
Two vectors $x$ and $y$ are said to be orthogonal $(\perp)$, if $x^Ty=y^Tx=0$

!!! tip

    - $0$ vector is orthogonal to every vector $x$.
    - If there are $k$ mutually orthogonal vectors, then the set of that vectors are linearly independent.

## Orthonormal Vectors
Let two vectors $u,v\in\R^n$.

$u,v$ are said to be orthonormal, if they are both orthogonal and of unit length. Mathematically,

$$
u^Tv=v^Tu=0 \text{ and } ||u||=||v||=1
$$

## Orthogonal Subspaces

Let $U, V$ be vector subspaces.

$U,V$ are vector subspaces if $u^Tv=v^Tu=0$, where, $v\in V,u\in U$

## Orthogonal Subspaces and Fundamental Subspaces

### $R(A)\perp N(A)$
Let $x\in N(A)$, i.e., $Ax=0$ which is equal to
$$
\begin{bmatrix}
\text{row 1}\ \text{row 2}\ \text{row 3}\\
\end{bmatrix}
\begin{bmatrix}
x_1\\ x_2\\ x_3
\end{bmatrix}=
\begin{bmatrix}
0 \\ 0\\ 0
\end{bmatrix}
$$

The above equation implies $\text{(row 1)}\perp x_1, \text{(row 2)}\perp x_2, ...$ and so on.

Thus for any $x$, $\alpha_1r_1+\alpha_2r_2+...\alpha_nr_n\perp x,$ where $r_i$ is a $i^{th}$ row of the matrix.

So $R(A)\perp N(A)\implies C(A^T)\perp N(A)$

### $C(A)\perp N(A^T)$
> Try it yourself.

!!! tip

    Follow the previous proof with the Column Space and Left Null space.