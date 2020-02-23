### 1.

#### (a)

$$
\nabla f(x)=\nabla(\frac{1}{2}x^TAx+b^Tx)=Ax+b
$$

#### (b)

$$
\frac{\partial g(h(x))}{\partial x_i}
=\frac{\partial g(h(x))}{\partial h(x)}\frac{\partial h(x)}{\partial x_i}
=g'(h(x))\frac{\partial h(x)}{\partial x_i}
$$

$$
\nabla f(x)=\nabla g(h(x))=g'(h(x))\nabla h(x)
$$

#### (c)

$$
\begin{align}
\nabla^2f(x)
& = \begin{bmatrix}
\frac{\partial\nabla f(x)}{\partial x_1} & \frac{\partial\nabla f(x)}{\partial x_2} & \ldots & \frac{\partial\nabla f(x)}{\partial x_n}\\
\end{bmatrix}\\
& = \begin{bmatrix}
\frac{\partial\nabla(Ax+b)}{\partial x_1} & \frac{\partial\nabla(Ax+b)}{\partial x_2} & \ldots & \frac{\partial\nabla(Ax+b)}{\partial x_n}\\
\end{bmatrix}\\
& = \begin{bmatrix}
A_{11} & A_{12} & \ldots & A_{1n}\\
A_{21} & A_{22} & \ldots & A_{2n}\\
\vdots & \vdots & \ddots & \vdots\\
A_{n1} & A_{n2} & \ldots & A_{nn}\\
\end{bmatrix}=A
\end{align}
$$

#### (d)

$$
\nabla f(x)
=\nabla g(a^Tx)
=g'(a^Tx)\nabla(a^Tx)
=g'(a^Tx)a
$$

$$
\frac{\partial^2 g(h(x))}{\partial x_i\partial x_j}
=\frac{\partial^2 g(h(x))}{\partial(h(x))^2}\frac{\partial h(x)}{\partial x_i}\frac{\partial h(x)}{\partial x_j}
=g''(h(x))\frac{\partial h(x)}{\partial x_i}\frac{\partial h(x)}{\partial x_j}
$$

$$
\frac{\partial^2 g(a^Tx)}{\partial x_i\partial x_j}
=g''(a^Tx)\frac{\partial(a^Tx)}{\partial x_i}\frac{\partial(a^Tx)}{\partial x_j}
=g''(a^Tx)a_ia_j
$$

$$
\nabla^2 f(x)
=\nabla^2 g(a^Tx)
=g''(a^Tx)\begin{bmatrix}
a_1a_1 & a_1a_2 & \ldots & a_1a_n\\
a_2a_1 & a_2a_2 & \ldots & a_2a_n\\
\vdots & \vdots & \ddots & \vdots\\
a_na_1 & a_na_2 & \ldots & a_na_n\\
\end{bmatrix}
=g''(a^Tx)aa^T
$$

---

### 2.

#### (a)

$$
A^T=(zz^T)^T=zz^T=A
$$

$$
x^TAx=x^Tzz^Tx=x^Tz(x^Tz)^T=(x^Tz)^2\ge0
$$

#### (b)

$$
Ax=zz^Tx=z(z^Tx)=0
$$

$$
N(A)=\{x\in\R^n:z^Tx=0\}
$$

$$
R(A)=R(zz^T)\le\min\{R(z),R(z^T)\}=1
$$

$$
R(A)=1
$$

#### (c)

$$
(BAB^T)^T=BA^TB^T=BAB^T
$$

$$
x^TBAB^Tx=(x^TB)A(x^TB)^T\ge0
$$

---

### 3.

#### (a)

$$
A=T\Lambda T^{-1}
$$

$$
AT=T\Lambda
$$

$$
A\begin{bmatrix}
t^{(1)} & t^{(2)} & \ldots & t^{(n)}\\
\end{bmatrix}
=\begin{bmatrix}
t^{(1)} & t^{(2)} & \ldots & t^{(n)}\\
\end{bmatrix}
\begin{bmatrix}
\lambda_1 & 0 & \ldots & 0\\
0 & \lambda_2 & \ldots & 0\\
\vdots & \vdots & \ddots & \vdots\\
0 & 0 & \ldots & \lambda_n\\
\end{bmatrix}
$$

$$
\begin{bmatrix}
At^{(1)} & At^{(2)} & \ldots & At^{(n)}\\
\end{bmatrix}
=\begin{bmatrix}
\lambda_1 t^{(1)} & \lambda_2 t^{(2)} & \ldots & \lambda_n t^{(n)}\\
\end{bmatrix}
$$

$$
At^{(i)}=\lambda_i t^{(i)}
$$

#### (b)

$$
A=U\Lambda U^T
$$

$$
AU=U\Lambda U^TU=U\Lambda
$$

$$
A\begin{bmatrix}
u^{(1)} & u^{(2)} & \ldots & u^{(n)}\\
\end{bmatrix}
=\begin{bmatrix}
u^{(1)} & u^{(2)} & \ldots & u^{(n)}\\
\end{bmatrix}
\begin{bmatrix}
\lambda_1 & 0 & \ldots & 0\\
0 & \lambda_2 & \ldots & 0\\
\vdots & \vdots & \ddots & \vdots\\
0 & 0 & \ldots & \lambda_n\\
\end{bmatrix}
$$

$$
\begin{bmatrix}
Au^{(1)} & Au^{(2)} & \ldots & Au^{(n)}\\
\end{bmatrix}
=\begin{bmatrix}
\lambda_1 u^{(1)} & \lambda_2 u^{(2)} & \ldots & \lambda_n u^{(n)}\\
\end{bmatrix}
$$

$$
Au^{(i)}=\lambda_i u^{(i)}
$$

#### (c)

$$
At^{(i)}=\lambda_i t^{(i)}
$$

$$
(t^{(i)})^TAt^{(i)}=\lambda_i\|t^{(i)}\|_2=\lambda_i\ge0
$$

