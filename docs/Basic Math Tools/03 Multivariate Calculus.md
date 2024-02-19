# Multivariate Calculus

Let a function $f$ be defined as $f:\R^d\to\R$. This will be used to reference each multivariate function described in this article.

## Lines
- A line in $\R^d$ is a subset of $\R^d$
- A line through point $u\in\R^d$ along the vector $x\in\R^d$ is given by $\{x\in\R^d: x= u +\alpha v, \alpha\in\R\}$
- A line through two points $u,u'\in\R^d$ is given by $\{x\in\R^d:x=u+\alpha(u-u'), \alpha\in\R\}$

## Hyper Plane
- A hyperplane of $d-1$ dimensions $\subseteq R^d$.
- A hyperplane perpendicular to a vector $w\in\R^d$ with a value $b\in\R$ is given by $\{x\in\R^d:w^Tx=b\} = \{x\in\R^d:\sum_{i=1}^dw_ix_i=b\}$ 

## Partial Derivatives
The partial derivative of $f$ is defined as the derivative of $f$ with respect to one of the variables, keeping the other variables constant, i.e.,

$$
\cfrac{\partial f}{\partial x_i}(v) = lim_{\alpha\to{0}}\cfrac{f(v+\alpha e_i)-f(v)}{\alpha}
$$
Here $e_i$ is the $i^{th}$ unit vector in $\R^d$

Let $f:\R^d\to\R$ and $f=1x_1+2x_2+\dots nx_n$

Then the partial derivative of $f$ 
- with respect to the variable $x_1$ is 
$$
\cfrac{\partial f}{\partial x_1} = 1
$$
- with respect to the variable $x_2$ is 
$$
\cfrac{\partial f}{\partial x_2} = 2
\\\ \\\vdots
$$
and so on

## Gradients

Let $f:\R^d\to\R$ be defined.

Then $\cfrac{\partial f}{\partial x} = \begin{bmatrix}\cfrac{\partial f}{\partial x_1},\cfrac{\partial f}{\partial x_2}, \cfrac{\partial f}{\partial x_3}, \cfrac{\partial f}{\partial x_4}, \cfrac{\partial f}{\partial x_5}, \dots, \cfrac{\partial f}{\partial x_d}, \end{bmatrix}$

Hence the gradient is equal to $[\cfrac{\partial f}{\partial x}]^T$, i.e.,
$$
\cfrac{\triangledown f}{\triangledown x} = \begin{bmatrix}
\cfrac{\partial f}{\partial x_1}\\\ \\
\cfrac{\partial f}{\partial x_2}\\ \ \\
\vdots\\\ \\\
\cfrac{\partial f}{\partial x_n}
\end{bmatrix}
$$

### Linear Approximations and Gradients
Let $f$ be a function defined from $\R^d\to\R$

Then the linear approximation of $f$ at a vector $v\in\R^d$ is given by, 

$$
L_v[f](x)= f(x) = f(v) + \triangledown f(v)^T(x-v)
$$

### Gradients and Tangent Planes
The graph of $L_v[f]$ is a plane that is tangent to the graph of $f$ at the point $(v, f(v))$


### Gradients and Contours
The gradient of $f$ evaluated at $v$ is $\perp$ to the level set of $f.$ Mathematically,

$$
\triangledown f(v) \perp \{x\in\R^d:f(x)=f(v)\}
$$

#### Proof
$$
\{x\in\R^d:f(x)=f(v)\}\newline
\ \newline
\rightarrow\{x\in\R^d:L_v[f](x)=f(v)\}\newline
\ \newline
\rightarrow\{x\in\R^d:f(v)+\triangledown f(v)^T(x-v)=f(v)\}\newline
\ \newline

\rightarrow  \{x\in\R^d:\triangledown f(v)^Tx=\triangledown f(v)^Tv\}\newline
\ \newline
\text{Comparing with } \{x\in\R^d:W^Tx=b\}, \text{where W is }\perp\text{to the plane}\newline\ \newline
\therefore \triangledown f(v) \perp \{x\in\R^d:L_v[f](x)=f(v)\}
$$

## Directional Derivative


The directional derivative of the function $f$ at the point $v$ along the direction of $u$ is given by,

$$
D_u[f](v) = lim_{\alpha\to 0} \cfrac{f(v+\alpha u)-f(v)}{\alpha}\newline\ \newline=lim_{\alpha\to 0} \cfrac{L_v[f](v)-f(v)}{\alpha}\newline\ \newline=lim_{\alpha\to 0} \cfrac{f(v)+\triangledown f(v)^T(\alpha u)-f(v)}{\alpha}\newline\ \newline=\triangledown f(v)^Tu
$$

## Cauchy-Schwarz Inequality

Let $a,b\in\R^d$. Then the equality states that

$$
-||a||.||b|| \leq a^Tb \leq ||a||.||b||
$$

### Points to Note
1. $-||a||.||b|| = a^Tb$, if and only if, $a=\alpha b$ and $a<0$
2. $||a||.||b|| = a^Tb$, if and only if, $a=\alpha b$ and $a>0$

## Direction of steepest ascent

For a function $f$, the direction of a unit vector $u$ such that it maximises the directional derivative of $f$ along $u$ is $u=\triangledown f(v)$, i.e., for steepest ascent $u$ should be in direction of $\triangledown f$

## Direction of steepest descent

For a function $f$, the direction of a unit vector $u$ such that it minimises the directional derivative of $f$ along $u$ is $u=-\triangledown f(v)$, i.e., for steepest descent $u$ should be in direction opposite to $\triangledown f$