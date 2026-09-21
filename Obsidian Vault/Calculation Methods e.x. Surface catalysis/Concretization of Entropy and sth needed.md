

> [!info] 
> - 统计物理中熵（entropy）的定义与推导已对它所反映的系统微观性质有了极其好的体现：$$S=k_{B}\ln \Omega$$但$\Omega$这个$微观状态数$依旧不是讨论具体系统性质的好量，于是我们在此需要讨论熵在不同相的系统中的具体化。


以理想气体为例，体系量子态数目应当正比于体系体积$V$。对于$N$个全同粒子组成的系综，其中单个粒子可及的状态数$\omega$=$const *V$系综的总状态数有如下关系：
$$\Omega \propto \frac{V^N}{N!}$$
再考虑理想气体状态方程：
$$V=\frac{Nk_{B}T}{p}$$
代入$\Omega$则有:
$$\Omega \propto \left( \frac{1}{p} \right)^N$$
亦即有:
$$S=k_{B}\ln \Omega=k_{B}\ln(const*p^{-N})$$
即：
$$S=const'-Nk_{B}\ln p$$
同时注意，此处将const'作为常数化入全式即有：
$$S=-Nk_{B}T\ln\left( \frac{p}{p^\circ} \right)$$
其中$p^\circ可根据克拉珀龙方程表示$
于是对于气体，具体化的气体熵变有结果：
$$\Delta S_{12}=k_{B}\ln \frac{p_{2}}{p_{1}}$$
类似地，对于理想稀溶液也有这样的推导过程：
$$\Delta S_{12}=k_{B}\ln \frac{C_{2}}{C_{1}}$$
> [!info] 
> 建立在统计物理基础上，我们讨论化学势$\mu$

对于固定温度压强不变/固定温度体积不变这一相对容易做到的实验条件，又根据勒让德（共轭变量）变换我们能够得到的等价热力学势函数，分别有：
$$\mu_{i}=\left( \frac{\partial H}{\partial N_{i}} \right)_{T,p,N_{j\neq i}}$$
$$\mu_{i}=\left( \frac{\partial F}{\partial N_{i}} \right)_{T,V,N_{j\neq i}}$$
其中$H=U-TS+PV，F=U-TS$
对于理想气体（Boltzmann）我们取第二条：
又对于理想气体定域情况与满足经典极限的情况，$$F=-NkT\ln Z$$
$$F=-NkT\ln Z+NkT\ln N!$$
且对于经典情况$Z=\sum_{l} \omega_{l} e^{-\beta \epsilon_{l}}$
于是有$$\mu=kT\ln\left[ \frac{N}{V} \right(\frac{h^2}{2\pi mkT})^{3/2}]$$
同时对于理想气体，ln内容$\ll 1$，所以理想气体的化学势是负的。




