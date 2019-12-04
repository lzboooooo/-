# Green 公式
#### 甲型积分
![Qlplsf.png](https://s2.ax1x.com/2019/12/04/Qlplsf.png)

$P$ 是 $D\rarr R$ 函数，计算
$$
\int_{\partial D}Pdx
$$
看图，可以将 $\int_{\partial D}Pdx$ 分成四段的和
$$
\begin{gathered}
AB: \int_{AB}Pdx \qquad\\
BC: \int_{BC}Pdx = 0\\
CD: \int_{CD}Pdx \qquad\\
DA: \int_{DA}Pdx = 0\\
\int_{\partial D} = \int_{a}^{b}P(x,\varphi(x))-P(x,\psi(x))dx\\
=-\int_{a}^{b}\int _{\varphi(x)} ^{\psi(x)} \frac{P}{y}dxdy\quad\quad\quad\\
=\iint \limits_{D} -\frac{\partial P}{\partial y} dxdy\quad\quad\quad\quad\quad
\end{gathered}
$$

#### 乙型区域
同理在乙型区域我们可以得出
$$
\begin{gathered}
    \int_{\partial D}Qdy=\iint \limits_{D} \frac{\partial Q}{\partial x} dxdy
\end{gathered}
$$

## **Green 公式**
一个区域可以被分解成多个甲型区域与乙型区域的和，所以有：
$$
\int_{\partial \Omega} Pdx + Qdy = \iint\limits_{\Omega}\frac{\partial Q}{\partial x} - \frac{\partial P}{\partial y}dxdy
$$

#### Green 公式推导的面积公式
$$
\begin{gathered}
    \int_{\partial D}xdy=\iint\limits_{D}\frac{\partial x}{\partial x}dxdy = \iint\limits_{D}d\sigma = S_D\quad\qquad\\
    \int_{\partial D}ydx=\iint\limits_{D}-\frac{\partial y}{\partial y}dxdy = -\iint\limits_{D}d\sigma = -S_D\quad\\
    S_D = \frac{1}{2}\int_{\partial D}xdy-ydx\qquad\qquad\qquad\qquad\quad\quad
\end{gathered}
$$