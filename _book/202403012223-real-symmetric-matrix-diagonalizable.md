# real symmetric matrix diagonalizable

::: {show-in="html"}

https://ccjou.wordpress.com/2011/02/09/實對稱矩陣可正交對角化的證明/

:::

::: {show-in="pdf"}

\begin{CJK}{UTF8}{bsmi}
https://ccjou.wordpress.com/2011/02/09/實對稱矩陣可正交對角化的證明/
\end{CJK}

:::

https://tex.stackexchange.com/questions/30619/what-is-the-best-symbol-for-vector-matrix-transpose

::: {.theorem #real-sym-real-eigen}

::: {show-in="html"}

實對稱矩陣的特徵值皆是實數，且對應特徵向量是實向量。

$$
\begin{array}{c}
\begin{cases}
\begin{cases}
A\in\mathcal{M}_{n\times n}\left(\mathbb{R}\right) & \text{real matrix}\\
A^{\intercal}=A & \text{symmetric matrix}
\end{cases} & \text{real symmetric matrix}\\
A\boldsymbol{x}=\lambda\boldsymbol{x} & \begin{cases}
\lambda\in\mathbb{C} & \text{complex eigenvalue}\\
\boldsymbol{0}\ne\boldsymbol{x}\in\mathbb{C}^{n} & \text{complex eigenvector}
\end{cases}
\end{cases}\\
\Downarrow\\
\begin{cases}
\lambda\in\mathbb{R} & \text{real eigenvalue}\left(1\right)\\
\boldsymbol{x}\in\mathbb{R}^{n} & \text{real eigenvector}\left(2\right)
\end{cases}
\end{array}
$$

:::

::: {show-in="pdf"}

\begin{CJK}{UTF8}{bsmi}
實對稱矩陣的特徵值皆是實數，且對應特徵向量是實向量。
\end{CJK}

$$
\begin{array}{c}
\begin{cases}
\begin{cases}
A\in\mathcal{M}_{n\times n}\left(\mathbb{R}\right) & \textup{real matrix}\\
A^{\intercal}=A & \textup{symmetric matrix}
\end{cases} & \textup{real symmetric matrix}\\
A\boldsymbol{x}=\lambda\boldsymbol{x} & \begin{cases}
\lambda\in\mathbb{C} & \textup{complex eigenvalue}\\
\boldsymbol{0}\ne\boldsymbol{x}\in\mathbb{C}^{n} & \textup{complex eigenvector}
\end{cases}
\end{cases}\\
\Downarrow\\
\begin{cases}
\lambda\in\mathbb{R} & \textup{real eigenvalue}\left(1\right)\\
\boldsymbol{x}\in\mathbb{R}^{n} & \textup{real eigenvector}\left(2\right)
\end{cases}
\end{array}
$$

:::

:::

::: {.proof}
$\left(1\right)$

$$
\begin{aligned}
A\boldsymbol{x}= & \lambda\boldsymbol{x}\\
\overline{A}\overline{\boldsymbol{x}}=\overline{A\boldsymbol{x}}= & \overline{\lambda\boldsymbol{x}}=\overline{\lambda}\overline{\boldsymbol{x}}\\
\overline{\boldsymbol{x}}^{\intercal}\overline{A}^{\intercal}=\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}= & \left(\overline{\lambda}\overline{\boldsymbol{x}}\right)^{\intercal}=\overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\\
\overline{\boldsymbol{x}}^{\intercal}A\overset{\text{symmetric}}{=}\overline{\boldsymbol{x}}^{\intercal}A^{\intercal}\overset{\text{real}}{=}\\
\overline{\boldsymbol{x}}^{\intercal}A= & \overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\\
\lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}=\overline{\boldsymbol{x}}^{\intercal}\left(\lambda\boldsymbol{x}\right)\underset{A\boldsymbol{x}=\lambda\boldsymbol{x}}{\overset{\cdot\boldsymbol{x}}{=}}\overline{\boldsymbol{x}}^{\intercal}A\boldsymbol{x}= & \overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}= & \overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\left(\lambda-\overline{\lambda}\right)\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}= & 0\wedge\begin{cases}
\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}=\sum\limits _{i=1}^{n}\left|x_{i}\right|^{2}\\
\boldsymbol{x}\ne\boldsymbol{0}
\end{cases}\Rightarrow\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\ne0\\
\lambda-\overline{\lambda}= & 0\\
\lambda= & \overline{\lambda}\Leftrightarrow\lambda\in\mathbb{R}
\end{aligned}
$$
:::

::: {.proof}
$\left(1\right)$ fast concept

::: {show-in="html"}

$$
\begin{aligned}
\color{orange}{\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}}=\left(\overline{\boldsymbol{x}}^{\intercal}\overline{A}^{\intercal}\right)\boldsymbol{x}\overset{\text{symmetric}}{=} & \left(\overline{\boldsymbol{x}}^{\intercal}\overline{A}\right)\boldsymbol{x}=\color{orange}{\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}\\
\left(L\right)=\color{orange}{\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}=} & \color{orange}{\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}=\left(R\right)\\
\left(L\right)=\color{orange}{\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}}\overset{A\boldsymbol{x}=\lambda\boldsymbol{x}}{=} & \left(\overline{\lambda}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}=\overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\left(R\right)=\color{orange}{\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}\overset{\text{real}}{=}\overline{\boldsymbol{x}}^{\intercal}\left(A\boldsymbol{x}\right)\overset{A\boldsymbol{x}=\lambda\boldsymbol{x}}{=} & \overline{\boldsymbol{x}}^{\intercal}\left(\lambda\boldsymbol{x}\right)=\lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}=\color{orange}{\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}=} & \color{orange}{\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}=\lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}= & \lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}
\end{aligned}
$$

:::

::: {show-in="pdf"}

$$
\begin{aligned}
{\color{orange}\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}}=\left(\overline{\boldsymbol{x}}^{\intercal}\overline{A}^{\intercal}\right)\boldsymbol{x}\overset{\text{symmetric}}{=} & \left(\overline{\boldsymbol{x}}^{\intercal}\overline{A}\right)\boldsymbol{x}={\color{orange}\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}\\
\left(L\right)={\color{orange}\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}=} & {\color{orange}\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}=\left(R\right)\\
\left(L\right)={\color{orange}\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}}\overset{A\boldsymbol{x}=\lambda\boldsymbol{x}}{=} & \left(\overline{\lambda}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}=\overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\left(R\right)={\color{orange}\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}\overset{\text{real}}{=}\overline{\boldsymbol{x}}^{\intercal}\left(A\boldsymbol{x}\right)\overset{A\boldsymbol{x}=\lambda\boldsymbol{x}}{=} & \overline{\boldsymbol{x}}^{\intercal}\left(\lambda\boldsymbol{x}\right)=\lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}={\color{orange}\left(\overline{A}\overline{\boldsymbol{x}}\right)^{\intercal}\boldsymbol{x}=} & {\color{orange}\overline{\boldsymbol{x}}^{\intercal}\left(\overline{A}\boldsymbol{x}\right)}=\lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}\\
\overline{\lambda}\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}= & \lambda\overline{\boldsymbol{x}}^{\intercal}\boldsymbol{x}
\end{aligned}
$$

:::

:::

::: {.proof}
$\left(2\right)$

???
  
::: {show-in="html"}

推論特徵空間 $N(A-\lambda I)$ ($A-\lambda I$ 的零空間) 為 $\mathbb{R}^n$ 的子空間，故 $\boldsymbol{x}\in N(A-\lambda I)$  是一個非零實向量。

:::

::: {show-in="pdf"}

\begin{CJK}{UTF8}{bsmi}
推論特徵空間 $N(A-\lambda I)$ ($A-\lambda I$ 的零空間) 為 $\mathbb{R}^n$ 的子空間，故 $\boldsymbol{x}\in N(A-\lambda I)$  是一個非零實向量。
\end{CJK}

:::

:::

::: {.theorem #unnamed-chunk-4}

::: {show-in="html"}

實對稱矩陣對應相異特徵值的特徵向量互為正交。

$$
\begin{array}{c}
\begin{cases}
\begin{cases}
A\in\mathcal{M}_{n\times n}\left(\mathbb{R}\right) & \text{real matrix}\\
A^{\intercal}=A & \text{symmetric matrix}
\end{cases} & \text{real symmetric matrix}\\
A\boldsymbol{x}=\lambda\boldsymbol{x} & \ref{real-sym-real-eigen}\begin{cases}
\lambda\in\mathbb{R} & \text{real eigenvalue}\\
\boldsymbol{x}\in\mathbb{R}^{n} & \text{real eigenvector}
\end{cases}\\
\begin{cases}
A\boldsymbol{x}_{{\scriptscriptstyle 1}}=\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}} & \left(e_{{\scriptscriptstyle 1}}\right)\\
A\boldsymbol{x}_{{\scriptscriptstyle 2}}=\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 2}} & \left(e_{{\scriptscriptstyle 2}}\right)
\end{cases} & \lambda_{{\scriptscriptstyle 1}}\ne\lambda_{{\scriptscriptstyle 2}}
\end{cases}\\
\Downarrow\\
\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=0\Leftrightarrow\boldsymbol{x}_{{\scriptscriptstyle 1}}\perp\boldsymbol{x}_{{\scriptscriptstyle 2}}
\end{array}
$$

:::

::: {show-in="pdf"}

\begin{CJK}{UTF8}{bsmi}
實對稱矩陣對應相異特徵值的特徵向量互為正交。
\end{CJK}

$$
\begin{array}{c}
\begin{cases}
\begin{cases}
A\in\mathcal{M}_{n\times n}\left(\mathbb{R}\right) & \textup{real matrix}\\
A^{\intercal}=A & \textup{symmetric matrix}
\end{cases} & \textup{real symmetric matrix}\\
A\boldsymbol{x}=\lambda\boldsymbol{x} & \ref{thm:real-sym-real-eigen}\begin{cases}
\lambda\in\mathbb{R} & \textup{real eigenvalue}\\
\boldsymbol{x}\in\mathbb{R}^{n} & \textup{real eigenvector}
\end{cases}\\
\begin{cases}
A\boldsymbol{x}_{{\scriptscriptstyle 1}}=\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}} & \left(e_{{\scriptscriptstyle 1}}\right)\\
A\boldsymbol{x}_{{\scriptscriptstyle 2}}=\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 2}} & \left(e_{{\scriptscriptstyle 2}}\right)
\end{cases} & \lambda_{{\scriptscriptstyle 1}}\ne\lambda_{{\scriptscriptstyle 2}}
\end{cases}\\
\Downarrow\\
\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=0\Leftrightarrow\boldsymbol{x}_{{\scriptscriptstyle 1}}\perp\boldsymbol{x}_{{\scriptscriptstyle 2}}
\end{array}
$$

:::

:::

::: {.proof}
$\left(1\right)$

$$
\begin{aligned}
A\boldsymbol{x}_{{\scriptscriptstyle 2}}= & \lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A\boldsymbol{x}_{{\scriptscriptstyle 2}}\overset{\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\cdot}{=} & \boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 2}}=\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=\left(1\right)\\
A\boldsymbol{x}_{{\scriptscriptstyle 1}}= & \lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}\\
\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A^{\intercal}=\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}= & \left(\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}=\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\\
\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A^{\intercal}= & \lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\\
\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A\boldsymbol{x}_{{\scriptscriptstyle 2}}\overset{\text{symmetric}}{=}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\overset{\cdot\boldsymbol{x}_{{\scriptscriptstyle 2}}}{=} & \lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=\left(2\right)\\
\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\overset{\left(1\right)}{=}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A\boldsymbol{x}_{{\scriptscriptstyle 2}}\overset{\left(2\right)}{=} & \lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}= & \lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\left(\lambda_{{\scriptscriptstyle 2}}-\lambda_{{\scriptscriptstyle 1}}\right)\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}= & 0\wedge\lambda_{{\scriptscriptstyle 1}}\ne\lambda_{{\scriptscriptstyle 2}}\\
\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}= & 0
\end{aligned}
$$
:::

::: {.proof}
$\left(1\right)$ fast concept

::: {show-in="html"}

$$
\begin{aligned}
\color{orange}{\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}}=\left(\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A^{\intercal}\right)\boldsymbol{x}_{{\scriptscriptstyle 2}}\overset{\text{symmetric}}{=} & \left(\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A\right)\boldsymbol{x}_{{\scriptscriptstyle 2}}=\color{orange}{\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}\\
\left(L\right)=\color{orange}{\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=} & \color{orange}{\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}
=\left(R\right)\\
\left(L\right)=\color{orange}{\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}}
\overset{\left(e_{{\scriptscriptstyle 1}}\right)}{=} & \left(\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\left(R\right)=\color{orange}{\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}\overset{\left(e_{{\scriptscriptstyle 2}}\right)}{=} & \boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)=\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=\color{orange}{\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=} & \color{orange}{\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}=\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}= & \lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}
\end{aligned}
$$

:::

::: {show-in="pdf"}

$$
\begin{aligned}
{\color{orange}\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}}=\left(\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A^{\intercal}\right)\boldsymbol{x}_{{\scriptscriptstyle 2}}\overset{\text{symmetric}}{=} & \left(\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}A\right)\boldsymbol{x}_{{\scriptscriptstyle 2}}={\color{orange}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}\\
\left(L\right)={\color{orange}\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=} & {\color{orange}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}=\left(R\right)\\
\left(L\right)={\color{orange}\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}}\overset{\left(e_{{\scriptscriptstyle 1}}\right)}{=} & \left(\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\left(R\right)={\color{orange}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}\overset{\left(e_{{\scriptscriptstyle 2}}\right)}{=} & \boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)=\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}={\color{orange}\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}=} & {\color{orange}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)}=\lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}\\
\lambda_{{\scriptscriptstyle 1}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}= & \lambda_{{\scriptscriptstyle 2}}\boldsymbol{x}_{{\scriptscriptstyle 1}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 2}}
\end{aligned}
$$

:::
:::

::: {.theorem #unnamed-chunk-7}

::: {show-in="html"}

$$
\begin{array}{c}
\begin{cases}
\begin{cases}
A\in\mathcal{M}_{n\times n}\left(\mathbb{R}\right) & \text{real matrix}\\
A^{\intercal}=A & \text{symmetric matrix}
\end{cases} & \text{real symmetric matrix}\\
A\boldsymbol{x}_{{\scriptscriptstyle 1}}=\lambda\boldsymbol{x}_{{\scriptscriptstyle 1}} & \left(e\right)\\
\boldsymbol{x}_{{\scriptscriptstyle 2}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 1}}=0\Leftrightarrow\boldsymbol{x}_{{\scriptscriptstyle 2}}\perp\boldsymbol{x}_{{\scriptscriptstyle 1}} & \left(o\right)
\end{cases}\\
\Downarrow\\
A\boldsymbol{x}_{{\scriptscriptstyle 2}}\perp\boldsymbol{x}_{{\scriptscriptstyle 1}}\Leftrightarrow\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 1}}=0
\end{array}
$$

:::

::: {show-in="pdf"}

$$
\begin{array}{c}
\begin{cases}
\begin{cases}
A\in\mathcal{M}_{n\times n}\left(\mathbb{R}\right) & \textup{real matrix}\\
A^{\intercal}=A & \textup{symmetric matrix}
\end{cases} & \textup{real symmetric matrix}\\
A\boldsymbol{x}_{{\scriptscriptstyle 1}}=\lambda\boldsymbol{x}_{{\scriptscriptstyle 1}} & \left(e\right)\\
\boldsymbol{x}_{{\scriptscriptstyle 2}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 1}}=0\Leftrightarrow\boldsymbol{x}_{{\scriptscriptstyle 2}}\perp\boldsymbol{x}_{{\scriptscriptstyle 1}} & \left(o\right)
\end{cases}\\
\Downarrow\\
A\boldsymbol{x}_{{\scriptscriptstyle 2}}\perp\boldsymbol{x}_{{\scriptscriptstyle 1}}\Leftrightarrow\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 1}}=0
\end{array}
$$

:::

:::

::: {.proof}
$$
\begin{aligned}
\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 1}}= & \left(\boldsymbol{x}_{{\scriptscriptstyle 2}}^{\intercal}A^{\intercal}\right)\boldsymbol{x}_{{\scriptscriptstyle 1}}\overset{\text{symmetric}}{=}\left(\boldsymbol{x}_{{\scriptscriptstyle 2}}^{\intercal}A\right)\boldsymbol{x}_{{\scriptscriptstyle 1}}\\
= & \boldsymbol{x}_{{\scriptscriptstyle 2}}^{\intercal}\left(A\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)\overset{\left(e\right)}{=}\boldsymbol{x}_{{\scriptscriptstyle 2}}^{\intercal}\left(\lambda\boldsymbol{x}_{{\scriptscriptstyle 1}}\right)\\
= & \lambda\boldsymbol{x}_{{\scriptscriptstyle 2}}^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 1}}\overset{\left(o\right)}{=}\lambda\cdot0=0\\
\left(A\boldsymbol{x}_{{\scriptscriptstyle 2}}\right)^{\intercal}\boldsymbol{x}_{{\scriptscriptstyle 1}}= & 0\Leftrightarrow A\boldsymbol{x}_{{\scriptscriptstyle 2}}\perp\boldsymbol{x}_{{\scriptscriptstyle 1}}
\end{aligned}
$$
:::
