
对与某一经典体系，其动力学状态在相空间中有一连续分布，以$d\Omega=dq_{1}\dots dq_{f}dp_{1}\dots dp_{f}$为对应体积元，用$\rho(q,p,t)$表示时刻t时的分布函数，于是我们能够表示系统的微观状态处在$d\Omega$中的概率为：
$$\rho(q,p,t)d\Omega$$
它满足归一化条件：
$$\int \rho(q,p,t)d\Omega=1$$
微观量B在一切可能的微观状态上的平均值也就被表示为：
$$\overline{B}=\int B\rho(q,p,t)d\Omega$$
建立在这个基础上，我们能对这样看似普适的统计学表达式给出物理意义：

> [!info] 统计系综
> - 设想有大量结构完全相同的系统，在相同的宏观条件直线，我们把这些大量系统的集合统称为统计系综。而在时刻t从统计系综中任意选取系统，这个系统的状态处在$d\Omega$范围内的概率为$\rho(q,p,t)d\Omega$,就此$\overline{B}=\int B\rho(q,p,t)d\Omega$则被称为微观量B在统计系综上的平均值，称为系综平均值。
> - 而对于量子状况下，仅需把微观量视为非连续的，并逐一对表达式做改造即可。

然后我们来讨论为正则系综理论的热力学公式：
关键在于将一个孤立系统$A^{(0)}$切成两有微弱相互作用的系统$A_{1}、A_{2}$
对于孤立复合系统$A^{(0)}$的微观状态数：
$$\Omega^{(0)}(E_{1},E_{2})=\Omega_{1}(E_{1})\Omega_{2}(E_{2})$$
在$A_{1},A_{2}$进行热接触时，理想状态下二者可以交换能量，但不能交换粒子或改变体积。对于孤立系统当有：
$$E_{1}+E_{2}=E^{(0)}$$
借此我们可以表示出
$$\Omega^{(0)}(E_{1},E^{(0)}-E_{1})=\Omega_{1}(E_{1})\Omega_{2}(E^{(0)}-E_{1})$$
亦即对于孤立复合系统对于给定的复合系统能量，微观状态数取决于$E_{1}$，或者直接来讲，它取决于复合系统总能量在$A_{1}、A_{2}$之间的分配。另外根据[[Ergodic hypothesis and so on]]，最概然情况/平均情况重合，我们可以认为$\overline{E_{1}}$,$\overline{E_{2}}$就是在热平衡情况下两分系统具有的内能。
由最概然情况与平均情况的重合，我们得以方便地确定条件：
$$\frac{\partial\Omega ^{(0)}}{\partial E_{1}}=0$$
代入则有：
$$\left[ \frac{\partial\ln\Omega_{1}(E_{1})}{\partial E_{1}} \right]_{N_{1},V_{1}}=\left[ \frac{\partial\ln\Omega_{2}(E_{2})}{\partial E_{2}} \right]_{N_{2},V_{2}}$$
对于这样的平衡量我们以$\beta$表示，则热平衡条件亦可表示为：
$$\beta_{1}=\beta_{2}$$
类似地，我们在热力学中有类似的结果，两个系统达到热平衡的条件为：
$$\left( \frac{\partial S_{1}}{\partial U_{1}} \right)=\left( \frac{\partial S_{2}}{\partial U_{2}} \right)$$
而$\left( \frac{\partial S_{}}{\partial U_{}} \right)=\frac{1}{T}$，显然$\beta与 \frac{1}{T}$成正比，所以有：
$\beta=\frac{1}{kT}$
进而有玻尔兹曼关系：
$$S=k\ln \Omega$$


> [!warning] 
> 此处$成正比$仅只是基于物理直觉的推断否？请验证之


类似地，对于更普适的体系，$A_{1},A_{2}$间不仅可以交换能量，而且可以改变体积和交换粒子，我们有：

$$\left[ \frac{\partial\ln\Omega_{1}(E_{1})}{\partial E_{1}} \right]_{N_{1},V_{1}}=\left[ \frac{\partial\ln\Omega_{2}(E_{2})}{\partial E_{2}} \right]_{N_{2},V_{2}}$$
$$\left[ \frac{\partial\ln\Omega_{1}(V_{1})}{\partial V_{1}} \right]_{N_{1},E_{1}}=\left[ \frac{\partial\ln\Omega_{2}(V_{2})}{\partial V_{2}} \right]_{N_{2},E_{2}}$$
$$\left[ \frac{\partial\ln\Omega_{1}(N_{1})}{\partial N_{1}} \right]_{E_{1},V_{1}}=\left[ \frac{\partial\ln\Omega_{2}(N_{2})}{\partial N_{2}} \right]_{E_{2},V_{2}}$$
简单地定义：
$$\gamma=\left[ \frac{\partial\ln\Omega_{}(N,E,V)}{\partial V_{}} \right]_{N_{},E_{}}$$
$$\alpha=\left[ \frac{\partial\ln\Omega_{}(N_{},E,V)}{\partial N_{}} \right]_{E_{},V_{}}$$
于是对于这样的系统，仅需比较在$N,E,V$均作为自变量的情况下，$\ln \Omega$的全微分与开系的热力学基本方程：$dS=\frac{dU}{T}+\frac{p}{T}dV-\frac{\mu}{T}dV$



> [!info] solution to atomic situation
>首先列出哈密顿量：
>$$H=\sum^{3N}_{i=1} \frac{p^2_{i}}{2m}$$ 
>另外对于维度为3N的体系，它的微观状态数为：
>$$\Omega(E)=\frac{1}{N!h^{3N}}\int_{E\leq H(q,p)\leq E+\Delta E}dq_{1}\dots dq_{3N}dp_{1}dp_{3N}$$
>为了计算在所有能量范围下的微观状态数总量，我们先计算有限能量幅度之内的微观状态数：
>$$\Sigma(E)=\frac{1}{N!h^{3N}}\int_{H(p,q)\leq E}dq_{1}\dots dq_{3N}dp_{1}dp_{3N}=\frac{V^{N}}{N!h^{3N}}\int_{H(q,p)\leq E}dp_{1}\dots dp_{3N}$$
>做[[变量代换]]容易有：
>$$\Sigma(E)=\frac{V^{N}}{N!h^{3N}}\int(2mE)^{3N/2}K$$
>另外注意K为[[3N维空间中半径为1的球体积]]
>因此有$$\Sigma(E)=\left( \frac{V}{h^3} \right)^N \frac{\pi^{3N/2}}{N!\left( \frac{3N}{2} \right)!}$$



再进一步，我们来讨论建立在此基础上系统的能量涨落。
首先，



同时更进一步，对于非平衡态系统，只需要参照上述逻辑，把它分成若干个相互有微弱相互作用友处在局域平衡的部分，玻尔兹曼关系就同样自然的得以导出。因此它也当适用于非平衡态。



根据前述的所有讨论，我们观察到力学规律与统计规律的密切关系，但它们究竟能追溯到怎样根本的地方？
> [!info] 力学规律与统计规律 
> - [[Ergodic hypothesis and so on]]
> - 邓煜

