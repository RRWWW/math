# hypergeometric function

## linear space of function

::: {show-in="html"}
<iframe width=500 height=300 frameborder="0" allowfullscreen src="https://player.bilibili.com/player.html?bvid=BV1PX4y167RS&autoplay=0"></iframe>
:::

[quantum state]^[\@ref(quantum-state)]^

[Taylor vs. Fourier]^[\@ref(taylor-vs.-fourier)]^

$$
f\left(x\right)=a_{{\scriptscriptstyle 0}}x^{0}+a_{{\scriptscriptstyle 1}}x^{1}+a_{{\scriptscriptstyle 2}}x^{2}+\cdots=\sum\limits _{k=0}^{\infty}a_{{\scriptscriptstyle k}}x^{k}
$$

$$
f\left(x\right)=x_{{\scriptscriptstyle 0}}x^{0}+x_{{\scriptscriptstyle 1}}x^{1}+x_{{\scriptscriptstyle 2}}x^{2}+\cdots=\sum\limits _{k=0}^{\infty}x_{{\scriptscriptstyle k}}x^{k}
$$

Def: \@ref(def:distance)

$$
\left\langle f\middle|g\right\rangle =\int_{a}^{b}\overline{f\left(x\right)}g\left(x\right)\mathrm{d}x\overset{f,g:\mathbb{R}\rightarrow\mathbb{R}}{=}\int_{a}^{b}f\left(x\right)g\left(x\right)\mathrm{d}x
$$

[Dirac bracket]^[\@ref(dirac-bracket)]^

$$
\left\langle x^{2}\middle|x\right\rangle \overset{x^{2},x:\mathbb{R}\rightarrow\mathbb{R}}{=}\int_{a}^{b}x^{2}x\mathrm{d}x=\int_{a}^{b}x^{3}\mathrm{d}x=\left[\dfrac{x^{4}}{4}\right]_{a}^{b}\not\equiv0
$$

$$
x^{0}\not\perp x^{1},x^{1}\not\perp x^{2},\cdots
$$

$$
\left\langle x_{{\scriptscriptstyle m}}\middle|x^{n}\right\rangle =\int_{a}^{b}x_{{\scriptscriptstyle m}}x^{n}\mathrm{d}x=\delta_{{\scriptscriptstyle mn}}
$$

$$
\left\langle 1\middle|x^{n}\right\rangle =\int_{a}^{b}x_{{\scriptscriptstyle 0}}x^{n}\mathrm{d}x=\delta_{{\scriptscriptstyle 0n}}\Rightarrow x_{{\scriptscriptstyle 0}}=\delta\left(x\right)=\delta\left(x-0\right)
$$

$$
\left\langle x_{{\scriptscriptstyle m}}\middle|x^{n}\right\rangle =\int_{a}^{b}x_{{\scriptscriptstyle m}}x^{n}\mathrm{d}x=\delta_{{\scriptscriptstyle mn}}\Rightarrow x_{{\scriptscriptstyle m}}=\dfrac{\left(-1\right)^{m}}{m!}\delta^{\left(m\right)}\left(x\right)
$$

$$
\left|f\right\rangle =1\left|f\right\rangle =\left(\sum\limits _{i}\left|\hat{f}_{{\scriptscriptstyle i}}\right\rangle \left\langle \hat{f}_{{\scriptscriptstyle i}}\right|\right)\left|f\right\rangle =\sum\limits _{i}\left|\hat{f}_{{\scriptscriptstyle i}}\right\rangle \left\langle \hat{f}_{{\scriptscriptstyle i}}\middle|f\right\rangle 
$$

$$
\begin{aligned}
\left|f\right\rangle = & 1\left|f\right\rangle =\left(\sum\limits _{i}\left|\hat{f}_{{\scriptscriptstyle i}}\right\rangle \left\langle \hat{f}_{{\scriptscriptstyle i}}\right|\right)\left|f\right\rangle =\sum\limits _{i}\left|\hat{f}_{{\scriptscriptstyle i}}\right\rangle \left\langle \hat{f}_{{\scriptscriptstyle i}}\middle|f\right\rangle \\
= & 1\left|f\right\rangle =\left(\sum\limits _{n}\left|x^{n}\right\rangle \left\langle x^{n}\right|\right)\left|f\right\rangle =\sum\limits _{n}\left|x^{n}\right\rangle \left\langle x^{n}\middle|f\right\rangle =\sum\limits _{n}\left\langle x^{n}\middle|f\right\rangle \left|x^{n}\right\rangle \\
\left\langle x^{n}\right|\left|f\right\rangle = & \left\langle x^{n}\middle|f\right\rangle =\int_{a}^{b}x_{{\scriptscriptstyle n}}f\left(x\right)\mathrm{d}x=\int_{a}^{b}\dfrac{\left(-1\right)^{n}}{n!}\delta^{\left(n\right)}\left(x\right)f\left(x\right)\mathrm{d}x=\dfrac{f^{\left(n\right)}\left(0\right)}{n!}\\
\left|f\right\rangle = & \sum\limits _{n}\left\langle x^{n}\middle|f\right\rangle \left|x^{n}\right\rangle =\sum\limits _{n}\dfrac{f^{\left(n\right)}\left(0\right)}{n!}\left|x^{n}\right\rangle \\
\left|f\right\rangle = & \sum\limits _{n}\dfrac{f^{\left(n\right)}\left(0\right)}{n!}\left|x^{n}\right\rangle \\
\Downarrow\\
f\left(x\right)= & \sum\limits _{n}\dfrac{f^{\left(n\right)}\left(0\right)}{n!}x^{n}
\end{aligned}
$$

## beta function

::: {show-in="html"}
<iframe width=500 height=300 frameborder="0" allowfullscreen src="https://player.bilibili.com/player.html?bvid=BV1pa4y1P7Da&autoplay=0"></iframe>
:::

$$
\begin{aligned}
\dbinom{n}{k}=\mathrm{C}_{k}^{n}= & \dfrac{n!}{\left(n-k\right)!k!}\\
= & \dfrac{n\left(n-1\right)\cdots\left(n-k+1\right)}{k!},\begin{cases}
n\in\mathbb{N}\\
k\in\left(\left\{ 0\right\} \cup\mathbb{N}\right)
\end{cases}\\
\dbinom{r}{k}= & \begin{cases}
\dfrac{r\left(r-1\right)\cdots\left(r-k+1\right)}{k!} & k\ge0,k\in\mathbb{Z}\\
0 & k<0,k\in\mathbb{Z}
\end{cases}
\end{aligned}
$$

$$
\sum\limits _{k=0}^{n}\dbinom{r}{k}\left(\cdot\right)
$$

$$
\sum\limits _{k=-\infty}^{n}\dbinom{r}{k}\left(\cdot\right)=\left(0+0+\cdots\right)+\sum\limits _{k=0}^{n}\dbinom{r}{k}\left(\cdot\right)
$$

$$
\sum\limits _{k=-\infty}^{\infty}\dbinom{r}{k}\left(\cdot\right)
$$

***

$$
n!=\Gamma\left(n+1\right)=\int_{0}^{\infty}x^{\left(n+1\right)-1}\mathrm{e}^{-x}\mathrm{d}x
$$

$$
\Gamma\left(z\right)=\int_{0}^{\infty}x^{z-1}\mathrm{e}^{-x}\mathrm{d}x
$$

$$
\Gamma\left(z+1\right)=z\Gamma\left(z\right)
$$

$$
\Gamma\left(z\right)\Gamma\left(1-z\right)=\dfrac{\pi}{\sin\left(\pi z\right)}
$$

$$
\begin{aligned}
\Gamma\left(z\right)\Gamma\left(1-z\right)= & \dfrac{\pi}{\sin\left(\pi z\right)}\\
\left[\Gamma\left(z\right)\Gamma\left(1-z\right)\right]_{z=-n}= & \left[\dfrac{\pi}{\sin\left(\pi z\right)}\right]_{z=-n},n\in\mathbb{N}\\
\Gamma\left(-n\right)n!=\Gamma\left(n+1\right)=\Gamma\left(-n\right)\Gamma\left(1-\left(-n\right)\right)= & \dfrac{\pi}{\sin\left(\pi\left(-n\right)\right)}=\dfrac{\pi}{-\sin\left(n\pi\right)}\\
\Gamma\left(-n\right)= & \dfrac{-\pi}{n!\sin\left(n\pi\right)}=\dfrac{-\pi}{n!0}\rightarrow-\infty,n\in\mathbb{N}
\end{aligned}
$$

$$
\begin{aligned}
\dbinom{n}{k}=\mathrm{C}_{k}^{n}= & \dfrac{n!}{\left(n-k\right)!k!}\\
= & \dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n-k+1\right)\Gamma\left(k+1\right)}
\end{aligned}
$$

$$
\dbinom{n}{k}=\dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n-k+1\right)\Gamma\left(k+1\right)}
$$

$$
\dbinom{n}{k}=\dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n-k+1\right)\Gamma\left(k+1\right)}\overset{k\le0}{=}\begin{cases}
\dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n+1\right)\Gamma\left(1\right)}=\dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n+1\right)1}=1 & k=0\\
\dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n-k+1\right)\left(-\infty\right)}=0 & k\le-1,k\in\mathbb{Z}
\end{cases}
$$

beta function = $\beta$ function

::: {.definition #beta-function}
beta function = $\beta$ function
:::

$$
B\left(p,q\right)=\int_{0}^{1}x^{p-1}\left(1-x\right)^{q-1}\mathrm{d}x=\dfrac{\Gamma\left(p\right)\Gamma\left(q\right)}{\Gamma\left(p+q\right)}
$$

$$
\begin{aligned}
\dbinom{n}{k}= & \dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n-k+1\right)\Gamma\left(k+1\right)}\\
\left[\dbinom{n}{k}\right]_{{\scriptscriptstyle \begin{cases}
n=a+b\\
k=a
\end{cases}}}= & \left[\dfrac{\Gamma\left(n+1\right)}{\Gamma\left(n-k+1\right)\Gamma\left(k+1\right)}\right]_{{\scriptscriptstyle \begin{cases}
n=a+b\\
k=a
\end{cases}}}\\
\dbinom{a+b}{a}= & \dfrac{\Gamma\left(a+b+1\right)}{\Gamma\left(a+b-a+1\right)\Gamma\left(a+1\right)}\\
= & \dfrac{\Gamma\left(a+b+1\right)}{\Gamma\left(b+1\right)\Gamma\left(a+1\right)}
\end{aligned}
$$

$$
\begin{aligned}
B\left(p,q\right)= & \dfrac{\Gamma\left(p\right)\Gamma\left(q\right)}{\Gamma\left(p+q\right)}\\
\left[B\left(p,q\right)\right]_{{\scriptscriptstyle \begin{cases}
p=a+1\\
q=b+1
\end{cases}}}= & \left[\dfrac{\Gamma\left(p\right)\Gamma\left(q\right)}{\Gamma\left(p+q\right)}\right]_{{\scriptscriptstyle \begin{cases}
p=a+1\\
q=b+1
\end{cases}}}\\
B\left(a+1,b+1\right)= & \dfrac{\Gamma\left(a+1\right)\Gamma\left(b+1\right)}{\Gamma\left(a+1+b+1\right)}\\
= & \dfrac{\Gamma\left(a+1\right)\Gamma\left(b+1\right)}{\Gamma\left(\left[a+b+1\right]+1\right)}=\dfrac{\Gamma\left(a+1\right)\Gamma\left(b+1\right)}{\left[a+b+1\right]\Gamma\left(a+b+1\right)}
\end{aligned}
$$

$$
\begin{aligned}
\dbinom{a+b}{a}= & \dfrac{\Gamma\left(a+b+1\right)}{\Gamma\left(b+1\right)\Gamma\left(a+1\right)}=\dfrac{1}{\dfrac{\Gamma\left(b+1\right)\Gamma\left(a+1\right)}{\Gamma\left(a+b+1\right)}}\\
= & \dfrac{1}{\left[a+b+1\right]\dfrac{\Gamma\left(b+1\right)\Gamma\left(a+1\right)}{\left[a+b+1\right]\Gamma\left(a+b+1\right)}}\\
= & \dfrac{1}{\left[a+b+1\right]B\left(a+1,b+1\right)}
\end{aligned}
$$

***

https://en.wikipedia.org/wiki/Beta_function

https://en.wikipedia.org/wiki/Beta_function#Other_identities_and_formulas

https://en.wikipedia.org/wiki/Beta_function#Multivariate_beta_function

https://www.bilibili.com/video/BV1pa4y1P7Da/?t=4m

### Wallis product formula

https://en.wikipedia.org/wiki/Wallis_product

https://www.bilibili.com/video/BV1pa4y1P7Da/?t=4m10s

https://www.math.sinica.edu.tw/mathmedia/journals/4739?keywords%5B%5D=Paul+Dirac

## gamma function

::: {show-in="html"}
<iframe width=500 height=300 frameborder="0" allowfullscreen src="https://player.bilibili.com/player.html?bvid=BV1cT411H7Hp&autoplay=0"></iframe>
:::

## recursion

::: {show-in="html"}
<iframe width=500 height=300 frameborder="0" allowfullscreen src="https://player.bilibili.com/player.html?bvid=BV1FV4y1Z7jm&autoplay=0"></iframe>
:::

::: {show-in="html"}
<iframe width=500 height=300 frameborder="0" allowfullscreen src="https://player.bilibili.com/player.html?bvid=BV1Sg4y1L7DF&autoplay=0"></iframe>
:::

## mean and variance of discrete probability distributions

::: {show-in="html"}
<iframe width=500 height=300 frameborder="0" allowfullscreen src="https://player.bilibili.com/player.html?bvid=BV1Tk4y1n7NX&autoplay=0"></iframe>
:::
