

> [!abstract] 本篇综述
>- 在本篇笔记中，我们从能量——这一较于力在理论上更具基础意义的概念开始奠基。
>- 我们将从势能出发得到理论构造上对于力更自然的定义，并从这里出发，尝试导出哈密顿力学的根本动力学方程：哈密顿正则方程。
>- 然后，作为结尾与勾连，我们将介绍一点外代数、外微分与它们的Stokes和Gaussian


 首先，我们先不加定义地接受能量与势能的概念，然后由此得到力的概念：


> [!info] 力
> 我们认为，力是相互作用能随系统空间变化的变化，具体而言，如果一个粒子在某外场中有相互作用能$\mathcal{V}(x)$，则其受力与相互作用能的关系被定义为：$$Fdx=-dV(x)$$
> 具体来讲，受力则为:$$F=- \partial\frac{V(x)}{\partial x}$$
> 或者更普适的形式：$$F=-\nabla V(x)$$


然后，通过定义哈密顿量，我们得到哈密顿正则方程：

> [!info] 哈密顿量与哈密顿正则方程
> 我们将粒子的总能量写为哈密顿量$\mathcal{H}$,且有:$$H=\hat{\frac{p^2}{2m}}+V(x)$$
> 我们首先借用牛顿的先例，写出在上述力定义下的牛顿运动定律：$$ \frac{\partial p}{\partial t}=F=-\frac{\partial V}{\partial x}$$
> 且其中p为粒子的动量，其定义为：$$\frac{dx}{dt}=\frac{p}{m}$$
> 然后，我们可以借哈密顿量的定义重写牛顿运动定律，由此得到
> 
> **哈密顿正则方程**：$$\frac{\partial p}{\partial t}=- \frac{\partial H}{\partial x}, \frac{dx}{dt}= \frac{\partial H}{\partial p}$$



另外，在此我们首次讨论一种重要的数学方法：


> [!info] **外代数与微分形式**
> 外微分与此基础上的微分形式建立在多变量微积分的基础上，它的灵感（或者最明显的应用）首先出现在多变量函数的坐标变换上，亦即：
> 
> 对于$$x=x(x',y')$$
> $$y=y(x',y')$$
我们有：$$A=\int \int f(x,y)dxdy=\int \int f(x,y)|\frac{\partial(x,y)}{\partial(x',y')}|dx'dy' $$
其中：$$\frac{\partial(x,y)}{\partial(x',y')}= \frac{\partial x}{\partial x'} \frac{\partial y}{\partial y'}- \frac{\partial x}{\partial y'} \frac{\partial y}{\partial x'}$$
此即坐标变换的 **Jacobi determinant**
我们可以采取一个简单的代数操作快速导出这一结果，即将多元微积分（此处为二元）的积分微元从 *dxdy* 重写成 *dx$\land$dy*,
我们实际规定了一种新的乘法，这种代数乘法称为外积，且满足性质：$$dx\land dy=-dy\land dx$$
由此我们计算 *dx $\land$dy* 与 *dx' $\land$dy'*间的变换关系即有：$$dx\land dy=|\frac{\partial(x,y)}{\partial(x',y')}|dx'\land dy'$$
在推导中自然得到。







