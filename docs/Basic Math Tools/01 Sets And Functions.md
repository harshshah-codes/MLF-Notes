# Sets and Functions

## Some important symbols

|                   |              |
| :---------------: | ------------ |
|    $\implies$     | Implies      |
|     $\forall$     | For All      |
|     $\exists$     | There exists |
| $\Leftrightarrow$ | Equivalence  |

## Sets

### Some basic sets to remember

- $\R \to $ Set of Real Numbers
- $\R_+ \to $ Set of Positive Real numbers (including $0$)
- $\Z \to$ Set of all integers
- $\Z_+ \to$ Set of positive integers including $0$
- $[a,b] \to \{x\in\R\ |\ a\leq x\leq b\}$
- $(a,b) \to \{x\in\R\ |\ a< x< b\}$
- $\R^d \to $  Set of $d$-dimensional vectors
- $[a,b]^d \to \{x\in\R^d:x_i\in[a,b], i\in\{1,2,3,\dots d\}\}$

### Metric Spaces

**Metric spaces** are basically vectors with some **Distance function $D$** associated with them.

For most of question throughout the course the default metric space used is $\R^d$ where $D=\sqrt{(x_1-y_1)^2+(x_2-y_2)^2+\dots(x_d-y_d)^2}$,

#### Open ball in Metric Space

Let $x\in\R^d$. Then, the open ball is given by $B(x,\epsilon)=\{y\in\R^d: D(x,y)<\epsilon\}$

#### Closed ball in Metric Space

Let $x\in\R^d$. Then, the closed ball is given by $B(x,\epsilon)=\{y\in\R^d: D(x,y)\leq\epsilon\}$

!!! tip

    If you include the boundary, it is a **closed ball**, else an **open ball**.

## Sets

Sets are basically a collection of objects.

Some basic operations defined on sets are

- Union ($\cup$)
- Intersection ($\cap$)
- Complement ($S^{c}$)
- $A-B$

### Union ($\cup$)

The union of two sets $A$ and $B$ is the set of elements which are in $A$, as well as in $B$ or in both.

### Intersection ($\cap$)

The intersection of two sets $A$ and $B$ is the set of elements which are in both $A$ and $B$.

### Complement ($S^{c}$)

The complement of a set $S$ is the set of all elements which are in the universal set but not in $S$.

### $A-B$

This contains all the elements of $A$ that are not in $B$.

### De Morgan's Law

Let there be two sets $A$ and $B$. Then, the De-Morgan's Law states that,

- $(A\cup B)^{c}=A^c\cap B^c$
- $(A\cap B)^{c}=A^c\cup B^c$
