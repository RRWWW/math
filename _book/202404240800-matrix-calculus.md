# matrix calculus

[@ccjou2013]

$$
\boldsymbol{x}=\left\langle x_{1},x_{2},\cdots,x_{n}\right\rangle =\begin{bmatrix}x_{1} & x_{2} & \cdots & x_{n}\end{bmatrix}^{\intercal}=\begin{bmatrix}x_{1}\\
x_{2}\\
\vdots\\
x_{n}
\end{bmatrix}
$$

$$
f\left(x_{1},x_{2},\cdots,x_{n}\right)=f\left(\left\langle x_{1},x_{2},\cdots,x_{n}\right\rangle \right)=f\left(\boldsymbol{x}\right)
$$
$$
\boldsymbol{y}=\left\langle y_{1},y_{2},\cdots,y_{m}\right\rangle =\begin{bmatrix}y_{1} & y_{2} & \cdots & y_{m}\end{bmatrix}^{\intercal}=\begin{bmatrix}y_{1}\\
y_{2}\\
\vdots\\
y_{m}
\end{bmatrix}
$$

## vector-by-scalar

$$
\dfrac{\partial\boldsymbol{y}}{\partial x}=\left[\begin{array}{c}
\dfrac{\partial y_{1}}{\partial x}\\
\dfrac{\partial y_{2}}{\partial x}\\
\vdots\\
\dfrac{\partial y_{m}}{\partial x}
\end{array}\right]
$$

## scalar-by-vector

$$
\boldsymbol{\nabla}f=\dfrac{\partial}{\partial\boldsymbol{x}}f=\dfrac{\partial f}{\partial\boldsymbol{x}}=\left\langle \dfrac{\partial f}{\partial x_{1}},\dfrac{\partial f}{\partial x_{2}},\cdots,\dfrac{\partial f}{\partial x_{n}}\right\rangle =\begin{bmatrix}\dfrac{\partial f}{\partial x_{1}} & \dfrac{\partial f}{\partial x_{2}} & \cdots & \dfrac{\partial f}{\partial x_{n}}\end{bmatrix}^{\intercal}=\begin{bmatrix}\dfrac{\partial f}{\partial x_{1}}\\
\dfrac{\partial f}{\partial x_{2}}\\
\vdots\\
\dfrac{\partial f}{\partial x_{n}}
\end{bmatrix}
$$

$$
f_i = f_i\left(x_{1},x_{2},\cdots,x_{n}\right)=f_i\left(\boldsymbol{x}\right)
$$

$$
\boldsymbol{f}=\left\langle f_{1},f_{2},\cdots,f_{m}\right\rangle =\begin{bmatrix}f_{1} & f_{2} & \cdots & f_{m}\end{bmatrix}^{\intercal}=\begin{bmatrix}f_{1}\\
f_{2}\\
\vdots\\
f_{m}
\end{bmatrix}
$$

## vector-by-vector

### numerator-layout notation


::: {show-in="html"}
分子布局
:::

::: {show-in="pdf"}
\begin{CJK}{UTF8}{bsmi}
分子布局
\end{CJK}
:::

$$
\dfrac{\partial\boldsymbol{y}}{\partial\boldsymbol{x}}=\begin{bmatrix}\dfrac{\partial y_{1}}{\partial\boldsymbol{x}}\\
\dfrac{\partial y_{2}}{\partial\boldsymbol{x}}\\
\vdots\\
\dfrac{\partial y_{p}}{\partial\boldsymbol{x}}
\end{bmatrix}=\begin{bmatrix}\dfrac{\partial\boldsymbol{y}}{\partial x_{1}} & \dfrac{\partial\boldsymbol{y}}{\partial x_{2}} & \cdots & \dfrac{\partial\boldsymbol{y}}{\partial x_{n}}\end{bmatrix}=\begin{bmatrix}\dfrac{\partial y_{1}}{\partial x_{1}} & \dfrac{\partial y_{1}}{\partial x_{2}} & \cdots & \dfrac{\partial y_{1}}{\partial x_{n}}\\
\dfrac{\partial y_{2}}{\partial x_{1}} & \dfrac{\partial y_{2}}{\partial x_{2}} & \cdots & \dfrac{\partial y_{2}}{\partial x_{n}}\\
\vdots & \vdots & \ddots & \vdots\\
\dfrac{\partial y_{m}}{\partial x_{1}} & \dfrac{\partial y_{m}}{\partial x_{2}} & \cdots & \dfrac{\partial y_{m}}{\partial x_{n}}
\end{bmatrix}=\left[\dfrac{\partial y_{i}}{\partial x_{j}}\right]_{m\times n}
$$

### denominator-layout notation 

::: {show-in="html"}
分母布局
:::

::: {show-in="pdf"}
\begin{CJK}{UTF8}{bsmi}
分母布局
\end{CJK}
:::

$$
\dfrac{\partial\boldsymbol{y}}{\partial\boldsymbol{x}}=\begin{bmatrix}\dfrac{\partial\boldsymbol{y}}{\partial x_{1}}\\
\dfrac{\partial\boldsymbol{y}}{\partial x_{2}}\\
\vdots\\
\dfrac{\partial\boldsymbol{y}}{\partial x_{n}}
\end{bmatrix}=\begin{bmatrix}\dfrac{\partial y_{1}}{\partial\boldsymbol{x}} & \dfrac{\partial y_{2}}{\partial\boldsymbol{x}} & \cdots & \dfrac{\partial y_{m}}{\partial\boldsymbol{x}}\end{bmatrix}=\begin{bmatrix}\dfrac{\partial y_{1}}{\partial x_{1}} & \dfrac{\partial y_{2}}{\partial x_{1}} & \cdots & \dfrac{\partial y_{m}}{\partial x_{1}}\\
\dfrac{\partial y_{1}}{\partial x_{2}} & \dfrac{\partial y_{2}}{\partial x_{2}} & \cdots & \dfrac{\partial y_{m}}{\partial x_{2}}\\
\vdots & \vdots & \ddots & \vdots\\
\dfrac{\partial y_{1}}{\partial x_{n}} & \dfrac{\partial y_{2}}{\partial x_{n}} & \cdots & \dfrac{\partial y_{m}}{\partial x_{n}}
\end{bmatrix}=\left[\dfrac{\partial y_{j}}{\partial x_{i}}\right]_{n\times m}
$$