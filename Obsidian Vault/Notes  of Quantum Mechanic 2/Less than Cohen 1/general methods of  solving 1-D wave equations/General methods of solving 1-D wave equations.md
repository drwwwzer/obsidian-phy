
> [!abstract] 
> 本章中我们将介绍几种基本的一维不含时波函数情况解法。
> - 无穷深方势阱情况
> - 谐振子势情况
> - $\delta$势阱
> - 自由粒子情况 
> - 有限深方势阱
> 
> 我们首先讨论不含时情况的便利性：$$\Psi(x,t)=\psi(x)\varphi(t) \tag{1.1}$$
> 即如上对于不含时的情形，波函数总有这样的分离变量解。由此，我们能将计算简化。

在正式介绍开始之前，我们首先介绍一种较传统教材自然导出能量E的方法，首先我们写出对任意量子体系的一般薛定谔方程：$$i\hbar \frac{\partial\Psi}{\partial t}=-\frac{\hbar^2}{2m} \frac{\partial^2\Psi}{\partial x^2} +V\Psi$$
我们再利用式（1.1），容易得到$$i\hbar \frac{\partial \varphi}{\partial t}\psi=-\frac{\hbar^2}{2m} \frac{\partial^2\psi}{\partial x^2}\varphi +V\psi \varphi$$
我们将显含t与显含x分列两边，自然地，我们得到$$i\hbar \frac{\partial\varphi}{\partial t} \frac{1}{\varphi }=-\frac{\hbar^2}{2m} \frac{\partial^2\psi}{\partial x^2} \frac{1}{\psi}+V$$

> [!info] E
> 由于t与x相独立，唯一使得该式成立的条件就是$$L.H.S=R.H.S=Const=E$$

容易得到$$\frac{\partial\varphi}{\partial t}=-\frac{iE}{\hbar}\varphi$$
于是完整的薛定谔方程导出：$$E\varphi=-\frac{\hbar^2}{2m} \frac{\partial^2\varphi}{\partial x^2}+V(x)\varphi $$


我们尤其着重介绍谐振子势情况、$\delta$势情况与自由粒子情况。最前者涉及ladder operator(它的数学必然性与泛用性在何处？)与一般的偏微分方程解析解法，最后者则涉及波振幅的透射与反射。


> [!info] 谐振子势
> 即
> $$V(x)=\frac{1}{2}kx^2=\frac{\hat{p}^2}{2m}$$时
> 我们需要解微分方程$$E\varphi(x)=-\frac{\hbar^2}{2m} \frac{\partial^2\varphi(x)}{\partial x^2}+\frac{\hat{p}^2}{2m}\varphi(x) $$此方程的具体解法我们另起一章，在此主要介绍两种主要解法：
> - Ladder Operator method
> - Analysis method
> 主要的问题是，对于[[Ladder operators methods]]，在量子力学实践中不少出现类似的升降算符机制，相关数学结构？
> 对于[[Analysis method]] ，则作为相应特殊方程求解与性质运用的典例。



第二是$\delta$势情况

> [!info] $\delta$势
> 即$$V(x)=\delta(x)$$
> 时，我们需要解微分方程$$E\varphi(x)=-\frac{\hbar^2}{2m} \frac{\partial^2\varphi(x)}{\partial x^2}+\delta(x)\varphi(x) $$
>解法分为两步：首先考虑x!=0的部分，$\delta(x)=0。$
>于是这部分即变为解一个二阶齐次微分方程，参考本章末述。
>然后是本部分的重点：由于$\delta$势的特点，需要考虑x=0处的跃变。 











> [!info] 一般解的选择
> 对于涉及含$x\to\infty$问题时，通常选择通解：$$\psi(x)=Ae^{\lambda x}+B\psi^{-\lambda x} $$
> 对于局域问题，通常选择通解：$$\psi(x)=A\sin \lambda x+B\cos \lambda x$$

