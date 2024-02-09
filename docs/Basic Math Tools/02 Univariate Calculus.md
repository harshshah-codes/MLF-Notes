# Univariate Calculus

A univariate function is defined as $f:\R\to\R$

## Continuity of a univariate function $f$

A function $f:\R\to\R$ is continous if the $lim_x\to x^* f(x)$ exists and is equal to $f(x^*)$.

!!! tip

    If there are no sudden breaks in the graph or the graph does not break in the domain specified than the function is **continous** in the specified domain.

## Differentiability of a univariate function $f$

A function $f:\R\to\R$ is differentiable if the $f'(x^*) = lim_{h\to 0} \frac{f(x^*+h)-f(x^*)}{h}$ exists.

!!! warning

    If $f$ is not continous at $x^*$, then the function is not differentiable at $x^*$.
    But if a function is not differentiable at $x^*$,then it is not necessary that the function is not continous at $x^*$.

!!! tip

    If the graph of the function has no sudden breaks or no sharp corners in the specified domain, then the function is **differentiable** in the specified domain.

## Derivatives and Linear Approximation of a function $f$

Let $f:\R\to\R$ be a differentiable function.

Then the derivate of the function $f$ at $x^*$ is defined as

$$
f'(x^*) = lim_{x\to x^*}\cfrac{f(x)-f(x^*)}{x-x^*}\\ \ \\
\text{Let } f'(x^*) \approx \cfrac{f(x)-f(x^*)}{x-x^*}\text{  (Around } x=x*)\\\ \\
f(x) \approx f(x^*)+f'(x*)(x-x^*)
$$.

Now $f(x^*)+f'(x*)(x-x^*)$ is known as linear approximation $L_{x^*}[f](x)$ of $x$ around $x=x^*$.

!!! tip Remember

    $f(x)\approx L_{x^*}[f](x) $, where $ L_{x^*}[f](x) =f(x^*)+f'(x*)(x-x^*)$

## Linear Approximations And Tangent Lines

Graph of $ L_{x^*}[f]$, i.e. $G_{ L_{x^*}[f]}$ is a tangent to the graph of $f$, i.e., $G_f$ at the point $(x^*,f(x^*))$

## Some rules and Advanced Applications

<!-- TODO -->
### Higher order Approximations

### Product Rule
Let $f(x) = g(x).h(x)$ and $x^*=0$. We need to find $f'(x)$.

Now, using linear approximation and approximating $g(x)$ and $f(x)$ **seprately**.
$$

f(x) \approx (g(0) + xg'(0))(h(0) + xh'(0))\\ \ \\
f(x) \approx g(0)h(0) + x[g'(0)h(0)+h'(0)g(0)]+x^2g'(0)h'(0) \dots (1)\\ \ \\ \ \\
\text{ We know that }, L_{x^{*}}[f](0) = f(0) + xf'(0)\dots(2)$$

Comparing $(1)$ with $(2)$ we get $f'(0) = g'(0)h(0) + g(0)h'(0)$

### Chain rule

Let $f(x) = g(h(x))$.

Now approximating $h(x)$ around $0$. We get, $f(x) \approx g(h(0) + xh'(0))$

Now approximating $g(x)$ around $h(0)$. We get, $f(x) \approx g(h(0)) + g'(h(0))h'(0)x \dots (1)$

We know that $L_{x^*}[f](0) = g(h(0))+f'(0)x \dots(2)$

Comparing $(1)$ and $(2)$, We get, $f'(0) = g'(h(0)).h'(0)$

## Maxima, Minima And Saddle Point
Since $L_{x^*}[f] = f(x^*)+f'(x^*)(x-x^*)$ and if $f'(x^*) = 0$, then the linear approximation of $f(x)$ becomes a constant and this happens only at either the maxima, minima or a saddle point.

Hence if $f'(x^*) = 0$, then $x^*$ is a critical point.