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
$$
