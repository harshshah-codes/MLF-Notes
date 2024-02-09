# Sets and Functions

## Some important symbols

|      Symbol       | Used for     |
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

Some basic operations defined on sets are

- Union ($\cup$)
- Intersection ($\cap$)
- Complement ($S^{c}$)
- $A-B$

#### Union ($\cup$)

The union of two sets $A$ and $B$ is the set of elements which are in $A$, as well as in $B$ or in both.

#### Intersection ($\cap$)

The intersection of two sets $A$ and $B$ is the set of elements which are in both $A$ and $B$.

#### Complement ($S^{c}$)

The complement of a set $S$ is the set of all elements which are in the universal set but not in $S$.

#### $A-B$

This contains all the elements of $A$ that are not in $B$.

#### De Morgan's Law

Let there be two sets $A$ and $B$. Then, the De-Morgan's Law states that,

- $(A\cup B)^{c}=A^c\cap B^c$
- $(A\cap B)^{c}=A^c\cup B^c$

### Sequences

An **ordered collection** of elements is known as a **sequence**.

Let there be a sequence where the elements are $x_1,x_2,...$, where $x_i\in\R^d$. And, if $lim_{i\to\infin} x^i = x^*$ then, $\forall\text{  } \epsilon>0, \exists \text{ a }N, \text{ such that } x_n\in B(x^*, \epsilon)\ \forall\ n\geq N$

### Vector Spaces

A **vector space** is a set of elements called **vectors**, having operations of addition and scalar multiplication defined on it.

A vector space must satisfy the following properties:

- **Additive Closure**: If the vector space is $V$ and $v_1,v_2\in V$, then
$c_1v_1 + c_2v_2\in V$, where $c_1,c_2\in \R$
<!-- TODO -->
- **Multiplative Closure**

#### Dot Product of two vectors

Let $x$ and $y$ be two vectors such that $x,y\in\R^d$.
Then, $x.y=x^Ty=\sum_{i=1}^dx_i.y_i$

#### Norm of a vector

Let $x$ be a vector such that $x\in\R^d$.
Then, the norm of the vector is given by $||x||=\sqrt{x^Tx}=\sqrt{\sum_{i=1}^dx_i^2}$

#### Orthognal Vectors

Let $x$ and $y$ be two vectors such that $x,y\in\R^d$.
Then, $x$ and $y$ are orthogonal if $x.y=0$, i.e., $x^Ty=0$

## Functions And Graphs

Let $f$ be a function with domain $A$ and co-domain $B$. Then, the function is denoted as $f:A\to B$.

### $d$-dimensional functions

A function with domain $\R^d$ to $\R$ is known as a $d$-dimensional function or multivariate function.

It is denoted as $f:\R^d\to\R$

### Graph of a function $f$

The graph of a $d$-dimensional function is defined as $G_f \subseteq \R^{d+1}$.

$$
G_f=\{(x, f(x)): x\in\R^d\}
$$
