# computer graphics

## Cem Yuksel

### introduction

https://www.youtube.com/playlist?list=PLplnkTzzqsZTfYh4UbhLGpI5kGd5oW_Hh

#### 2D transformation

https://www.youtube.com/watch?v=EKN7dTJ4ep8&list=PLplnkTzzqsZTfYh4UbhLGpI5kGd5oW_Hh&index=6

##### translation

$$
\boldsymbol{p}^{\prime}=\boldsymbol{p}+\boldsymbol{t}\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}
\end{bmatrix}=\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}
\end{bmatrix}+\begin{bmatrix}t_{{\scriptscriptstyle x}}\\
t_{{\scriptscriptstyle y}}
\end{bmatrix}=\begin{bmatrix}p_{{\scriptscriptstyle x}}+t_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}+t_{{\scriptscriptstyle y}}
\end{bmatrix}
$$

##### scale

$$
\boldsymbol{p}^{\prime}=s\boldsymbol{p}\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}
\end{bmatrix}=s\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}
\end{bmatrix}=\begin{bmatrix}sp_{{\scriptscriptstyle x}}\\
sp_{{\scriptscriptstyle y}}
\end{bmatrix}
$$


##### non-uniform scale

$$
\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}
\end{bmatrix}=\begin{bmatrix}s_{{\scriptscriptstyle x}}p_{{\scriptscriptstyle x}}\\
s_{{\scriptscriptstyle y}}p_{{\scriptscriptstyle y}}
\end{bmatrix}=\begin{bmatrix}s_{{\scriptscriptstyle x}} & 0\\
0 & s_{{\scriptscriptstyle y}}
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}
\end{bmatrix}=S\boldsymbol{p}
$$

##### rotation

$$
\boldsymbol{p}=p_{{\scriptscriptstyle x}}\hat{\boldsymbol{x}}+p_{{\scriptscriptstyle y}}\hat{\boldsymbol{y}}=p_{{\scriptscriptstyle x}}\begin{bmatrix}1\\
0
\end{bmatrix}+p_{{\scriptscriptstyle y}}\begin{bmatrix}0\\
1
\end{bmatrix}=\begin{bmatrix}1 & 0\\
0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}
\end{bmatrix}=I\boldsymbol{p}
$$

$$
\boldsymbol{p}^{\prime}=p_{{\scriptscriptstyle x}}\begin{bmatrix}\cos\theta\\
\sin\theta
\end{bmatrix}+p_{{\scriptscriptstyle y}}\begin{bmatrix}-\sin\theta\\
\cos\theta
\end{bmatrix}=\begin{bmatrix}\cos\theta & -\sin\theta\\
\sin\theta & \cos\theta
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}
\end{bmatrix}=R_{{\scriptscriptstyle \theta}}\boldsymbol{p}
$$


$$
\boldsymbol{p}^{\prime}=p_{{\scriptscriptstyle x}}\begin{bmatrix}\cos\theta\\
-\sin\theta
\end{bmatrix}+p_{{\scriptscriptstyle y}}\begin{bmatrix}\sin\theta\\
\cos\theta
\end{bmatrix}=\begin{bmatrix}\cos\theta & \sin\theta\\
-\sin\theta & \cos\theta
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}
\end{bmatrix}=R_{{\scriptscriptstyle -\theta}}\boldsymbol{p}
$$

##### skew = rotation + non-uniform scale + rotation 

$$
back\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}
\end{bmatrix}=\begin{bmatrix}\cos\theta & \sin\theta\\
-\sin\theta & \cos\theta
\end{bmatrix}\begin{bmatrix}s_{{\scriptscriptstyle x}} & 0\\
0 & s_{{\scriptscriptstyle y}}
\end{bmatrix}\begin{bmatrix}\cos\theta & -\sin\theta\\
\sin\theta & \cos\theta
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}
\end{bmatrix}=R_{{\scriptscriptstyle -\theta}}SR_{{\scriptscriptstyle \theta}}\boldsymbol{p}
$$

##### any $2\times2$ matrix

$$
\boldsymbol{p}^{\prime}=M\boldsymbol{p}
$$

SVD = singular value decomposition

$$
M=U\varSigma V^{\intercal}\overset{\text{e.g.}}{=}RSR^{\intercal}=R_{{\scriptscriptstyle -\theta}}SR_{{\scriptscriptstyle \theta}}
$$

any $2\times2$ matrix + translation

$$
\boldsymbol{p}^{\prime}=M\boldsymbol{p}+\boldsymbol{t}
$$

$$
\boldsymbol{p}^{\prime}=M_{{\scriptscriptstyle 2}}\left(M_{{\scriptscriptstyle 1}}\boldsymbol{p}+\boldsymbol{t}_{{\scriptscriptstyle 1}}\right)+\boldsymbol{t}_{{\scriptscriptstyle 2}}
$$

##### homogeneous coordinate

$$
\boldsymbol{p}^{\prime}=\boldsymbol{p}+\boldsymbol{t}
$$

$$
\boldsymbol{p}^{\prime}=T\boldsymbol{p}=\boldsymbol{p}+\boldsymbol{t}
$$

$$
\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}
\end{bmatrix}=\begin{bmatrix}p_{{\scriptscriptstyle x}}+t_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}+t_{{\scriptscriptstyle y}}
\end{bmatrix}=\begin{bmatrix}1 & 0 & t_{{\scriptscriptstyle x}}\\
0 & 1 & t_{{\scriptscriptstyle y}}
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
1
\end{bmatrix}
$$

$$
\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
1
\end{bmatrix}=\begin{bmatrix}p_{{\scriptscriptstyle x}}+t_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}+t_{{\scriptscriptstyle y}}\\
1
\end{bmatrix}=\begin{bmatrix}1 & 0 & t_{{\scriptscriptstyle x}}\\
0 & 1 & t_{{\scriptscriptstyle y}}\\
0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
1
\end{bmatrix}=T\boldsymbol{p}
$$

$$
\boldsymbol{p}^{\prime}=M\boldsymbol{p}\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
1
\end{bmatrix}=\begin{bmatrix}a & c & e\\
b & d & f\\
0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
1
\end{bmatrix}=M\boldsymbol{p}
$$

##### position vs. direction

position vector: transformation affected by rotation and translation

$$
\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
1
\end{bmatrix}=\begin{bmatrix}a & c & e\\
b & d & f\\
0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
1
\end{bmatrix}=M\boldsymbol{p}
$$

direction vector: transformation affected by only rotation but not translation

$$
\boldsymbol{d}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
0
\end{bmatrix}=\begin{bmatrix}a & c & e\\
b & d & f\\
0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
0
\end{bmatrix}=M\boldsymbol{d}
$$

#### 3D transformation

https://www.youtube.com/watch?v=1z1S2kQKXDs&list=PLplnkTzzqsZTfYh4UbhLGpI5kGd5oW_Hh&index=7

##### homogeneous coordinate

affine transformation

$$
\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
1
\end{bmatrix}=\begin{bmatrix}a & c & e\\
b & d & f\\
0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
1
\end{bmatrix}=M\boldsymbol{p}
$$

$$
\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
p_{{\scriptscriptstyle z}}^{\prime}\\
1
\end{bmatrix}=\begin{bmatrix}a & d & g & j\\
b & e & h & k\\
c & f & i & l\\
0 & 0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
p_{{\scriptscriptstyle z}}\\
1
\end{bmatrix}=M\boldsymbol{p}
$$

##### scale

$$
\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
p_{{\scriptscriptstyle z}}^{\prime}\\
1
\end{bmatrix}=\begin{bmatrix}s_{{\scriptscriptstyle x}} & 0 & 0 & 0\\
0 & s_{{\scriptscriptstyle y}} & 0 & 0\\
0 & 0 & s_{{\scriptscriptstyle z}} & 0\\
0 & 0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
p_{{\scriptscriptstyle z}}\\
1
\end{bmatrix}=S\boldsymbol{p}
$$

##### translation

$$
\boldsymbol{p}^{\prime}=\begin{bmatrix}p_{{\scriptscriptstyle x}}^{\prime}\\
p_{{\scriptscriptstyle y}}^{\prime}\\
p_{{\scriptscriptstyle z}}^{\prime}\\
1
\end{bmatrix}=\begin{bmatrix}1 & 0 & 0 & t_{{\scriptscriptstyle x}}\\
0 & 1 & 0 & t_{{\scriptscriptstyle y}}\\
0 & 0 & 1 & t_{{\scriptscriptstyle z}}\\
0 & 0 & 0 & 1
\end{bmatrix}\begin{bmatrix}p_{{\scriptscriptstyle x}}\\
p_{{\scriptscriptstyle y}}\\
p_{{\scriptscriptstyle z}}\\
1
\end{bmatrix}=T\boldsymbol{p}
$$

### interactive

https://www.youtube.com/playlist?list=PLplnkTzzqsZS3R5DjmCQsqupu43oS9CFN
