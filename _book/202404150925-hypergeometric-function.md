# hypergeometric function

## linear space of function

::: {show-in="html"}
<iframe width=500 height=300 frameborder="0" allowfullscreen src="https://player.bilibili.com/player.html?bvid=BV1PX4y167RS&autoplay=0"></iframe>
:::

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
