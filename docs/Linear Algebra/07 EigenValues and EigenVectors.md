# Eigen Values and Eigen Vectors


## Eigen Values
Let us consider a matrix $A,$ a vector $v$ and a scalar $\lambda,$ if the matrix $A$ satisfies the equation,

$$
Av=\lambda v
$$

then, the values that $\lambda$ attains are known as **Eigen Values**.

### How to find Eigen Values?
To find eigen values, let us do some manipulation of the equation above,

$$
Av=\lambda v\newline
\to Av=\lambda Iv\newline
\to Av-\lambda Iv=0\newline
\to v(A-\lambda I) = 0
$$

So now for non trivial solutions of the equation above 👆, i.e., $v\neq0$ vector, we solve $A-\lambda I=0.$

The values of $\lambda$ thus obtained are **Eigen Values**

### Eigen Vectors
Now as we have learnt about [*Eigen Values*](#eigen-values) we will now learn about **Eigen Vectors**.

Eigen vectors are basically the values of vector $v$ corresponding to each eigenvalue $\lambda,$ 

## Finding Eigen Vectors

After finding [*Eigen Values*](#how-to-find-eigen-values), put each value of $\lambda$ in the equation $Av=\lambda v$ or $(A-\lambda I)v=0$ and find the value of $v$

The values of $v$ thus obtained are the **eigen vectors** to your matrix $A$ corresponding to the [*eigen values*](#eigen-values) $\lambda.$

## Some Important Properties
1. The sum of the **eigen values** is equal to the *trace* of the matrix $A,$ i.e., $\sum\lambda=tr(A).$
2. The product of the **eigen values** is equal to the *determinant* of the matrix $A,$ i.e., $\prod\lambda=det(A).$
3. A quick and easy way to find out the eigen values is by using the first two properties.
4. Symmetric matrices have **real** eigenvalues.
5. There may be some matrices for which there may be repeated **eigen values**. 

## Importance of Eigen Values and Eigen Vectors
If $x$ is an **eigen vector**, then $A$ either ***extends it or shrinks it*** by the scale of $\lambda$

This has been gracefully demonstrated by the professor in the lecture and if you prefer an animated version of the same, here is a great video by [3blue1brown](https://www.youtube.com/@3blue1brown)

<iframe width="850" height="669" src="https://www.youtube.com/embed/PFDu9oVAE-g" title="Eigenvectors and eigenvalues | Chapter 14, Essence of linear algebra" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>