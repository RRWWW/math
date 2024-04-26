# autoregression in time series

::: {show-in="html"}
張翔老師. 2015. “ARMA Part1.” https://www.youtube.com/watch?v=G-0dR57W-fo.

張翔老師. 2015. “ARMA Part2.” https://www.youtube.com/watch?v=fQaZzO7E6FE.

張翔老師. 2015. “ARMA Part3.” https://www.youtube.com/watch?v=Ocw4NXoO8Xo.
:::

::: {show-in="pdf"}
\begin{CJK}{UTF8}{bsmi}
張翔老師. 2015. “ARMA Part1.” https://www.youtube.com/watch?v=G-0dR57W-fo.

張翔老師. 2015. “ARMA Part2.” https://www.youtube.com/watch?v=fQaZzO7E6FE.

張翔老師. 2015. “ARMA Part3.” https://www.youtube.com/watch?v=Ocw4NXoO8Xo.
\end{CJK}
:::

time series [data]

$$
\cdots,Y_{t-2},Y_{t-1},Y_{t},Y_{t+1},Y_{t+2},\cdots
$$

- lag
  - $1^\text{st}$ lag = lag $1$
    $$
    Y_{t-1}
    $$
  - $k^\text{th}$ lag = lag $k$
    $$
    Y_{t-k}
    $$

$1^\text{st}$ difference

$$
\Delta Y_{t}=Y_{t}-Y_{t-1}
$$ approximation for RoR = rate of return

$$
\begin{aligned}
\Delta\ln Y_{t}=\ln Y_{t}-\ln Y_{t-1}= & \ln\dfrac{Y_{t}}{Y_{t-1}}=\ln\left(1+\dfrac{Y_{t}-Y_{t-1}}{Y_{t-1}}\right)\\
= & \dfrac{Y_{t}-Y_{t-1}}{Y_{t-1}}+\mathrm{O}\left(\left(\dfrac{Y_{t}-Y_{t-1}}{Y_{t-1}}\right)^{2}\right)\\
\approx & \dfrac{Y_{t}-Y_{t-1}}{Y_{t-1}}=\mathrm{RoR}
\end{aligned}
$$

$$
\begin{cases}
\ln(1+x)=\sum\limits _{n=1}^{\infty}(-1)^{n+1}\dfrac{x^{n}}{n}=x-\frac{x^{2}}{2}+\frac{x^{3}}{3}-\cdots\\
\ln(1-x)=-\sum\limits _{n=1}^{\infty}\dfrac{x^{n}}{n}=-x-\frac{x^{2}}{2}-\frac{x^{3}}{3}-\cdots
\end{cases}
$$

$$
\begin{aligned}
\frac{1}{1+t}= & 1-t+t^{2}-t^{3}+\cdots\\
\ln(1+x)= & \int_{0}^{x}\frac{1}{1+t}dt\\
= & x-\frac{x^{2}}{2}+\frac{x^{3}}{3}-\frac{x^{4}}{4}+\cdots
\end{aligned}
$$

::: {.definition #unnamed-chunk-1}
autocorrelation = serial correlation
:::

$$
\exists t_{1}\ne t_{2}\left[\mathrm{V}\left(Y_{t_{1}},Y_{t_{2}}\right)\ne0\right]
$$


$$
\begin{cases}
\mathrm{E}\left(Y_{t}\right)\triangleq\mu_{t}\\
\mathrm{V}\left(Y_{t}\right)\triangleq\sigma_{t}^{2}
\end{cases}
$$

::: {.definition #unnamed-chunk-2}
$k^\text{th}$ order autocovariance
:::

$$
\mathrm{V}\left(Y_{t},Y_{t-k}\right)\triangleq\gamma\left(t,k\right)
$$

$$
\sigma_{t}^{2}\triangleq\mathrm{V}\left(Y_{t}\right)=\mathrm{V}\left(Y_{t},Y_{t}\right)=\mathrm{V}\left(Y_{t},Y_{t-0}\right)=\gamma\left(t,k=0\right)=\gamma\left(t,0\right)
$$

::: {.definition #unnamed-chunk-3}
$k^\text{th}$ order autocorrelation
:::

$$
\rho_{t,t-k}=\dfrac{\sigma_{t,t-k}}{\sqrt{\sigma_{tt}}\sqrt{\sigma_{t-k,t-k}}}=\dfrac{\sigma_{t,t-k}}{\sqrt{\sigma_{t}^{2}}\sqrt{\sigma_{t-k}^{2}}}=\dfrac{\sigma_{t,t-k}}{\sigma_{t}\sigma_{t-k}}=\dfrac{\mathrm{V}\left(Y_{t},Y_{t-k}\right)}{\sqrt{\mathrm{V}\left(Y_{t}\right)}\sqrt{\mathrm{V}\left(Y_{t-k}\right)}}\triangleq\mathrm{R}\left(Y_{t},Y_{t-k}\right)\triangleq\rho\left(t,k\right)
$$


::: {.definition #unnamed-chunk-4}
stationary time series
:::

$$
\begin{cases}
\mathrm{E}\left(Y_{t}\right)\triangleq\mu_{t}=\mu & \left(1\right)\text{independent of }t\\
\mathrm{V}\left(Y_{t}\right)\triangleq\sigma_{t}^{2}=\sigma^{2}<\infty & \left(2\right)\text{independent of }t\\
\mathrm{V}\left(Y_{t},Y_{t-k}\right)\triangleq\gamma\left(t,k\right)=\gamma\left(k\right) & \left(3\right)\text{independent of }t
\end{cases}
$$

properties

$$
\begin{cases}
\mathrm{V}\left(Y_{t}\right)\triangleq\sigma_{t}^{2}=\gamma\left(t,k=0\right)=\gamma\left(k=0\right)\overset{\left(3\right)}{=}\gamma\left(0\right)\triangleq\gamma_{0}\overset{\left(2\right)}{=}\sigma^{2} & \left(4\right)\Rightarrow\mathrm{V}\left(Y_{t-k}\right)=\gamma\left(0\right)\\
\mathrm{R}\left(Y_{t},Y_{t-k}\right)\triangleq\rho\left(t,k\right)\triangleq\dfrac{\mathrm{V}\left(Y_{t},Y_{t-k}\right)}{\sqrt{\mathrm{V}\left(Y_{t}\right)}\sqrt{\mathrm{V}\left(Y_{t-k}\right)}}\\
=\dfrac{\gamma\left(t,k\right)}{\sqrt{\gamma\left(0\right)}\sqrt{\gamma\left(0\right)}}\overset{\left(3\right)}{\underset{\left(4\right)}{=}}\dfrac{\gamma\left(k\right)}{\gamma\left(0\right)}\triangleq\dfrac{\gamma_{k}}{\gamma_{0}}\triangleq\rho\left(k\right)\triangleq\rho_{k} & \left(5\right)\\
\gamma\left(k\right)=\gamma\left(-k\right) & \left(6\right)\Rightarrow\rho\left(k\right)=\rho\left(-k\right)
\end{cases}
$$

$$
\gamma\left(k\right)\overset{\left(3\right)}{=}\mathrm{V}\left(Y_{t},Y_{t-k}\right)=\mathrm{V}\left(Y_{t-k},Y_{t}\right)=\mathrm{V}\left(Y_{t^{\prime}},Y_{t^{\prime}+k}\right)=\mathrm{V}\left(Y_{t^{\prime}},Y_{t^{\prime}-\left(-k\right)}\right)\overset{\left(3\right)}{=}\gamma\left(-k\right)\Rightarrow\left(6\right)
$$

point estimation

$$
\begin{cases}
\widehat{\mathrm{E}}\left(Y_{t}\right)\triangleq\overline{Y}\triangleq\widehat{\mu}=\dfrac{1}{T}\sum\limits _{t=1}^{T}Y_{t} & \rightarrow\mathrm{E}\left(Y_{t}\right)=\mu\\
\widehat{\mathrm{V}}\left(Y_{t}\right)\triangleq\widehat{\gamma}_{0}=\dfrac{1}{T}\sum\limits _{t=1}^{T}\left(Y_{t}-\overline{Y}\right)^{2} & \rightarrow\mathrm{V}\left(Y_{t}\right)=\sigma^{2}=\gamma_{0}\\
\widehat{\mathrm{V}}\left(Y_{t},Y_{t-k}\right)\triangleq\widehat{\gamma}_{k}\\
=\dfrac{1}{T}\sum\limits _{t=k+1}^{T}\left(Y_{t}-\overline{Y}\right)\left(Y_{t-k}-\overline{Y}\right)=\dfrac{1}{T}\sum\limits _{t=1}^{T-k}\left(Y_{t}-\overline{Y}\right)\left(Y_{t+k}-\overline{Y}\right) & \rightarrow\mathrm{V}\left(Y_{t},Y_{t-k}\right)=\gamma_{k}\\
\dfrac{\widehat{\mathrm{V}}\left(Y_{t},Y_{t-k}\right)}{\sqrt{\mathrm{\widehat{\mathrm{V}}}\left(Y_{t}\right)}\sqrt{\mathrm{\widehat{\mathrm{V}}}\left(Y_{t-k}\right)}}\triangleq\widehat{\rho}_{k}=\dfrac{\widehat{\gamma}_{k}}{\widehat{\gamma}_{0}}=\dfrac{\dfrac{1}{T}\sum\limits _{t=k+1}^{T}\left(Y_{t}-\overline{Y}\right)\left(Y_{t-k}-\overline{Y}\right)}{\dfrac{1}{T}\sum\limits _{t=1}^{T}\left(Y_{t}-\overline{Y}\right)^{2}} & \rightarrow\mathrm{R}\left(Y_{t},Y_{t-k}\right)=\rho_{k}
\end{cases}
$$

$$
Y_{1}Y_{1+k}+Y_{2}Y_{2+k}+\cdot\cdots+Y_{t}Y_{t+k}+\cdot\cdots+Y_{T-k}Y_{T}
$$

$1^\text{st}$-order autocorrelation estimation

$$
\widehat{\rho}_{1}=\dfrac{\widehat{\gamma}_{1}}{\widehat{\gamma}_{0}}=\dfrac{\dfrac{1}{T}\sum\limits _{t=1+1=2}^{T}\left(Y_{t}-\overline{Y}\right)\left(Y_{t-1}-\overline{Y}\right)}{\dfrac{1}{T}\sum\limits _{t=1}^{T}\left(Y_{t}-\overline{Y}\right)^{2}}
$$

## AR(1) = $1^\text{st}$-order autoregressive model = first-order autoregressive model

::: {show-in="html"}
張翔老師. 2015. “ARMA Part3.” https://www.youtube.com/watch?v=Ocw4NXoO8Xo.
:::

::: {show-in="pdf"}
\begin{CJK}{UTF8}{bsmi}
張翔老師. 2015. “ARMA Part3.” https://www.youtube.com/watch?v=Ocw4NXoO8Xo.
\end{CJK}
:::

::: {.definition #unnamed-chunk-5}
AR(1) = $1^\text{st}$-order autoregressive model$
:::

$$
Y_{t}=\beta_{0}+\beta_{1}Y_{t-1}+\mathcal{E}_{t}
$$

$$
\mathcal{E}_{t}\sim\mathcal{N}\left(0,\sigma_{\mathcal{E}}^{2}\right)
$$
$$
\begin{aligned}
Y_{t}= & \beta_{0}+\beta_{1}Y_{t-1}+\mathcal{E}_{t}\\
= & \beta_{0}+\beta_{1}\left(\beta_{0}+\beta_{1}Y_{t-2}+\mathcal{E}_{t-1}\right)+\mathcal{E}_{t}\\
= & \beta_{0}\left(1+\beta_{1}\right)+\beta_{1}^{2}Y_{t-2}+\mathcal{E}_{t}+\beta_{1}\mathcal{E}_{t-1}\\
= & \beta_{0}\left(1+\beta_{1}\right)+\beta_{1}^{2}\left(\beta_{0}+\beta_{1}Y_{t-3}+\mathcal{E}_{t-2}\right)+\mathcal{E}_{t}+\beta_{1}\mathcal{E}_{t-1}\\
= & \beta_{0}\left(1+\beta_{1}+\beta_{1}^{2}\right)+\beta_{1}^{3}Y_{t-3}+\mathcal{E}_{t}+\beta_{1}\mathcal{E}_{t-1}+\beta_{1}^{2}\mathcal{E}_{t-2}\\
\vdots\\
= & \beta_{0}\left(1+\beta_{1}+\beta_{1}^{2}+\cdots\right)+\mathcal{E}_{t}+\beta_{1}\mathcal{E}_{t-1}+\beta_{1}^{2}\mathcal{E}_{t-2}+\cdots\\
\overset{\left|\beta_{1}\right|<1}{=} & \dfrac{\beta_{0}}{1-\beta_{1}}+\sum_{k=0}^{\infty}\beta_{1}^{k}\mathcal{E}_{t-k}
\end{aligned}
$$

$$
\begin{cases}
\mu=\mathrm{E}\left(Y_{t}\right)=\mathrm{E}\left(\dfrac{\beta_{0}}{1-\beta_{1}}+\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-i}\right)\\
=\dfrac{\beta_{0}}{1-\beta_{1}}+\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathrm{E}\left(\mathcal{E}_{t-i}\right)\overset{\mathcal{E}_{t}\sim\mathcal{N}\left(0,\sigma_{\mathcal{E}}^{2}\right)}{=}\dfrac{\beta_{0}}{1-\beta_{1}} & \mu=\dfrac{\beta_{0}}{1-\beta_{1}}\\
\gamma_{0}=\sigma^{2}=\mathrm{V}\left(Y_{t}\right)=\mathrm{V}\left(\mu+\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-i}\right)=\mathrm{V}\left(\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-i}\right)\\
=\sum_{i=0}^{\infty}\left(\beta_{1}^{i}\right)^{2}\mathrm{V}\left(\mathcal{E}_{t-i}\right)\overset{\mathcal{E}_{t}\sim\mathcal{N}\left(0,\sigma_{\mathcal{E}}^{2}\right)}{=}\sum\limits _{i=0}^{\infty}\left(\beta_{1}^{2}\right)^{i}\sigma_{\mathcal{E}}^{2}=\dfrac{\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}} & \gamma_{0}=\sigma^{2}=\dfrac{\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}\\
\gamma_{k}=\mathrm{V}\left(Y_{t},Y_{t-k}\right)=\mathrm{V}\left(\mu+\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-i},\mu+\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-k-i}\right)\\
=\mathrm{V}\left(\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-i},\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-k-i}\right)=\cdots & \gamma_{k}=\dfrac{\beta_{1}^{k}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}\\
\rho_{k}=\mathrm{R}\left(Y_{t},Y_{t-k}\right)=\dfrac{\gamma_{k}}{\gamma_{0}}=\dfrac{\dfrac{\beta_{1}^{k}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}}{\dfrac{\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}}=\beta_{1}^{k} & \rho_{k}=\dfrac{\gamma_{k}}{\gamma_{0}}=\beta_{1}^{k}
\end{cases}
$$

$$
\rho_{1}=\dfrac{\gamma_{1}}{\gamma_{0}}=\beta_{1}^{1}=\beta_{1}
$$

$$
\begin{aligned}
\gamma_{k}=\mathrm{V}\left(Y_{t},Y_{t-k}\right)= & \mathrm{V}\left(\mu+\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-i},\mu+\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-k-i}\right)\\
= & \mathrm{V}\left(\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-i},\sum\limits _{i=0}^{\infty}\beta_{1}^{i}\mathcal{E}_{t-k-i}\right)=\cdots
\end{aligned}
$$

$$
\boldsymbol{Y}=\left\langle Y_{1},Y_{2},\cdots,Y_{T}\right\rangle =\begin{bmatrix}Y_{1} & Y_{2} & \cdots & Y_{T}\end{bmatrix}^{\mathrm{T}}=\begin{bmatrix}Y_{1}\\
Y_{2}\\
\vdots\\
Y_{T}
\end{bmatrix}
$$

AR(1) covariance matrix

by \@ref(eq:covmatrix)

$$
\begin{aligned}
\mathrm{V}\left(\boldsymbol{Y}\right)= & \mathrm{E}\left[\left[\boldsymbol{Y}-\mathrm{E}\left(\boldsymbol{Y}\right)\right]\left[\boldsymbol{Y}-\mathrm{E}\left(\boldsymbol{Y}\right)\right]^{\mathrm{T}}\right]\\
= & \begin{bmatrix}\sigma_{1}^{2} & \sigma_{12} & \cdots & \sigma_{1T}\\
\sigma_{21} & \sigma_{2}^{2} & \cdots & \sigma_{2T}\\
\vdots & \vdots & \ddots & \vdots\\
\sigma_{T1} & \sigma_{T2} & \cdots & \sigma_{T}^{2}
\end{bmatrix}=\begin{bmatrix}\sigma_{11} & \sigma_{12} & \cdots & \sigma_{1T}\\
\sigma_{21} & \sigma_{22} & \cdots & \sigma_{2T}\\
\vdots & \vdots & \ddots & \vdots\\
\sigma_{T1} & \sigma_{T2} & \cdots & \sigma_{TT}
\end{bmatrix}=\left[\sigma_{ij}\right]_{T\times T}=\mathit{\Sigma}\\
= & \begin{bmatrix}\gamma_{0} & \gamma_{1} & \cdots & \gamma_{T-1}\\
\gamma_{1} & \gamma_{0} & \cdots & \gamma_{T-2}\\
\vdots & \vdots & \ddots & \vdots\\
\gamma_{T-1} & \gamma_{T-2} & \cdots & \gamma_{0}
\end{bmatrix}=\begin{bmatrix}\dfrac{\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}} & \dfrac{\beta_{1}^{1}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}} & \cdots & \dfrac{\beta_{1}^{T-1}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}\\
\dfrac{\beta_{1}^{1}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}} & \dfrac{\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}} & \cdots & \dfrac{\beta_{1}^{T-2}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}\\
\vdots & \vdots & \ddots & \vdots\\
\dfrac{\beta_{1}^{T-1}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}} & \dfrac{\beta_{1}^{T-2}\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}} & \cdots & \dfrac{\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}
\end{bmatrix}\\
= & \dfrac{\sigma_{\mathcal{E}}^{2}}{1-\beta_{1}^{2}}\begin{bmatrix}1 & \beta_{1} & \cdots & \beta_{1}^{T-1}\\
\beta_{1} & 1 & \cdots & \beta_{1}^{T-2}\\
\vdots & \vdots & \ddots & \vdots\\
\beta_{1}^{T-1} & \beta_{1}^{T-2} & \cdots & 1
\end{bmatrix}=\sigma^{2}\begin{bmatrix}1 & \beta_{1} & \beta_{1}^{2} & \cdots & \beta_{1}^{T-1}\\
\beta_{1} & 1 & \beta_{1} & \cdots & \beta_{1}^{T-2}\\
\beta_{1}^{2} & \beta_{1} & 1 & \cdots & \beta_{1}^{T-3}\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
\beta_{1}^{T-1} & \beta_{1}^{T-2} & \beta_{1}^{T-3} & \cdots & 1
\end{bmatrix}\\
= & \sigma^{2}\begin{bmatrix}1 & \rho_{1} & \rho_{2} & \cdots & \rho_{T-1}\\
\rho_{1} & 1 & \rho_{1} & \cdots & \rho_{T-2}\\
\rho_{2} & \rho_{1} & 1 & \cdots & \rho_{T-3}\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
\rho_{T-1} & \rho_{T-2} & \rho_{T-3} & \cdots & 1
\end{bmatrix}=\sigma^{2}\begin{bmatrix}1 & \rho & \rho^{2} & \cdots & \rho^{T-1}\\
\rho & 1 & \rho & \cdots & \rho^{T-2}\\
\rho^{2} & \rho & 1 & \cdots & \rho^{T-3}\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
\rho^{T-1} & \rho^{T-2} & \rho^{T-3} & \cdots & 1
\end{bmatrix}
\end{aligned}
$$

$$
\boldsymbol{Y}\sim\mathcal{D}\left(\boldsymbol{\mu},\mathit{\Sigma}\right)=\mathrm{d}\left(\boldsymbol{\mu}_{\boldsymbol{Y}},\mathit{\Sigma}_{\boldsymbol{Y}}\right)=\mathrm{d}\left(\mathrm{E}\left[\boldsymbol{Y}\right],\mathrm{V}\left[\boldsymbol{Y}\right]\right)
$$

where

$$
\mathit{\Sigma}=\begin{bmatrix}\gamma_{0} & \gamma_{1} & \cdots & \gamma_{T-1}\\
\gamma_{1} & \gamma_{0} & \cdots & \gamma_{T-2}\\
\vdots & \vdots & \ddots & \vdots\\
\gamma_{T-1} & \gamma_{T-2} & \cdots & \gamma_{0}
\end{bmatrix}=\sigma^{2}\begin{bmatrix}1 & \rho & \rho^{2} & \cdots & \rho^{T-1}\\
\rho & 1 & \rho & \cdots & \rho^{T-2}\\
\rho^{2} & \rho & 1 & \cdots & \rho^{T-3}\\
\vdots & \vdots & \vdots & \ddots & \vdots\\
\rho^{T-1} & \rho^{T-2} & \rho^{T-3} & \cdots & 1
\end{bmatrix}
$$

## AR(2) = $2^\text{nd}$-order autoregressive model = second-order autoregressive model

::: {.definition #unnamed-chunk-6}
AR(2) = $2^\text{nd}$-order autoregressive model
:::

$$
Y_{t}=\beta_{0}+\beta_{1}Y_{t-1}+\beta_{2}Y_{t-2}+\mathcal{E}_{t}
$$

$$
\mathcal{E}_{t}\sim\mathcal{N}\left(0,\sigma_{\mathcal{E}}^{2}\right)
$$

## AR($p$) = $p^\text{th}$-order autoregressive model

$$
Y_{t}=\beta_{0}+\sum_{i=1}^{p}\beta_{i}Y_{t-i}+\mathcal{E}_{t}
$$

## MA($q$) = $q^\text{th}$-order moving-average model

$$
Y_{t}=\mu+\mathcal{E}_{t}+\sum_{i=1}^{q}\alpha_{i}\mathcal{E}_{t-i}
$$


## ARMA($p$,$q$) = $p^\text{th},q^\text{th}$-order autoregressive-moving-average model

$$
Y_{t}=\mathcal{E}_{t}+\sum_{i=1}^{q}\alpha_{i}\mathcal{E}_{t-i}+\sum_{i=1}^{p}\beta_{i}Y_{t-i}
$$