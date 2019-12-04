# Minkowiki不等式
设$f$在$[a,b]\times[c,d]$上非负、连续，$p\geq 1$，那么
$$
(\int_a^b(\int_c^df(x,y)dy)^pdx)^{\frac{1}{p}} 
\leq 
\int_c^d(\int_a^bf^p(x,y)dy)^{\frac{1}{p}}dx
$$
当$p>1$时，等式成立的充分必要条件是
$$
f(x,y) = u(x)v(y)
$$
#### **证明**
当$p=1$时等式成立.现设$p>1$.记
$$
g(x)=\int_c^df(x,y)dy,
$$
易知g在$[a,b]$上连续，而且
$$
\begin{gathered}
    \int_a^b g^p(x)dx = \int_{a}^{b} g^{p-1}(x)g(x) dx = \int_{a}^{b} g^{p-1}(x)\int_c^df(x,y)dy dx\\
    =\int_a^b (\int_c^d f(x,y)g^{p-1}(x)dy ) dx
\end{gathered}
$$
先交换积分次序，再用$H\ddot{o}lder$不等式，得
$$
\begin{gathered}
    \int_a^b g^p(x)dx = \int_a^b \Big(\int_c^d f(x,y)g^{p-1}(x)dy \Big) dx \\
    \leq
    \int_c^d \Big(\int_a^b f^p(x,y) dx \Big)^{\frac{1}{p}} \Big(\int_c^d g^{(p-1)q}(x,y) \Big)^{\frac{1}{q}} dy\\
    = \int_c^d \Big(\int_a^b f^p(x,y) dx \Big)^{\frac{1}{p}} dy\Big(\int_c^d g^{p}(x,y) \Big)^{\frac{1}{q}}
\end{gathered}
$$
在这里$p$,$q$满足 $\frac{1}{q}+\frac{1}{p} = 1$ , 因而$(p-1)q = p$.不等式的两边同除以$\Big(\int_c^d g^{p}(x,y) \Big)^{\frac{1}{q}}$即得
$$
\Big(\int_a^b g^p(x)dx\Big)^{\frac{1}{p}} \leq \int_c^d \Big(\int_a^b f^p(x,y) dx \Big)^{\frac{1}{p}} dy
$$
这个不等式就是
$$
\Big(\int_a^b\Big(\int_c^df(x,y)dy\Big)^pdx\Big)^{\frac{1}{p}} 
\leq 
\int_c^d\Big(\int_a^bf^p(x,y)dy\Big)^{\frac{1}{p}}dx
$$