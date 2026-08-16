

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

