# Least Squares and Projections

Let us say that there is a system of equations $Ax=b$ and the vector $b$ leads to an inconsistent system.

Let the data be of the form $(x_1,b_1),(x_2,b_2)...(x_n,b_n)$

Now we want to solve this system, so what we could do is find out the errors and try to **minimise** them.

Thus my squared error is $E^2=(b_1-x_1)^2+(b_2-x_2)^2...+(b_n-x_n)^2$
If we try to minimise it using calculus, i.e., $\cfrac{d E^2}{d x}=0$

$$
\cfrac{d E^2}{d x}=0
\\\ \\\rightarrow 2[2(b_1-\cfrac{dx_1}{dx})+2(b_2-\cfrac{dx_2}{dx})+...+2(b_n-\cfrac{dx_n}{dx})] = 0
\\\ \\\rightarrow \text{On solving, this looks similar to, }\cfrac{a^Tb}{a^Ta}
$$

!!! note

    Taking derivative and finding the **minima** actually turns out to be the same as peforming [*a projection* on a subspace](./03%20Projections.md/#projection-onto-a-subspace). Solving $A^TA\hat{x}=A^Tb$ leads to an $\hat{x}$ that minimises $||Ax-b||^2$




