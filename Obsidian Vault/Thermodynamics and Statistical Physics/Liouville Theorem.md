
> [!abstract] 
> 刘维尔定理说明这样一件事：$$如果随着一个代表点沿哈密顿正则方程所确定的轨道在相空间中运动，其邻域的代表点密度是不随时间改变的常量。$$

我们做一些简易证明：
前提是对于一保守系统，有分别以N个广义坐标与广义动量构造一2N维的相空间：它们必有一条件：
$$H(q_{1},\dots q_{N},p_{1},\dots，p_{N})=E$$所有该保守系统运动状态的代表点都必然落在该条件所表征的曲面之上。
设想大量结构完全相同的系统，各自从其初态出发沿哈密顿正则方程所给定的相空间轨道运动，这些系统的运动状态的代表点将在相空间中形成一个分布。我们以
$$\rho(q_{1},\dots q_{N},p_{1},\dots，p_{N})$$
表示相空间中的点密度，
$$d\Omega=dq_{1\dots }dq_{N}dp_{1}\dots dp_{N}$$
表示相空间中的一个体积元。
接下来考虑点密度$\rho$随时间$t$的变化：当时间由t变成t+dt时，在$(q_{i},p_{i})$处的代表点将运动到$(q_{i}+\dot{q_{i}}dt，p_{i}+\dot{p_{i}}dt)$
于是我们有对于点密度$\rho$的表达式：
$$\rho(q_{1}+\dot{q_{1}}dt,\dots q_{N}\dot{q_{N}}dt,p_{1}+\dot{p_{1}}dt,\dots，p_{N}+\dot{p_{N}}dt)=\rho+ \frac{d\rho}{dt}dt$$
其中：
$$\frac{d\rho}{dt}=\frac{\partial\rho}{\partial t}+\sum_{i}\left( \frac{\partial\rho}{\partial q_{i}}\dot{q_{i}}+\frac{\partial\rho}{\partial p_{i}}\dot{p_{i}} \right)$$
现在要证明：
$$\frac{d\rho}{dt}=0$$

我们的基本思路是这样的：
对于任意维度（如$2f$）的相空间与其中的体积元$d\Omega$在时刻t，在$d\Omega$内的代表点数为$\rho d\Omega$，在经过时间dt之后，有些代表点走出了这个体积元，另有些代表点走进了这个体积元，使得在这个固定的体积元中的代表点数变为$\left( \rho+ \frac{\partial\rho}{\partial t} dt\right)d\Omega$，前后相减，则有经过dt时间后$d\Omega$内代表点的增加数为：
$$\frac{\partial\rho}{\partial t}dtd\Omega$$
然后我们需要考察代表点是如何通过所选界面从而能够形成代表点的数量变化：
代表点需要通过这2f对边界平面才能走入或离开体积元$d\Omega$，于是我们分别计算在t时刻进入体积元的代表点数，它们必须位于以dA为底，以$\dot{q}，\dot{p}$为轴线，以$\dot{q_{i}}dt$为高的柱体内，亦即其内代表点数为：
$$\rho\dot{q_{i}}dtdA$$
而对于在t+dt时刻离开体积元的代表点有：
$$(\rho \dot{q_{i}})_{q_{i}+dq_{i}}dtdA=\left( \rho \dot{q_{i}}+\frac{\partial}{\partial q_{i}}(\rho \dot{q_{i}})dq_{i} \right)dtdA$$
两者做差即有在dt时间流入体积元的净代表点数：
$$-\frac{\partial}{\partial q_{i}}(\rho \dot{q_{i}})dq_{i} dtdA=-\frac{\partial}{\partial q_{i}}(\rho \dot{q_{i}})dtd\Omega$$
类似地，对于在dt时间内净流入任意一对平面$p_{i}$和$p_{i}+dp_{i}$的净代表点数为：
$$-\frac{\partial}{\partial p_{i}}(\rho \dot{p_{i}})dtd\Omega$$
分别讨论对$q_{i}$与$p_{i}$的流入之后，我们可以表示净代表点数：
$$\frac{\partial\rho}{\partial t}dtd\Omega=-\sum_{i}[-\frac{\partial}{\partial p_{i}}(\rho \dot{p_{i}})+\frac{\partial}{\partial q_{i}}(\rho \dot{q_{i}})]dtd\Omega$$
