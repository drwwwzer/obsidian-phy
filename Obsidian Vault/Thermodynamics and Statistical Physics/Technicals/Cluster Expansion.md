
首先我们讨论经典统计下理想气体的集团展开,
由N个分子组成的这样的气体哈密顿量与配分函数能够方便写出：
此处由Pathria记号,$Q为配分函数，Z为其概率系数$
$$Q_{N}=\frac{1}{N!h^{3N}}\int e^{-\beta E}d^{3N}pd^{3N}r=\frac{1}{N!h^{3N}}\int e^{-\beta \left( \sum_{i} p^2_{i}/2m +u_{ij}\right )}d^{3N}pd^{3N}r$$
动量部分显然是高斯积分，这是容易的，我们有：
$$Q=\frac{1}{N!\lambda^{3N}}\int e^{-\beta \sum_{i<j} u_{ij}}=\frac{1}{N!\lambda^{3N}}Z$$
其中$(\lambda=\frac{h}{2\pi mkT})^{1/2}$
由此我们把位形积分/构型积分（configuration integral）单独做了分离变量，单拆Z有：
$$Z=\int e^{-\beta \sum_{i<j}u_{ij}}d^{3N}r=\int \prod _{i<j}e^{-\beta u_{ij}}d^{3N}r$$
当无需使用以微扰法为例的方法处理粒子，亦即粒子间毫无相互作用，$u_{ij}=0$的时候有：
$$Z_{N}^{(0)}=V^N,Q^{(0)}_{N}=\frac{1}{N!\lambda^{3N}}V^N$$


为了处理非理想情况的粒子气体，接下来我们自然要讨论有相互作用的情况，这由$Mayer$给
出。自然，我们从双原子情况开始，不妨设：
$$f_{ij}=e^{-\beta u_{ij}}-1$$
这个函数在无相互作用的情况符合为0，而在有相互作用的情况下，近似于实际配分函数地，在高温时这相对于1相当小，我们因此希望它能在高温情形下很好地近似于目标配分函数。

![[Pasted image 20260915222524.png]]

第一直觉地，我们对构型积分做展开：
$$\begin{align}
Z_{N}&=\int \prod_{i<j}(1+f_{ij})d^{3N}r_{1}\dots d^{3N}r_{N} \\ \\
&=\int\left[ 1+\sum f_{ij}+\sum f_{ij}f_{jk}+\dots \right]d^{3N}r_{1}\dots d^{3N}r_{N} \\
\end{align}
$$
具体而言对于其中展开的计算有

这里也展示了设出$f_{ij}$的另一层面原因：能够使展开成立。
具体而言，集团展开的方便诠释针对构型积分的困难计算简化。
在此我们使用引用概括，不再详述：
[[]]
其一在于重要的是集团数量
我们需要具体诠释集团展开下配分函数/巨配分函数


> [!info] 位力展开
> 位力展开并不困难，无非是泰勒展开的取舍位数不同而已，在此我们重在讨论位力展开与集团展开之间的关系；
> 具体而言，我们关注物态方程对于位力展开的表达式：
> $$\frac{Pv}{kT}=\sum_{l=1}^\infty a_{l}(T)\left( \frac{\lambda^3}{v} \right)^{l-1}$$
> 同时关注它对于集团展开的表达式：
> $$\frac{P}{kT}=\lim_{ V \to \infty }\left( \frac{1}{V} \right)\ln Q=\frac{1}{\lambda^3}\sum_{l=1}^\infty \bar{b}_{l}z^l $$
> 且：
> 
> 我们正是利用本式达成除去z目的的位力展开的。
> 
> 
> 






