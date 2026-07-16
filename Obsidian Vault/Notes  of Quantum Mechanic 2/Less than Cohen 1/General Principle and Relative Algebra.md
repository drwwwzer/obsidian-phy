				  
> [!abstract] 
> 对于量子力学的基本诠释，我们不再效仿教科书体系分章叙述，转而采取总纲+例子的形式在此做提纲挈领的提示，同时我们在此详细讨论经典框架下量子力学所需的数学工具。

 大体上，我们采取知乎用户拉格朗日的忧郁的版本：
 
> [!info] 量子力学基本假设
> - 全同性假设。
> - 一个处在时间$\mathbf{t}$的物理系统的状态可以用$Hilbert$空间的态矢量$\mathbf{|\psi(t)\rangle}$表示。
> - 可观测量由作用在$Hilbert$空间上的厄密算符$\hat{A}$来刻画。
> - 厄密算符$\hat{A}$的本征态$|u_{i}\rangle$可以构成一组正交完备基{$|u_{i}\rangle$}，这组完备正交基可以展开对应$Hilbert$空间的任意一个态，亦即：$$|\psi \rangle=\sum_{i}|u_{i}\rangle\langle u_{i}|\psi\rangle=\sum \alpha_{i}|u_{i}\rangle$$而对于物理量的测量就是把态矢量用对应物理量量的算符本征矢作展开，展开系数的模方$|\alpha|^2$就是测出相应本征值$\alpha_{i}$的几率，即$$\hat{A}|u_{i}\rangle=\alpha_{i}|u_{i}\rangle$$
> - 态矢量含时演化由薛定谔方程决定.

对于这些原理，我们做一些经典的解释。（并期望留下接口）
首先为何厄密算符如此特殊？这在于它的特殊性质。
然后我们讨论测量，实际上*算符*的作用类似于用于测量的的概念仪器，经由算符作用，我们能测出被作用的波函数待测的相应值。同时，对某量子体系的第一次测量将会造成该量子体系（所有的量子体系么？）的*坍缩*，亦即在第一次测量之前，该次测量将具有相应算符本征矢导致

 一个重点在于$\delta$函数：
 
> [!info] $\delta$函数
>  $\delta$函数被定义如下：$$\delta(x)=0\ \ \ \ \ \ \ \ \ \ \ \ \ (x\neq_{}0)$$且
>  $$\delta(x)\to \infty\ \ \ \ \ \ \ \ \ \ \ \ \ (x=0) $$
>  同时它具有以下性质：$$\lmoustache_{-\infty}^{+\infty}\delta(x)dx=1$$
>  不难得到，这导致$$f(x)\delta(x-a)=f(a)\delta(x-a)$$
>  于是有$$\lmoustache_{-\infty}^{+\infty}f(x)\delta(x-a)dx=f(a)\lmoustache_{-\infty}^{+\infty}\delta(x-a)dx=f(a)$$

对于它，我们来讨论一些例子，首先在于所有含$\delta(x)$函数,我们不妨设有两个这样的等价函数$D_{1}$(x)与$D_{2}$(x)，$D_{1}(x)$与$D_{2}(x)$的等价条件是：$$\lmoustache_{-\infty}^{+\infty}f(x)D_{1}(x)dx=\lmoustache_{-\infty}^{+\infty}f(x)D_{2}(x)dx$$
我们试做这样一个检验：$$\delta(cx)=\frac{1}{|c|}\delta(x)$$
我们讨论第一个例子，我们有阶跃函数：$$\theta(x)=1\ \ \ \ \ \ \ (x>0)$$$$\theta(x)=0\ \ \ \ \ \ \ (x<0)$$而当x=0时，$\theta(x)=\frac{1}{2}$，试证明：$$\frac{d\theta(x)}{dx}=\delta(x)$$然后我们来讨论第二个例子，试证明：$$\delta(x)=\frac{1}{2\pi}\lmoustache_{-\infty}^{+\infty}e^{ikx}dk$$


其中一个重点在于厄密算符与幺正算符的性质与计算：

> [!info] 厄密算符与幺正算符
> 若一个算符满足性质：$$\hat{H}^{\dagger}=\hat{H}$$则称此算符为厄密算符。
> 若一个算符满足性质：$$\hat{H}=\hat{H}^{-1}$$则称此算符为幺正算符

