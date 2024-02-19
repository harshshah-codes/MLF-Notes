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