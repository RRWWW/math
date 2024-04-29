# machine learning

## Shai Ben-David

https://www.youtube.com/playlist?list=PLPW2keNyw-usgvmR7FTQ3ZRjfLs5jT4BO

## deep learning

::: {show-in="html"}
### 我妻幸長
:::

::: {show-in="pdf"}
\begin{CJK}{UTF8}{bsmi}
我妻幸長
\end{CJK}
:::

Esc = Einstein summation convention

$$
\begin{aligned}
W\boldsymbol{x}= & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\begin{pmatrix}\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}\overset{\text{Esc}}{=}\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}\\
\boldsymbol{y}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=y_{{\scriptscriptstyle \mu}}= & w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=W\boldsymbol{x}\\
\boldsymbol{y}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=y_{{\scriptscriptstyle \mu}}^{\intercal}= & \left(w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}\right)^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=\left[\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}\right]^{\intercal}=\left[W\boldsymbol{x}\right]^{\intercal}\\
= & x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\boldsymbol{x}^{\intercal}W^{\intercal}\\
\boldsymbol{x}^{\intercal}W^{\intercal}=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}=y_{{\scriptscriptstyle \mu}}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=\boldsymbol{y}^{\intercal}
\end{aligned}
$$

***

$$
\begin{aligned}
W\boldsymbol{x}= & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\begin{pmatrix}\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}\overset{\text{Esc}}{=}\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=W\boldsymbol{x}= & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+\sum\limits _{j=1}^{n}w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+\sum\limits _{j=1}^{n}w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+\sum\limits _{j=1}^{n}w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}\overset{\text{Esc}}{=}\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=b_{{\scriptscriptstyle \mu}}+w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}\\
\boldsymbol{y}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=y_{{\scriptscriptstyle \mu}}= & w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=W\boldsymbol{x},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\boldsymbol{y}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=y_{{\scriptscriptstyle \mu}}= & w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=W\boldsymbol{x},\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\boldsymbol{y}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=y_{{\scriptscriptstyle \mu}}^{\intercal}= & \left(w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}\right)^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=\left[\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}\right]^{\intercal}=\left[W\boldsymbol{x}\right]^{\intercal}\\
= & x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\boldsymbol{x}^{\intercal}W^{\intercal},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
= & b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle \mu j}}^{\intercal}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal}\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\boldsymbol{x}^{\intercal}W^{\intercal}\\
\boldsymbol{x}^{\intercal}W^{\intercal}=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}=y_{{\scriptscriptstyle \mu}}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=\boldsymbol{y}^{\intercal}\\
\boldsymbol{x}^{\intercal}W^{\intercal}=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}=b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle \mu j}}^{\intercal}=y_{{\scriptscriptstyle \mu}}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=\boldsymbol{y}^{\intercal}
\end{aligned}
$$

***

$$
\begin{aligned}
W\boldsymbol{x}= & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\begin{pmatrix}\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
\sum\limits _{\nu=0}^{n}w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}\overset{\text{Esc}}{=}\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=W\boldsymbol{x}= & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+\sum\limits _{j=1}^{n}w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+\sum\limits _{j=1}^{n}w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+\sum\limits _{j=1}^{n}w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}\overset{\text{Esc}}{=}\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=b_{{\scriptscriptstyle \mu}}+w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}\\
\boldsymbol{y}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=y_{{\scriptscriptstyle \mu}}= & w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=W\boldsymbol{x},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\boldsymbol{y}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=y_{{\scriptscriptstyle \mu}}= & w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=W\boldsymbol{x},\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\boldsymbol{y}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=y_{{\scriptscriptstyle \mu}}^{\intercal}= & \left(w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}\right)^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=\left[\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}\right]^{\intercal}=\left[W\boldsymbol{x}\right]^{\intercal}\\
= & x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\boldsymbol{x}^{\intercal}W^{\intercal}\\
= & b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle \mu j}}^{\intercal}=b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal}\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\\
\boldsymbol{x}^{\intercal}W^{\intercal}=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=\boldsymbol{y}^{\intercal}\\
\boldsymbol{x}^{\intercal}W^{\intercal}=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}=b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}
\end{aligned}
$$

***

$$
\begin{aligned}
\boldsymbol{y}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=y_{{\scriptscriptstyle \mu}}= & w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=W\boldsymbol{x},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\boldsymbol{y}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=y_{{\scriptscriptstyle \mu}}= & w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=W\boldsymbol{x},\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\boldsymbol{x}^{\intercal}W^{\intercal}=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=\boldsymbol{y}^{\intercal}\\
=\boldsymbol{x}^{\intercal}W^{\intercal}=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}=b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}=\boldsymbol{y}^{\intercal}
\end{aligned}
$$

***

$$
\begin{aligned}
\sigma\left(\boldsymbol{y}\right)=\sigma\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma\left(y_{{\scriptscriptstyle \mu}}\right)= & \sigma\left(w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}\right)=\sigma\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\sigma\left(\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}\right)=\sigma\left(W\boldsymbol{x}\right),\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\sigma\left(\boldsymbol{y}\right)=\sigma\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma\left(y_{{\scriptscriptstyle \mu}}\right)= & \sigma\left(w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}\right)=\sigma\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\sigma\left(\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}\right)=\sigma\left(W\boldsymbol{x}\right),\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\left(\boldsymbol{x}^{\intercal}W^{\intercal}\right)\varsigma=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}\varsigma=\left(x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}\right)\varsigma=\left(x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}\right)\varsigma=\left(y_{{\scriptscriptstyle \mu}}^{\intercal}\right)\varsigma=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma=\left(\boldsymbol{y}^{\intercal}\right)\varsigma\\
=\left(\boldsymbol{x}^{\intercal}W^{\intercal}\right)\varsigma=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}\varsigma=\left(b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}\right)\varsigma=\left(y_{{\scriptscriptstyle \mu}}^{\intercal}\right)\varsigma=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma=\left(\boldsymbol{y}^{\intercal}\right)\varsigma
\end{aligned}
$$

***

$$
\begin{aligned}
\sigma\left(\boldsymbol{y}\right)=\sigma\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma\left(y_{{\scriptscriptstyle \mu}}\right)= & \sigma\left(w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}\right)=\sigma\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\sigma\left(\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}\right)=\sigma\left(W\boldsymbol{x}\right),\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\sigma\boldsymbol{y}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma_{{\scriptscriptstyle \mu}}y_{{\scriptscriptstyle \mu}}= & \sigma_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\sigma\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\sigma W\boldsymbol{x},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\sigma\left(\boldsymbol{y}\right)=\sigma\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma\left(y_{{\scriptscriptstyle \mu}}\right)= & \sigma\left(w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}\right)=\sigma\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\sigma\left(\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}\right)=\sigma\left(W\boldsymbol{x}\right),\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
=\sigma\boldsymbol{y}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma_{{\scriptscriptstyle \mu}}y_{{\scriptscriptstyle \mu}}= & \sigma_{{\scriptscriptstyle \mu}}\left(w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}\right)=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\sigma\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\sigma W\boldsymbol{x},\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\left(\boldsymbol{x}^{\intercal}W^{\intercal}\right)\varsigma=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}\varsigma=\left(x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}\right)\varsigma=\left(x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}\right)\varsigma=\left(y_{{\scriptscriptstyle \mu}}^{\intercal}\right)\varsigma=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma=\left(\boldsymbol{y}^{\intercal}\right)\varsigma\\
=\boldsymbol{x}^{\intercal}W^{\intercal}\varsigma=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}\varsigma=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}\varsigma_{{\scriptscriptstyle \mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\boldsymbol{y}^{\intercal}\varsigma\\
=\left(\boldsymbol{x}^{\intercal}W^{\intercal}\right)\varsigma=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}\varsigma=\left(b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}\right)\varsigma=\left(y_{{\scriptscriptstyle \mu}}^{\intercal}\right)\varsigma=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma=\left(\boldsymbol{y}^{\intercal}\right)\varsigma\\
=\boldsymbol{x}^{\intercal}W^{\intercal}\varsigma=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}\varsigma=\left(b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}\right)\varsigma_{{\scriptscriptstyle \mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\boldsymbol{y}^{\intercal}\varsigma
\end{aligned}
$$

***

$$
\begin{aligned}
\sigma\boldsymbol{y}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma_{{\scriptscriptstyle \mu}}y_{{\scriptscriptstyle \mu}}= & \sigma_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\sigma\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\sigma W\boldsymbol{x},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\sigma\boldsymbol{y}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma_{{\scriptscriptstyle \mu}}y_{{\scriptscriptstyle \mu}}= & \sigma_{{\scriptscriptstyle \mu}}\left(w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}\right)=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\sigma\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\sigma W\boldsymbol{x},\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\boldsymbol{x}^{\intercal}W^{\intercal}\varsigma=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}\varsigma=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}\varsigma_{{\scriptscriptstyle \mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\boldsymbol{y}^{\intercal}\varsigma\\
=\boldsymbol{x}^{\intercal}W^{\intercal}\varsigma=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}\varsigma=\left(b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}\right)\varsigma_{{\scriptscriptstyle \mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\boldsymbol{y}^{\intercal}\varsigma
\end{aligned}
$$

***

$$
\begin{aligned}
\boldsymbol{z}=\sigma\boldsymbol{y}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma_{{\scriptscriptstyle \mu}}y_{{\scriptscriptstyle \mu}}= & \sigma_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}=\sigma\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\sigma W\boldsymbol{x},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=\boldsymbol{z}=z_{{\scriptscriptstyle \mu}}=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle \mu}}
\end{pmatrix}=\sigma_{{\scriptscriptstyle \mu}}y_{{\scriptscriptstyle \mu}}= & \sigma_{{\scriptscriptstyle \mu}}\left(w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}\right)=\sigma_{{\scriptscriptstyle \mu}}\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}=\sigma\begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}=\sigma W\boldsymbol{x},\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\boldsymbol{x}^{\intercal}W^{\intercal}\varsigma=\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}w_{{\scriptscriptstyle 0\nu}}x_{{\scriptscriptstyle \nu}}\\
w_{{\scriptscriptstyle 1\nu}}x_{{\scriptscriptstyle \nu}}\\
\vdots\\
w_{{\scriptscriptstyle m\nu}}x_{{\scriptscriptstyle \nu}}
\end{pmatrix}^{\intercal}\varsigma=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}\varsigma_{{\scriptscriptstyle \mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\boldsymbol{y}^{\intercal}\varsigma=\boldsymbol{z}^{\intercal}\\
=\boldsymbol{x}^{\intercal}W^{\intercal}\varsigma=\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal} & \begin{pmatrix}b_{{\scriptscriptstyle 0}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
b_{{\scriptscriptstyle 1}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
b_{{\scriptscriptstyle m}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}^{\intercal}\varsigma=\begin{pmatrix}b_{{\scriptscriptstyle 0}}+w_{{\scriptscriptstyle 0j}}x_{{\scriptscriptstyle j}}\\
b_{{\scriptscriptstyle 1}}+w_{{\scriptscriptstyle 1j}}x_{{\scriptscriptstyle j}}\\
\vdots\\
b_{{\scriptscriptstyle m}}+w_{{\scriptscriptstyle mj}}x_{{\scriptscriptstyle j}}
\end{pmatrix}^{\intercal}\varsigma=\left(b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}\right)\varsigma_{{\scriptscriptstyle \mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=\begin{pmatrix}y_{{\scriptscriptstyle 0}}\\
y_{{\scriptscriptstyle 1}}\\
\vdots\\
y_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=z_{{\scriptscriptstyle \mu}}^{\intercal}=\boldsymbol{z}^{\intercal}
\end{aligned}
$$

***

$$
\begin{aligned}
\boldsymbol{z}= & \sigma\boldsymbol{y}=\sigma_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu\nu}}x_{{\scriptscriptstyle \nu}}=\sigma W\boldsymbol{x},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle \mu0}}=b_{{\scriptscriptstyle \mu}}
\end{cases}\\
=z_{{\scriptscriptstyle \mu}}= & \sigma_{{\scriptscriptstyle \mu}}y_{{\scriptscriptstyle \mu}}=\sigma_{{\scriptscriptstyle \mu}}\left(w_{{\scriptscriptstyle \mu j}}x_{{\scriptscriptstyle j}}+b_{{\scriptscriptstyle \mu}}\right),\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \mu}}=w_{{\scriptscriptstyle \mu0}}
\end{cases}\\
\boldsymbol{x}^{\intercal}W^{\intercal}\varsigma= & x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=x_{{\scriptscriptstyle \nu}}^{\intercal}w_{{\scriptscriptstyle \nu\mu}}\varsigma_{{\scriptscriptstyle \mu}}=\boldsymbol{y}^{\intercal}\varsigma=\boldsymbol{z}^{\intercal}\\
= & \left(b_{{\scriptscriptstyle \mu}}^{\intercal}+x_{{\scriptscriptstyle j}}^{\intercal}w_{{\scriptscriptstyle j\mu}}\right)\varsigma_{{\scriptscriptstyle \mu}}=y_{{\scriptscriptstyle \mu}}^{\intercal}\varsigma_{{\scriptscriptstyle \mu}}=z_{{\scriptscriptstyle \mu}}^{\intercal}
\end{aligned}
$$

***

[matrix calculus]^[\@ref(matrix-calculus)]^

4-15

wrong or incompatible transpose

$$
\begin{aligned}
\boldsymbol{x}^{\intercal}W= & \begin{pmatrix}x_{{\scriptscriptstyle 0}} & x_{{\scriptscriptstyle 1}} & \cdots & x_{{\scriptscriptstyle m}}\end{pmatrix}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\\
= & \begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}=\begin{pmatrix}\sum\limits _{\mu=1}^{m}x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu0}}\\
\sum\limits _{\mu=1}^{m}x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu1}}\\
\vdots\\
\sum\limits _{\mu=1}^{m}x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu n}}
\end{pmatrix}^{\intercal}\\
\overset{\text{Einstein summation convention}}{=} & \begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}=\begin{pmatrix}x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu0}}\\
x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu1}}\\
\vdots\\
x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu n}}
\end{pmatrix}^{\intercal}\\
= & x_{{\scriptscriptstyle \mu}}^{\intercal}w_{{\scriptscriptstyle \mu\nu}}=\left(x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu\nu}}\right)^{\intercal}?
\end{aligned}
$$

4-18

wrong or incompatible transpose

$$
\begin{aligned}
\boldsymbol{x}^{\intercal}W= & \begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}=\begin{pmatrix}x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu0}}\\
x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu1}}\\
\vdots\\
x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu n}}
\end{pmatrix}^{\intercal},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle 0\nu}}=b_{{\scriptscriptstyle \nu}}
\end{cases}\\
= & \begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\begin{pmatrix}b_{{\scriptscriptstyle 0}} & b_{{\scriptscriptstyle 1}} & \cdots & b_{{\scriptscriptstyle n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}=\begin{pmatrix}x_{{\scriptscriptstyle i}}w_{{\scriptscriptstyle i0}}+b_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle i}}w_{{\scriptscriptstyle i1}}+b_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{i}w_{{\scriptscriptstyle in}}+b_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal},\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \nu}}=w_{{\scriptscriptstyle 0\nu}}
\end{cases}
\end{aligned}
$$

wrong or incompatible transpose

$$
\begin{aligned}
\sigma\left(\boldsymbol{x}^{\intercal}W\right)= & \sigma\left(\begin{pmatrix}x_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\begin{pmatrix}w_{{\scriptscriptstyle 00}} & w_{{\scriptscriptstyle 01}} & \cdots & w_{{\scriptscriptstyle 0n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\right)=\sigma\left(\begin{pmatrix}x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu0}}\\
x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu1}}\\
\vdots\\
x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu n}}
\end{pmatrix}^{\intercal}\right)=\begin{pmatrix}\sigma_{{\scriptscriptstyle 0}}\left(x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu0}}\right)\\
\sigma_{{\scriptscriptstyle 1}}\left(x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu1}}\right)\\
\vdots\\
\sigma_{{\scriptscriptstyle n}}\left(x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu n}}\right)
\end{pmatrix}^{\intercal},\begin{cases}
x_{{\scriptscriptstyle 0}}=1\\
w_{{\scriptscriptstyle 0\nu}}=b_{{\scriptscriptstyle \nu}}
\end{cases}\\
= & \sigma\left(\begin{pmatrix}1\\
x_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{{\scriptscriptstyle m}}
\end{pmatrix}^{\intercal}\begin{pmatrix}b_{{\scriptscriptstyle 0}} & b_{{\scriptscriptstyle 1}} & \cdots & b_{{\scriptscriptstyle n}}\\
w_{{\scriptscriptstyle 10}} & w_{{\scriptscriptstyle 11}} & \cdots & w_{{\scriptscriptstyle 1n}}\\
\vdots & \vdots & \ddots & \vdots\\
w_{{\scriptscriptstyle m0}} & w_{{\scriptscriptstyle m1}} & \cdots & w_{{\scriptscriptstyle mn}}
\end{pmatrix}\right)=\sigma\left(\begin{pmatrix}x_{{\scriptscriptstyle i}}w_{{\scriptscriptstyle i0}}+b_{{\scriptscriptstyle 0}}\\
x_{{\scriptscriptstyle i}}w_{{\scriptscriptstyle i1}}+b_{{\scriptscriptstyle 1}}\\
\vdots\\
x_{i}w_{{\scriptscriptstyle in}}+b_{{\scriptscriptstyle n}}
\end{pmatrix}^{\intercal}\right)=\sigma_{{\scriptscriptstyle \nu}}\left(x_{{\scriptscriptstyle \mu}}w_{{\scriptscriptstyle \mu\nu}}\right),\begin{cases}
1=x_{{\scriptscriptstyle 0}}\\
b_{{\scriptscriptstyle \nu}}=w_{{\scriptscriptstyle 0\nu}}
\end{cases}
\end{aligned}
$$
