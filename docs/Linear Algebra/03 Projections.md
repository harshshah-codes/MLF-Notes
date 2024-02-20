# Projections of Vectors

## Motivation

You might have this question that **What is the need of projection?**

Let us say we are given some data $(x_1,b_1),(x_2,b_2),...(x_n,b_n)$ and it is given that this does not have a solution, i.e., $b\notin C(A).$ At this point, it makes sense to get a projection of $b$ onto $A$.

## Projecting a vector $b$ onto $a$

![Projections](../assets/Projection.png)

$$
\text{We know, }p = \hat{x}a\newline \text{ and } E=b-a\rightarrow E=b-\hat{x}a\\\text{ and } E\perp a \rightarrow b-\hat{x}a\perp a
\\ \rightarrow a(b-\hat{x}a) = 0\\ \rightarrow \hat{x} = \cfrac{a^Tb}{a^Ta}\\
\ \\
\text{Since, }p=\hat{x}a\\\text{Hence, } p = \cfrac{a^Tb}{a^Ta}a
$$

## Projection Matrix $P$
We know $p = \cfrac{a^Tb}{a^Ta}a = \cfrac{aa^T}{a^Ta}b$

Then the Projection Matrix $P=\cfrac{aa^T}{a^Ta}$ and the projection of $b$ onto $a$ is $Pa.$

### Important Observations
1. $P$ is always symmetric.
2. $P^2=P, \text{ i.e, }P^2b=Pb$
3. Column space of $P =$ line through $a$ 
4. Null space of $P=$ plane $\perp a$
5. Rank $P=1$