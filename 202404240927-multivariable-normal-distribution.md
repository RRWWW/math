# multivariate normal distribution

::: {.definition #unnamed-chunk-1}
probability density function (PDF) of normal distribution (= Gaussian distribution)
:::

$$ 
\mathcal{N}\left(x \mid \mu, \sigma^2\right)=\frac{1}{\sqrt{2 \pi} \sigma} \exp \left\{-\frac{(x-\mu)^2}{2 \sigma^2}\right\}
$$

If a continuous random variable $X$ follows a normal distribution with mean 0 and variance $\sigma^2$

$$
\begin{aligned}
X & \sim \mathrm{n}\left(\mu, \sigma^2\right)=\mathcal{N}\left(\mu, \sigma^2\right) \\
\Leftrightarrow f_X(x) 
& =\frac{1}{\sigma \sqrt{2 \pi}}\mathrm{e}^{\frac{-1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}
=\frac{\mathrm{e}^{\frac{-1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}}{\sigma \sqrt{2 \pi}}
=\mathrm{n}\left(x \mid \mu, \sigma^2\right) \\
& =\frac{1}{\sqrt{2 \pi} \sigma} \exp \left\{-\frac{(x-\mu)^2}{2 \sigma^2}\right\}
=\mathcal{N}\left(x \mid \mu, \sigma^2\right) 
\end{aligned}
$$

A random variable $X$ can be standardized by subtracting the mean $\mu$ and dividing by the standard deviation $\sigma$, resulting in the standardized random variable $Z$

$$
Z=\dfrac{X-\mu}{\sigma}\text{ or } z=\dfrac{x-\mu}{\sigma}
$$

The standardized random variable $Z$ follows the standard normal distribution

$$
\begin{aligned}
Z & \sim \mathrm{n}\left(0,1^2\right)=\mathcal{N}\left(0,1^2\right) \\
\Leftrightarrow f_Z(z) & =\frac{\mathrm{e}^{\frac{-1}{2}\left(\frac{x-0}{1}\right)^2}}{1 \cdot \sqrt{2 \pi}}=\frac{1}{\sqrt{2 \pi}} \exp \left\{-\frac{z^2}{2}\right\} \\
& =\mathrm{n}\left(z \mid 0,1^2\right)=\mathcal{N}\left(z \mid 0,1^2\right)
\end{aligned}
$$

To generalize from univariate random variables to multivariate random vectors, a random vector [@ccjou2014]

$$
\boldsymbol{Z}=\left\langle Z_{1},Z_{2},\cdots,Z_{p}\right\rangle =\begin{bmatrix}Z_{1} & Z_{2} & \cdots & Z_{p}\end{bmatrix}^{\intercal}=\begin{bmatrix}Z_{1}\\
Z_{2}\\
\vdots\\
Z_{p}
\end{bmatrix}
$$

with $p$ random variable components is said to follow the standard multivariate normal distribution if and only if its joint PDF is given by

\begin{equation}
(\#eq:smnd)
f_{\boldsymbol{Z}}(\boldsymbol{z})=\frac{1}{(2\pi)^{p/2}}\exp\left\{ -\frac{\boldsymbol{z}^{\intercal}\boldsymbol{z}}{2}\right\} =\frac{1}{(2\pi)^{p/2}}\exp\left\{ -\frac{\boldsymbol{z}\cdot\boldsymbol{z}}{2}\right\} 
\end{equation}

\@ref(eq:smnd) can be rewritten as the following

$$
\begin{aligned}
f_{\boldsymbol{Z}}(\boldsymbol{z})= & \underbrace{\frac{1}{\sqrt{2\pi}}\frac{1}{\sqrt{2\pi}}\cdots\frac{1}{\sqrt{2\pi}}}_{p\text{ times }}\exp\left\{ -\frac{z_{1}^{2}}{2}-\frac{z_{2}^{2}}{2}-\cdots-\frac{z_{p}^{2}}{2}\right\} \\
= & \frac{1}{\sqrt{2\pi}}\exp\left\{ -\frac{z_{1}^{2}}{2}\right\} \frac{1}{\sqrt{2\pi}}\exp\left\{ -\frac{z_{2}^{2}}{2}\right\} \cdots\frac{1}{\sqrt{2\pi}}\exp\left\{ -\frac{z_{p}^{2}}{2}\right\} \\
= & f\left(z_{1}\right)f\left(z_{2}\right)\cdots f\left(z_{p}\right)
\end{aligned}
$$

where

\begin{equation}
(\#eq:iidsnd)
f_{Z_{i}}\left(z_{i}\right)=\frac{1}{\sqrt{2\pi}}\exp\left\{ -\frac{z_{i}^{2}}{2}\right\} =f\left(z_{i}\right)\Rightarrow Z_{i}\sim\mathcal{N}\left(0,1^{2}\right)=\mathrm{n}\left(0,1^{2}\right)
\end{equation}

$$
\begin{aligned}
f_{Z_{i}}\left(z_{i}\right)= & \int_{-\infty}^{\infty}\cdots\int_{-\infty}^{\infty}f_{\boldsymbol{Z}}\left(z_{1},\ldots,z_{i-1},z_{i},z_{i+1},\ldots,z_{p}\right)\mathrm{d}z_{1}\cdots\mathrm{d}z_{i-1}\mathrm{d}z_{i+1}\cdots\mathrm{d}z_{p}\\
= & \int_{-\infty}^{\infty}\cdots\int_{-\infty}^{\infty}f\left(z_{1}\right)\cdots f\left(z_{i-1}\right)f\left(z_{i}\right)f\left(z_{i+1}\right)\cdots f\left(z_{p}\right)\mathrm{d}z_{1}\cdots\mathrm{d}z_{i-1}\mathrm{d}z_{i+1}\cdots\mathrm{d}z_{p}\\
= & f\left(z_{i}\right)\int_{-\infty}^{\infty}f\left(z_{1}\right)\mathrm{d}z_{1}\cdots\int_{-\infty}^{\infty}f\left(z_{i-1}\right)\mathrm{d}z_{i-1}\int_{-\infty}^{\infty}f\left(z_{i+1}\right)\mathrm{d}z_{i+1}\cdots\int_{-\infty}^{\infty}f\left(z_{p}\right)\mathrm{d}z_{p}\\
= & f\left(z_{i}\right) \overset{\eqref{eq:iidsnd}}{=}\frac{1}{\sqrt{2\pi}}\exp\left\{ -\frac{z_{i}^{2}}{2}\right\}
\end{aligned}
$$

[covariance matrix]^[\@ref(covariance-matrix)]^

::: {.definition #unnamed-chunk-2}
covariance matrix of a random vector[@ccjou2014a]
:::

$$ 
  \mathrm{C}\left[\boldsymbol{X}\right]=\mathrm{Cov}\left[\boldsymbol{X}\right]=\mathrm{V}\left[\boldsymbol{X}\right]=\mathrm{E}\left[\left[\boldsymbol{X}-\mathrm{E}\left(\boldsymbol{X}\right)\right]\left[\boldsymbol{X}-\mathrm{E}\left(\boldsymbol{X}\right)\right]^{\intercal}\right]
$$

$$
\boldsymbol{X}=\left\langle X_{1},X_{2},\cdots,X_{p}\right\rangle =\begin{bmatrix}X_{1} & X_{2} & \cdots & X_{p}\end{bmatrix}^{\intercal}=\begin{bmatrix}X_{1}\\
X_{2}\\
\vdots\\
X_{p}
\end{bmatrix}
$$

$$
\mathrm{E}\left[\boldsymbol{X}\right]=\left\langle \mathrm{E}\left[X_{1}\right],\mathrm{E}\left[X_{2}\right],\cdots,\mathrm{E}\left[X_{p}\right]\right\rangle =\begin{bmatrix}\mathrm{E}\left[X_{1}\right] & \mathrm{E}\left[X_{2}\right] & \cdots & \mathrm{E}\left[X_{p}\right]\end{bmatrix}^{\intercal}=\begin{bmatrix}\mathrm{E}\left[X_{1}\right]\\
\mathrm{E}\left[X_{2}\right]\\
\vdots\\
\mathrm{E}\left[X_{p}\right]
\end{bmatrix}
$$

$$
\boldsymbol{X}-\mathrm{E}\left[\boldsymbol{X}\right]=\begin{bmatrix}X_{1}-\mathrm{E}\left[X_{1}\right]\\
X_{2}-\mathrm{E}\left[X_{2}\right]\\
\vdots\\
X_{p}-\mathrm{E}\left[X_{p}\right]
\end{bmatrix}
$$

$$
\begin{aligned}
 & \left[\boldsymbol{X}-\mathrm{E}\left(\boldsymbol{X}\right)\right]\left[\boldsymbol{X}-\mathrm{E}\left(\boldsymbol{X}\right)\right]^{\intercal}\\
= & \begin{bmatrix}X_{1}-\mathrm{E}\left[X_{1}\right]\\
X_{2}-\mathrm{E}\left[X_{2}\right]\\
\vdots\\
X_{p}-\mathrm{E}\left[X_{p}\right]
\end{bmatrix}\begin{bmatrix}X_{1}-\mathrm{E}\left[X_{1}\right] & X_{2}-\mathrm{E}\left[X_{2}\right] & \cdots & X_{p}-\mathrm{E}\left[X_{p}\right]\end{bmatrix}\\
= & \begin{bmatrix}\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right) & \left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)\left(X_{2}-\mathrm{E}\left[X_{2}\right]\right) & \cdots & \left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\\
\left(X_{2}-\mathrm{E}\left[X_{2}\right]\right)\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right) & \left(X_{2}-\mathrm{E}\left[X_{2}\right]\right)\left(X_{2}-\mathrm{E}\left[X_{2}\right]\right) & \cdots & \left(X_{2}-\mathrm{E}\left[X_{2}\right]\right)\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\\
\vdots & \vdots & \ddots & \vdots\\
\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right) & \left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\left(X_{2}-\mathrm{E}\left[X_{2}\right]\right) & \cdots & \left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)
\end{bmatrix}\\
= & \begin{bmatrix}\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)^{2} & \cdots & \left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\\
\vdots & \ddots & \vdots\\
\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right) & \cdots & \left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)^{2}
\end{bmatrix}
\end{aligned}
$$


\begin{align}
(\#eq:covmatrix)
 & \mathrm{E}\left[\left[\boldsymbol{X}-\mathrm{E}\left(\boldsymbol{X}\right)\right]\left[\boldsymbol{X}-\mathrm{E}\left(\boldsymbol{X}\right)\right]^{\intercal}\right]\\
= & \mathrm{E}\begin{bmatrix}\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)^{2} & \cdots & \left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\\
\vdots & \ddots & \vdots\\
\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right) & \cdots & \left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)^{2}
\end{bmatrix}\\
= & \begin{bmatrix}\mathrm{E}\left[\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)^{2}\right] & \cdots & \mathrm{E}\left[\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\right]\\
\vdots & \ddots & \vdots\\
\mathrm{E}\left[\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)\left(X_{1}-\mathrm{E}\left[X_{1}\right]\right)\right] & \cdots & \mathrm{E}\left[\left(X_{p}-\mathrm{E}\left[X_{p}\right]\right)^{2}\right]
\end{bmatrix}\\
= & \begin{bmatrix}\mathrm{V}\left(X_{1},X_{1}\right) & \cdots & \mathrm{V}\left(X_{1},X_{p}\right)\\
\vdots & \ddots & \vdots\\
\mathrm{V}\left(X_{p},X_{1}\right) & \cdots & \mathrm{V}\left(X_{p},X_{p}\right)
\end{bmatrix}=\begin{bmatrix}\mathrm{V}\left(X_{1},X_{1}\right) & \mathrm{V}\left(X_{1},X_{2}\right) & \cdots & \mathrm{V}\left(X_{1},X_{p}\right)\\
\mathrm{V}\left(X_{2},X_{1}\right) & \mathrm{V}\left(X_{2},X_{2}\right) & \cdots & \mathrm{V}\left(X_{2},X_{p}\right)\\
\vdots & \vdots & \ddots & \vdots\\
\mathrm{V}\left(X_{p},X_{1}\right) & \mathrm{V}\left(X_{p},X_{2}\right) & \cdots & \mathrm{V}\left(X_{p},X_{p}\right)
\end{bmatrix}\\
= & \begin{bmatrix}\mathrm{V}\left(X_{1}\right) & \cdots & \mathrm{V}\left(X_{1},X_{p}\right)\\
\vdots & \ddots & \vdots\\
\mathrm{V}\left(X_{p},X_{1}\right) & \cdots & \mathrm{V}\left(X_{p}\right)
\end{bmatrix}=\begin{bmatrix}\mathrm{V}\left(X_{1}\right) & \mathrm{V}\left(X_{1},X_{2}\right) & \cdots & \mathrm{V}\left(X_{1},X_{p}\right)\\
\mathrm{V}\left(X_{2},X_{1}\right) & \mathrm{V}\left(X_{2}\right) & \cdots & \mathrm{V}\left(X_{2},X_{p}\right)\\
\vdots & \vdots & \ddots & \vdots\\
\mathrm{V}\left(X_{p},X_{1}\right) & \mathrm{V}\left(X_{p},X_{2}\right) & \cdots & \mathrm{V}\left(X_{p}\right)
\end{bmatrix}\\
= & \begin{bmatrix}\mathrm{V}\left(X_{1}\right) & \cdots & \mathrm{C}\left(X_{1},X_{p}\right)\\
\vdots & \ddots & \vdots\\
\mathrm{C}\left(X_{p},X_{1}\right) & \cdots & \mathrm{V}\left(X_{p}\right)
\end{bmatrix}=\begin{bmatrix}\mathrm{V}\left(X_{1}\right) & \mathrm{C}\left(X_{1},X_{2}\right) & \cdots & \mathrm{C}\left(X_{1},X_{p}\right)\\
\mathrm{C}\left(X_{2},X_{1}\right) & \mathrm{V}\left(X_{2}\right) & \cdots & \mathrm{C}\left(X_{2},X_{p}\right)\\
\vdots & \vdots & \ddots & \vdots\\
\mathrm{C}\left(X_{p},X_{1}\right) & \mathrm{C}\left(X_{p},X_{2}\right) & \cdots & \mathrm{V}\left(X_{p}\right)
\end{bmatrix}\\
= & \begin{bmatrix}\sigma_{1}^{2} & \cdots & \sigma_{1p}\\
\vdots & \ddots & \vdots\\
\sigma_{p1} & \cdots & \sigma_{p}^{2}
\end{bmatrix}=\begin{bmatrix}\sigma_{1}^{2} & \sigma_{12} & \cdots & \sigma_{1p}\\
\sigma_{21} & \sigma_{2}^{2} & \cdots & \sigma_{2p}\\
\vdots & \vdots & \ddots & \vdots\\
\sigma_{p1} & \sigma_{p2} & \cdots & \sigma_{p}^{2}
\end{bmatrix}=\begin{bmatrix}\sigma_{11} & \sigma_{12} & \cdots & \sigma_{1p}\\
\sigma_{21} & \sigma_{22} & \cdots & \sigma_{2p}\\
\vdots & \vdots & \ddots & \vdots\\
\sigma_{p1} & \sigma_{p2} & \cdots & \sigma_{pp}
\end{bmatrix}=\left[\sigma_{ij}\right]_{p\times p}=\mathit{\Sigma}
\end{align}

$$
\boldsymbol{X}\sim\mathcal{D}\left(\boldsymbol{\mu},\mathit{\Sigma}\right)=\mathrm{d}\left(\boldsymbol{\mu}_{\boldsymbol{X}},\mathit{\Sigma}_{\boldsymbol{X}}\right)=\mathrm{d}\left(\mathrm{E}\left[\boldsymbol{X}\right],\mathrm{C}\left[\boldsymbol{X}\right]\right)=\mathrm{d}\left(\mathrm{E}\left[\boldsymbol{X}\right],\mathrm{V}\left[\boldsymbol{X}\right]\right)
$$

$$
\boldsymbol{Z}\sim\mathcal{N}\left(\boldsymbol{\mu}_{\boldsymbol{Z}},\mathit{\Sigma}_{\boldsymbol{Z}}\right)=\mathrm{n}\left(\mathrm{E}\left[\boldsymbol{Z}\right],\mathrm{V}\left[\boldsymbol{Z}\right]\right)
$$

$$
\begin{aligned}
 & \mathrm{E}\left[\boldsymbol{Z}\right]=\begin{bmatrix}\mathrm{E}\left[Z_{1}\right]\\
\mathrm{E}\left[Z_{2}\right]\\
\vdots\\
\mathrm{E}\left[Z_{p}\right]
\end{bmatrix}=\begin{bmatrix}\mathrm{E}\left[Z_{i}\right]\end{bmatrix}_{p\times1}\\
\Rightarrow & \mathrm{E}\left[Z_{i}\right]=\int_{-\infty}^{\infty}z_{i}f_{Z_{i}}\left(z_{i}\right)\mathrm{d}z_{i}\overset{\eqref{eq:iidsnd}}{=}\int_{-\infty}^{\infty}z_{i}\frac{\mathrm{e}^{\frac{-1}{2}z_{i}^{2}}}{\sqrt{2\pi}}\mathrm{d}z_{i}=0\\
\Rightarrow & \mathrm{E}\left[\boldsymbol{Z}\right]=\boldsymbol{0}\\
\Rightarrow & \boldsymbol{Z}\sim\mathcal{N}\left(\boldsymbol{\mu}_{\boldsymbol{Z}}=\boldsymbol{0},\mathit{\Sigma}_{\boldsymbol{Z}}\right)=\mathrm{n}\left(\boldsymbol{0},\mathrm{V}\left[\boldsymbol{Z}\right]\right)
\end{aligned}
$$

$$
\mathrm{V}\left(Z_{i}\right)=\int_{-\infty}^{\infty}\left(z_{i}-\mu_{Z_{i}}\right)^{2}f_{Z_{i}}\left(z_{i}\right)\mathrm{d}z_{i}\overset{\eqref{eq:iidsnd}}{=}\int_{-\infty}^{\infty}\left(z_{i}-0\right)^{2}\frac{\mathrm{e}^{\frac{-1}{2}z_{i}^{2}}}{\sqrt{2\pi}}\mathrm{d}z_{i}=1
$$

\begin{equation}
(\#eq:idpsmnd)
\mathrm{V}\left(Z_{i},Z_{j}\right)\overset{i\ne j\Rightarrow Z_{i},Z_{j}\text{are independent}}{=}0
\end{equation}

$$
\begin{aligned}
\mathrm{V}\left[\boldsymbol{Z}\right]= & \begin{bmatrix}\mathrm{V}\left(Z_{1}\right) & \mathrm{V}\left(Z_{1},Z_{2}\right) & \cdots & \mathrm{V}\left(Z_{1},Z_{p}\right)\\
\mathrm{V}\left(Z_{2},Z_{1}\right) & \mathrm{V}\left(Z_{2}\right) & \cdots & \mathrm{V}\left(Z_{2},Z_{p}\right)\\
\vdots & \vdots & \ddots & \vdots\\
\mathrm{V}\left(Z_{p},Z_{1}\right) & \mathrm{V}\left(Z_{p},Z_{2}\right) & \cdots & \mathrm{V}\left(Z_{p}\right)
\end{bmatrix}=\begin{bmatrix}\sigma_{11} & \sigma_{12} & \cdots & \sigma_{1p}\\
\sigma_{21} & \sigma_{22} & \cdots & \sigma_{2p}\\
\vdots & \vdots & \ddots & \vdots\\
\sigma_{p1} & \sigma_{p2} & \cdots & \sigma_{pp}
\end{bmatrix}\\
= & \begin{bmatrix}\sigma_{1}^{2} & \sigma_{12} & \cdots & \sigma_{1p}\\
\sigma_{21} & \sigma_{2}^{2} & \cdots & \sigma_{2p}\\
\vdots & \vdots & \ddots & \vdots\\
\sigma_{p1} & \sigma_{p2} & \cdots & \sigma_{p}^{2}
\end{bmatrix}\overset{\ref{eq:idpsmnd}}{=}\begin{bmatrix}1 & 0 & \cdots & 0\\
0 & 1 & \cdots & 0\\
\vdots & \vdots & \ddots & \vdots\\
0 & 0 & \cdots & 1
\end{bmatrix}=I_{p\times p}=I_{p}=I
\end{aligned}
$$

$$
\boldsymbol{Z}\sim\mathcal{N}\left(\boldsymbol{\mu}_{\boldsymbol{Z}},\mathit{\Sigma}_{\boldsymbol{Z}}\right)=\mathrm{n}\left(\mathrm{E}\left[\boldsymbol{Z}\right],\mathrm{V}\left[\boldsymbol{Z}\right]\right)=\mathcal{N}\left(\boldsymbol{0},I\right)\Leftrightarrow\begin{cases}
\boldsymbol{\mu}_{\boldsymbol{Z}}=\mathrm{E}\left[\boldsymbol{Z}\right]=\boldsymbol{0}=\left[0\right]_{p}=\left[0\right]_{p\times1}\\
\mathit{\Sigma}_{\boldsymbol{Z}}=\mathrm{V}\left[\boldsymbol{Z}\right]=I=I_{p}=I_{p\times p}
\end{cases}
$$

$$
\begin{aligned}
\boldsymbol{Z}= & \begin{bmatrix}Z_{1}\\
Z_{2}\\
\vdots\\
Z_{p}
\end{bmatrix}=\begin{bmatrix}\dfrac{X_{1}-\mu_{1}}{\sigma_{1}}\\
\dfrac{X_{2}-\mu_{2}}{\sigma_{2}}\\
\vdots\\
\dfrac{X_{p}-\mu_{p}}{\sigma_{p}}
\end{bmatrix}=\begin{bmatrix}\dfrac{1}{\sigma_{1}} & 0 & \cdots & 0\\
0 & \dfrac{1}{\sigma_{2}} & \cdots & 0\\
\vdots & \vdots & \ddots & \vdots\\
0 & 0 & \cdots & \dfrac{1}{\sigma_{p}}
\end{bmatrix}\begin{bmatrix}X_{1}-\mu_{1}\\
X_{2}-\mu_{2}\\
\vdots\\
X_{p}-\mu_{p}
\end{bmatrix}\\
= & \begin{bmatrix}\dfrac{1}{\sigma_{1}} & 0 & \cdots & 0\\
0 & \dfrac{1}{\sigma_{2}} & \cdots & 0\\
\vdots & \vdots & \ddots & \vdots\\
0 & 0 & \cdots & \dfrac{1}{\sigma_{p}}
\end{bmatrix}\left(\begin{bmatrix}X_{1}\\
X_{2}\\
\vdots\\
X_{p}
\end{bmatrix}-\begin{bmatrix}\mu_{1}\\
\mu_{2}\\
\vdots\\
\mu_{p}
\end{bmatrix}\right)=B^{-1}\left(\boldsymbol{X}-\boldsymbol{\mu}\right)\\
\Rightarrow\boldsymbol{X}= & B\boldsymbol{Z}+\boldsymbol{\mu}
\end{aligned}
$$

$$
\boldsymbol{X} = B\boldsymbol{Z} + \boldsymbol{\mu} = T\left(\boldsymbol{Z}\right)
$$

by [$\mathrm{V}\left[A\boldsymbol{X}+\boldsymbol{b}\right]=A\mathrm{V}\left[\boldsymbol{X}\right]A^{\intercal}$](#mathrmvleftaboldsymbolxboldsymbolbrightamathrmvleftboldsymbolxrightamathrmt)

\begin{equation}
(\#eq:covlt)
\mathit{\Sigma}=\mathit{\Sigma}_{\boldsymbol{X}}=\mathrm{V}\left[\boldsymbol{X}\right]=\mathrm{V}\left[B\boldsymbol{Z}+\boldsymbol{\mu}\right]=B\mathrm{V}\left[\boldsymbol{Z}\right]B^{\intercal}=BIB^{\intercal}=BB^{\intercal}
\end{equation}

Consider two infinitesimal volumes of $p$-dimensional parallelepipeds in the different $\mathbb{R}^p$ spaces[@ccjou2012]

$$
V_{\boldsymbol{x}}=\left[x_{1},x_{1}+\mathrm{d}x_{1}\right]\times\left[x_{2},x_{2}+\mathrm{d}x_{2}\right]\times\cdots\times\left[x_{p},x_{p}+\mathrm{d}x_{p}\right]
$$

and

$$
V_{\boldsymbol{z}}=\left[z_{1},z_{1}+\mathrm{d}z_{1}\right]\times\left[z_{2},z_{2}+\mathrm{d}z_{2}\right]\times\cdots\times\left[z_{p},z_{p}+\mathrm{d}z_{p}\right]
$$

Their relationship under linear transformation is

$$
\begin{aligned}
V_{\boldsymbol{x}}=T\left(V_{\boldsymbol{z}}\right)= & \left[T\left(z_{1}\right),T\left(z_{1}\right)+T\left(\mathrm{d}z_{1}\right)\right]\\
 & \times\left[T\left(z_{2}\right),T\left(z_{2}\right)+T\left(\mathrm{d}z_{2}\right)\right]\\
 & \times\cdots\\
 & \times\left[T\left(z_{p}\right),T\left(z_{p}\right)+T\left(\mathrm{d}z_{p}\right)\right]
\end{aligned}
$$

and

$$
\mathrm{d}x_{i}=\sum_{j}\dfrac{\partial x_{i}}{\partial z_{j}}\mathrm{d}z_{j}
$$

For examples in 2 dimension,

$$
\begin{bmatrix}\mathrm{d}x_{1}\\
\mathrm{d}x_{2}
\end{bmatrix}=\begin{bmatrix}\dfrac{\partial x_{1}}{\partial z_{1}} & \dfrac{\partial x_{1}}{\partial z_{2}}\\
\dfrac{\partial x_{2}}{\partial z_{1}} & \dfrac{\partial x_{2}}{\partial z_{2}}
\end{bmatrix}\begin{bmatrix}\mathrm{d}z_{1}\\
\mathrm{d}z_{2}
\end{bmatrix}
$$
Two element infinitesimal one-directional vectors of $\boldsymbol{Z}$ transformed into another space of $\boldsymbol{X}$ are

$$
T\left(\mathrm{d}\boldsymbol{z}_{1}\right)=\begin{bmatrix}\dfrac{\partial x_{1}}{\partial z_{1}} & \dfrac{\partial x_{1}}{\partial z_{2}}\\
\dfrac{\partial x_{2}}{\partial z_{1}} & \dfrac{\partial x_{2}}{\partial z_{2}}
\end{bmatrix}\begin{bmatrix}\mathrm{d}z_{1}\\
0
\end{bmatrix}=\begin{bmatrix}\dfrac{\partial x_{1}}{\partial z_{1}}\mathrm{d}z_{1}\\
\dfrac{\partial x_{2}}{\partial z_{1}}\mathrm{d}z_{1}
\end{bmatrix}
$$

and

$$
T\left(\mathrm{d}\boldsymbol{z}_{2}\right)=\begin{bmatrix}\dfrac{\partial x_{1}}{\partial z_{1}} & \dfrac{\partial x_{1}}{\partial z_{2}}\\
\dfrac{\partial x_{2}}{\partial z_{1}} & \dfrac{\partial x_{2}}{\partial z_{2}}
\end{bmatrix}\begin{bmatrix}0\\
\mathrm{d}z_{2}
\end{bmatrix}=\begin{bmatrix}\dfrac{\partial x_{1}}{\partial z_{2}}\mathrm{d}z_{2}\\
\dfrac{\partial x_{2}}{\partial z_{2}}\mathrm{d}z_{2}
\end{bmatrix}
$$

Their corresponding area(volume) in the space of $\boldsymbol{X}$ is

$$
\begin{aligned}
 & \int_{A_{\boldsymbol{x}}}\mathrm{d}A_{\boldsymbol{x}}=\int_{A_{\boldsymbol{x}}}\mathrm{d}x_{1}\mathrm{d}x_{2}=\int_{T\left(A_{\boldsymbol{z}}\right)}\mathrm{d}x_{1}\mathrm{d}x_{2}\\
= & \int_{A_{\boldsymbol{z}}}\left|\begin{bmatrix}T\left(\mathrm{d}\boldsymbol{z}_{1}\right) & T\left(\mathrm{d}\boldsymbol{z}_{2}\right)\end{bmatrix}\right|=\int_{A_{\boldsymbol{z}}}\begin{vmatrix}\dfrac{\partial x_{1}}{\partial z_{1}}\mathrm{d}z_{1} & \dfrac{\partial x_{1}}{\partial z_{2}}\mathrm{d}z_{2}\\
\dfrac{\partial x_{2}}{\partial z_{1}}\mathrm{d}z_{1} & \dfrac{\partial x_{2}}{\partial z_{2}}\mathrm{d}z_{2}
\end{vmatrix}\\
= & \int_{A_{\boldsymbol{z}}}\begin{vmatrix}\dfrac{\partial x_{1}}{\partial z_{1}} & \dfrac{\partial x_{1}}{\partial z_{2}}\\
\dfrac{\partial x_{2}}{\partial z_{1}} & \dfrac{\partial x_{2}}{\partial z_{2}}
\end{vmatrix}\mathrm{d}z_{1}\mathrm{d}z_{2}=\int_{A_{\boldsymbol{z}}}\left|J\right|\mathrm{d}A_{\boldsymbol{z}}
\end{aligned}
$$

To generalize for volumes in $p$ dimension,

$$
\begin{aligned}
 & \int_{V_{\boldsymbol{x}}}\mathrm{d}V_{\boldsymbol{x}}=\int_{V_{\boldsymbol{x}}}\mathrm{d}x_{1}\mathrm{d}x_{2}\cdots\mathrm{d}x_{p}=\int_{T\left(V_{\boldsymbol{z}}\right)}\mathrm{d}x_{1}\mathrm{d}x_{2}\cdots\mathrm{d}x_{p}\\
= & \int_{A_{\boldsymbol{z}}}\left|\begin{bmatrix}T\left(\mathrm{d}\boldsymbol{z}_{1}\right) & T\left(\mathrm{d}\boldsymbol{z}_{2}\right) & \cdots & T\left(\mathrm{d}\boldsymbol{z}_{p}\right)\end{bmatrix}\right|=\int_{V_{\boldsymbol{z}}}\begin{vmatrix}\left[\dfrac{\partial x_{i}}{\partial z_{j}}\mathrm{d}z_{j}\right]_{p\times p}\end{vmatrix}\\
= & \int_{V_{\boldsymbol{z}}}\begin{vmatrix}\left[\dfrac{\partial x_{i}}{\partial z_{j}}\right]_{p\times p}\end{vmatrix}\mathrm{d}z_{1}\mathrm{d}z_{2}\cdots\mathrm{d}z_{p}=\int_{V_{\boldsymbol{z}}}\left|J\right|\mathrm{d}V_{\boldsymbol{z}}
\end{aligned}
$$

i.e.

\begin{equation}
(\#eq:mitj)
\int_{V_{\boldsymbol{x}}}\mathrm{d}V_{\boldsymbol{x}}=\int_{V_{\boldsymbol{z}}}\left|J\right|\mathrm{d}V_{\boldsymbol{z}}
\end{equation}

where $J$ is a Jacobian matrix

$$
J=\left[\dfrac{\partial x_{i}}{\partial z_{j}}\right]_{p\times p}=\dfrac{\partial\boldsymbol{x}}{\partial\boldsymbol{z}}
$$

or $\left|J\right|$ is a Jacobian determinant or simply Jacobian

$$
\left|J\right|=\left|\dfrac{\partial x_{i}}{\partial z_{j}}\right|_{p\times p}=\left|\dfrac{\partial\boldsymbol{x}}{\partial\boldsymbol{z}}\right|
$$

The probability of the same event should be invariant under transformation.

$$
\begin{aligned}
 & \int_{V_{\boldsymbol{x}}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\mathrm{d}V_{\boldsymbol{x}}=\int_{V_{\boldsymbol{x}}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\mathrm{d}x_{1}\mathrm{d}x_{2}\cdots\mathrm{d}x_{p}\\
= & \int_{T\left(V_{\boldsymbol{z}}\right)}f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\mathrm{d}x_{1}\mathrm{d}x_{2}\cdots\mathrm{d}x_{p}\\
= & \int_{V_{\boldsymbol{z}}}f_{\boldsymbol{Z}}\left(\boldsymbol{z}\right)\mathrm{d}V_{\boldsymbol{z}}=\int_{V_{\boldsymbol{z}}}f_{\boldsymbol{Z}}\left(\boldsymbol{z}\right)\mathrm{d}z_{1}\mathrm{d}z_{2}\cdots\mathrm{d}z_{p}
\end{aligned}
$$

i.e.

\begin{equation}
(\#eq:ipmit)
\int_{V_{\boldsymbol{x}}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\mathrm{d}V_{\boldsymbol{x}}=\int_{V_{\boldsymbol{z}}}f_{\boldsymbol{Z}}\left(\boldsymbol{z}\right)\mathrm{d}V_{\boldsymbol{z}}
\end{equation}

$$
\begin{cases}
\int_{V_{\boldsymbol{x}}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\mathrm{d}V_{\boldsymbol{x}}=\int_{V_{\boldsymbol{z}}}f_{\boldsymbol{Z}}\left(\boldsymbol{z}\right)\mathrm{d}V_{\boldsymbol{z}} & \ref{eq:ipmit}\\
\int_{V_{\boldsymbol{x}}}\mathrm{d}V_{\boldsymbol{x}}=\int_{V_{\boldsymbol{z}}}\left|J\right|\mathrm{d}V_{\boldsymbol{z}} & \ref{eq:mitj}
\end{cases}
$$

\begin{align}
\boldsymbol{Z}= & B^{-1}\left(\boldsymbol{X}-\boldsymbol{\mu}\right)\nonumber \\
\boldsymbol{z}= & B^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right) (\#eq:sltx2z)\\
\boldsymbol{X}= & B\boldsymbol{Z}+\boldsymbol{\mu}\nonumber \\
\boldsymbol{x}= & B\boldsymbol{z}+\boldsymbol{\mu}\nonumber \\
J=\left[\dfrac{\partial x_{i}}{\partial z_{j}}\right]_{p\times p}=\dfrac{\partial\boldsymbol{x}}{\partial\boldsymbol{z}}= & B (\#eq:sltj)\\
\left|J\right|=\left|\dfrac{\partial x_{i}}{\partial z_{j}}\right|_{p\times p}=\left|\dfrac{\partial\boldsymbol{x}}{\partial\boldsymbol{z}}\right|= & \left|B\right|\nonumber 
\end{align}

$$
\begin{aligned}
\int_{V_{\boldsymbol{z}}}f_{\boldsymbol{Z}}\left(\boldsymbol{z}\right)\mathrm{d}V_{\boldsymbol{z}}\overset{\ref{eq:ipmit}}{=} & \int_{V_{\boldsymbol{x}}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\mathrm{d}V_{\boldsymbol{x}}=\int_{V_{\boldsymbol{x}}}\mathrm{d}V_{\boldsymbol{x}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\\
\overset{\ref{eq:mitj}}{=}\int_{V_{\boldsymbol{z}}}\left|J\right|\mathrm{d}V_{\boldsymbol{z}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\left(\boldsymbol{z}\right)\right)= & \int_{V_{\boldsymbol{z}}}f_{\boldsymbol{X}}\left(\boldsymbol{x}\left(\boldsymbol{z}\right)\right)\left|J\right|\mathrm{d}V_{\boldsymbol{z}}\\
f_{\boldsymbol{Z}}\left(\boldsymbol{z}\right)\overset{\Downarrow}{=} & f_{\boldsymbol{X}}\left(\boldsymbol{x}\left(\boldsymbol{z}\right)\right)\left|J\right|\\
f_{\boldsymbol{X}}\left(\boldsymbol{x}\left(\boldsymbol{z}\right)\right)\overset{\Downarrow}{=} & \left|J\right|^{-1}f_{\boldsymbol{Z}}\left(\boldsymbol{z}\right)\overset{\ref{eq:smnd}}{=}\left|J\right|^{-1}\frac{1}{(2\pi)^{p/2}}\exp\left\{ \frac{-\boldsymbol{z}^{\intercal}\boldsymbol{z}}{2}\right\} \\
f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)\overset{\Downarrow}{=} & \left|J\right|^{-1}f_{\boldsymbol{Z}}\left(\boldsymbol{z}\left(\boldsymbol{x}\right)\right)\overset{\ref{eq:sltj},\ref{eq:sltx2z}}{=}\left|B\right|^{-1}f_{\boldsymbol{Z}}\left(B^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right)\\
= & \left|B\right|^{-1}(2\pi)^{-p/2}\exp\left\{ \frac{-1}{2}\left[B^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right]^{\intercal}\left[B^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right]\right\} \\
= & \left|B\right|^{-1/2}\left|B\right|^{-1/2}(2\pi)^{-p/2}\exp\left\{ \frac{-1}{2}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)^{\intercal}\left(B^{-1}\right)^{\intercal}B^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right\} \\
= & \left|B\right|^{-1/2}\left|B^{\intercal}\right|^{-1/2}(2\pi)^{-p/2}\exp\left\{ \frac{-1}{2}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)^{\intercal}\left(B^{\intercal}\right)^{-1}B^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right\} \\
= & \left|BB^{\intercal}\right|^{-1/2}(2\pi)^{-p/2}\exp\left\{ \frac{-1}{2}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)^{\intercal}\left(BB^{\intercal}\right)^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right\} \\
\overset{\ref{eq:covlt}}{=} & \left|\mathit{\Sigma}\right|^{-1/2}(2\pi)^{-p/2}\exp\left\{ \frac{-1}{2}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)^{\intercal}\mathit{\Sigma}^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right\} \\
= & \left(\left|\mathit{\Sigma}\right|\left(2\pi\right)^{p}\right)^{-1/2}\exp\left\{ \frac{-1}{2}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)^{\intercal}\mathit{\Sigma}^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right\} 
\end{aligned}
$$

::: {.definition #unnamed-chunk-3}
probability density function (PDF) of multivariate normal distribution (= multivariate Gaussian distribution)
:::

$$ 
\mathcal{N}\left(\boldsymbol{x}\mid\boldsymbol{\mu},\mathit{\Sigma}\right)=f_{\boldsymbol{X}}\left(\boldsymbol{x}\right)=\left(\left|\mathit{\Sigma}\right|\left(2\pi\right)^{p}\right)^{-1/2}\exp\left\{ \frac{-1}{2}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)^{\intercal}\mathit{\Sigma}^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right\} 
$$


::: {.definition #unnamed-chunk-4}
correlation coefficient
:::

$$
\rho_{ij}=\dfrac{\sigma_{ij}}{\sqrt{\sigma_{ii}}\sqrt{\sigma_{jj}}}=\dfrac{\sigma_{ij}}{\sqrt{\sigma_{i}^{2}}\sqrt{\sigma_{j}^{2}}}=\dfrac{\sigma_{ij}}{\sigma_{i}\sigma_{j}}=\dfrac{\mathrm{V}\left(X_{i},X_{j}\right)}{\sqrt{\mathrm{V}\left(X_{i}\right)}\sqrt{\mathrm{V}\left(X_{j}\right)}}=\mathrm{R}\left(X_{i},X_{j}\right)
$$

## bivariate normal distribution

$p=2$ is the case of bivariate normal distribution

$$
\mathit{\Sigma}=\left[\sigma_{ij}\right]_{2\times2}=\begin{bmatrix}\sigma_{11} & \sigma_{12}\\
\sigma_{21} & \sigma_{22}
\end{bmatrix}=\begin{bmatrix}\sigma_{1}^{2} & \sigma_{12}\\
\sigma_{21} & \sigma_{2}^{2}
\end{bmatrix}=\begin{bmatrix}\sigma_{1}^{2} & \sigma_{1}\sigma_{2}\rho_{12}\\
\sigma_{2}\sigma_{1}\rho_{21} & \sigma_{2}^{2}
\end{bmatrix}=\begin{bmatrix}\sigma_{1}^{2} & \sigma_{1}\sigma_{2}\rho\\
\sigma_{2}\sigma_{1}\rho & \sigma_{2}^{2}
\end{bmatrix}
$$

$$
\rho_{12}=\rho=\rho_{21}
$$

$$
\left|\mathit{\Sigma}\right|=\begin{vmatrix}\sigma_{1}^{2} & \sigma_{1}\sigma_{2}\rho_{12}\\
\sigma_{2}\sigma_{1}\rho_{21} & \sigma_{2}^{2}
\end{vmatrix}=\sigma_{1}^{2}\sigma_{2}^{2}\left(1-\rho_{12}\rho_{21}\right)=\sigma_{1}^{2}\sigma_{2}^{2}\left(1-\rho^{2}\right)
$$

$$
\left[\begin{array}{ll}
a & b\\
c & d
\end{array}\right]^{-1}=\frac{1}{\begin{vmatrix}a & b\\
c & d
\end{vmatrix}}\left[\begin{array}{cc}
d & -b\\
-c & a
\end{array}\right]
$$

$$
\begin{aligned}
\mathit{\Sigma}^{-1}= & \frac{1}{\left|\mathit{\Sigma}\right|}\left[\begin{array}{cc}
\sigma_{2}^{2} & -\sigma_{1}\sigma_{2}\rho\\
-\sigma_{2}\sigma_{1}\rho & \sigma_{1}^{2}
\end{array}\right]\\
= & \frac{1}{\sigma_{1}^{2}\sigma_{2}^{2}\left(1-\rho^{2}\right)}\left[\begin{array}{cc}
\sigma_{2}^{2} & -\sigma_{1}\sigma_{2}\rho\\
-\sigma_{2}\sigma_{1}\rho & \sigma_{1}^{2}
\end{array}\right]\\
= & \frac{1}{\left(1-\rho^{2}\right)}\left[\begin{array}{cc}
\dfrac{1}{\sigma_{1}^{2}} & \dfrac{-\rho}{\sigma_{1}\sigma_{2}}\\
\dfrac{-\rho}{\sigma_{2}\sigma_{1}} & \dfrac{1}{\sigma_{2}^{2}}
\end{array}\right]
\end{aligned}
$$

$$
\begin{aligned}
 & \mathcal{N}\left(\boldsymbol{x}=\begin{bmatrix}x_{1}\\
x_{2}
\end{bmatrix} \middle| \boldsymbol{\mu}=\begin{bmatrix}\mu_{1}\\
\mu_{2}
\end{bmatrix},\mathit{\Sigma}=\begin{bmatrix}\sigma_{1}^{2} & \sigma_{1}\sigma_{2}\rho\\
\sigma_{2}\sigma_{1}\rho & \sigma_{2}^{2}
\end{bmatrix}\right)\\
= & \left(\left|\mathit{\Sigma}\right|\left(2\pi\right)^{p=2}\right)^{-1/2}\exp\left\{ \frac{-1}{2}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)^{\intercal}\mathit{\Sigma}^{-1}\left(\boldsymbol{x}-\boldsymbol{\mu}\right)\right\} \\
= & \left(\sigma_{1}^{2}\sigma_{2}^{2}\left(1-\rho^{2}\right)\left(2\pi\right)^{2}\right)^{-1/2}\exp\left\{ \frac{-1}{2}\begin{bmatrix}x_{1}-\mu_{1}\\
x_{2}-\mu_{2}
\end{bmatrix}^{\intercal}\mathit{\Sigma}^{-1}\begin{bmatrix}x_{1}-\mu_{1}\\
x_{2}-\mu_{2}
\end{bmatrix}\right\} \\
= & \dfrac{1}{2\pi\sigma_{1}\sigma_{2}\sqrt{1-\rho^{2}}}\exp\left\{ \frac{-1}{2}\begin{bmatrix}x_{1}-\mu_{1}\\
x_{2}-\mu_{2}
\end{bmatrix}^{\intercal}\frac{1}{\left(1-\rho^{2}\right)}\left[\begin{array}{cc}
\dfrac{1}{\sigma_{1}^{2}} & \dfrac{-\rho}{\sigma_{1}\sigma_{2}}\\
\dfrac{-\rho}{\sigma_{2}\sigma_{1}} & \dfrac{1}{\sigma_{2}^{2}}
\end{array}\right]\begin{bmatrix}x_{1}-\mu_{1}\\
x_{2}-\mu_{2}
\end{bmatrix}\right\} \\
= & \dfrac{1}{2\pi\sigma_{1}\sigma_{2}\sqrt{1-\rho^{2}}}\exp\left\{ \frac{-1}{2\left(1-\rho^{2}\right)}\begin{bmatrix}x_{1}-\mu_{1}\\
x_{2}-\mu_{2}
\end{bmatrix}^{\intercal}\left[\begin{array}{cc}
\dfrac{1}{\sigma_{1}^{2}} & \dfrac{-\rho}{\sigma_{1}\sigma_{2}}\\
\dfrac{-\rho}{\sigma_{2}\sigma_{1}} & \dfrac{1}{\sigma_{2}^{2}}
\end{array}\right]\begin{bmatrix}x_{1}-\mu_{1}\\
x_{2}-\mu_{2}
\end{bmatrix}\right\} \\
= & \dfrac{1}{2\pi\sigma_{1}\sigma_{2}\sqrt{1-\rho^{2}}}\exp\left\{ \frac{-1}{2\left(1-\rho^{2}\right)}\left[\left(\dfrac{x_{1}-\mu_{1}}{\sigma_{1}}\right)^{2}-2\rho\left(\dfrac{x_{1}-\mu_{1}}{\sigma_{1}}\right)\left(\dfrac{x_{2}-\mu_{2}}{\sigma_{2}}\right)+\left(\dfrac{x_{2}-\mu_{2}}{\sigma_{2}}\right)^{2}\right]\right\} 
\end{aligned}
$$

::: {.definition #unnamed-chunk-5}
probability density function (PDF) of bivariate normal distribution (= bivariate Gaussian distribution)
:::

$$
\begin{aligned}
 & \mathcal{N}\left(\begin{bmatrix}x_{1}\\
x_{2}
\end{bmatrix} \middle| \begin{bmatrix}\mu_{1}\\
\mu_{2}
\end{bmatrix},\begin{bmatrix}\sigma_{1}^{2} & \sigma_{1}\sigma_{2}\rho\\
\sigma_{2}\sigma_{1}\rho & \sigma_{2}^{2}
\end{bmatrix}\right)\\
= & \dfrac{1}{2\pi\sigma_{1}\sigma_{2}\sqrt{1-\rho^{2}}}\exp\left\{ \frac{-1}{2\left(1-\rho^{2}\right)}\left[\left(\dfrac{x_{1}-\mu_{1}}{\sigma_{1}}\right)^{2}-2\rho\left(\dfrac{x_{1}-\mu_{1}}{\sigma_{1}}\right)\left(\dfrac{x_{2}-\mu_{2}}{\sigma_{2}}\right)+\left(\dfrac{x_{2}-\mu_{2}}{\sigma_{2}}\right)^{2}\right]\right\} 
\end{aligned}
$$
