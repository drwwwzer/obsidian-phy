
> [!abstract] solution to hamonic oscillator situation
> 1

首先我们写出谐振子势情况下的薛定谔方程：$$E\psi=-\frac{\hbar^2}{2m} \frac{d^2\psi}{dx^2}+\frac{1}{2}m\omega^2x^2\psi$$
通过观察，它是形如$$\frac{d^2\psi}{d\xi^2}=(\xi^2-K)\psi$$
的一般方程。通过参数选择，我们可以将本式简单地化为这个形式。其中，$$\xi=\sqrt{\frac{m\omega}{\hbar}  }x$$且$$K=\frac{2E}{\hbar \omega}$$
然后是一个简单的化简：对于$\xi$在非常大的情况下，K实际上被$\xi^2$项支配。于是原式化简为：$$\frac{d^2\psi}{d\xi^2}=\xi^2\psi$$
这个方程有这样的解：$$\psi(\xi)=Ae^{-\xi^2/2}+Be^{\xi^2/2}$$
且显然$\xi$在无穷远处会趋向无穷。
于是：$\psi(\xi)\to ()e^{-\xi^2/2}  at$
它能够得到渐进解：$$\psi(\xi)=h(\xi)e^{-\xi^2/2}$$
简单计算为$$\frac{d^2h}{d\xi^2}-2\xi  \frac{dh}{d\xi}+(K-1)h=0$$
如何给出这个方程的解？我们采取级数解：$$h(\xi)=a_{0}+a_{1}\xi+a_{2}\xi^2+\dots=\sum^{\infty}_{j=0}a_{j}\xi^j$$
于是有:
$$\frac{dh}{d\xi}=a_{1}+2a_{2}\xi+3a_{3}\xi^{2}+\dots=\sum^{\infty}_{j=0}(j+1)a_{j+1}\xi^{j}$$
$$\frac{d^2h}{d\xi^2}=2a_{2}+2*3a_{3}\xi+3*4a_{4}\xi^2+\dots=\sum^\infty_{j=0}(j+2)(j+3)a_{j+2}\xi^{j}$$
代入方程中即有关系：
$$\sum^\infty_{j=0}[(j+1)(j+2)a_{j+2}-2ja_{j}+(K-1)a_{j}]\xi^i=0$$
显然这是一个单位向量线性无关的方程，于是对于每个合法的j都有条件：$$(j+1)(j+2)a_{j+2}-2ja_{j}+(K-1)a_{j}=0$$
显然结果有：$$$$


