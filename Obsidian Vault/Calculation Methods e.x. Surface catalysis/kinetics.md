
> [!abstract] 
> 本章中，我们需要讨论异相催化/界面催化赖以建立的动力学。


首先，对于一个给定吸附质A分子与已吸附分子A的表面位点，A分子的脱附率由两式乘积决定：
$$r_{desorption}=k_{-}\theta_{*}$$
其中速率常数$k_{-}$表示的是对于一个给定位点的脱附过程在单位时间内发生的概率（脱附过程的频率），$\theta_{A}=K_{ads}p_{A}\theta_{*}$并有[[一简单的解释]]
同时，作为分析的起点，对于平衡态有：
$$r_{adsorption}=r_{desorption}$$
代入则能表示清楚$K_{ads}与k_{+},k_{-}$的关系：
$$K_{ads}=\frac{k_{+}}{k_{-}}$$
于是有：
$$K=e^{-\Delta G^\circ/k_{B}T}=\frac{\frac{k_{B}T}{h}e^{-(G_{+TS}^{\circ}-G_{I}^{\circ})/k_{B}T}} {\frac{k_{B}T}{h}e^{-(G_{-TS}^\circ-G_{F}^\circ)/k_{B}T}}=e^{-(G_{F}^\circ-G_{I}^\circ)/k_{B}T}$$
注意其中最后一个等号的成立条件，它意味着+-两态指示的反应经过同样的过渡态。在无其他条件的情况下，这由力学系统的时间反演对称性。
然后我们希望把是否可逆的标准确立清晰：
对于任意一个常见的吸附脱附过程对：$A+*与 A*$我们有：
$$\frac{\theta_{A}}{p_{A}\theta_{*}}=K_{ads}$$
我们不妨定义$平衡接近度$来封装具体信息：
$$\gamma_{ads}=\frac{\theta_{A}}{p_{A}\theta_{*}}K_{ads}^{-1}$$


由平衡接近度与1的关系，我们可以判断反应的方向和它与平衡状态的接近程度:
当$\gamma<1$时，该反应在为前向反应（正向反应？）。
当$\gamma=1$时，该反应为平衡状态。
当$\gamma>1$时，该反应为后向反应。


> [!info] 具体过程
> - 吸附/脱附过程(adsorption/desorption reaction)
> - 扩散过程（Diffussion reaction）
> - 耦合/断裂过程(coupling/scission reaction)

我们具体地落到某一$吸附/脱附过程$来讲：
$$2A^*\to A_{2}+2^*$$
我们将有一个速率表达式：
$$r_{ass}=k_{ass}\theta_{A}^2$$
其中覆盖比$\theta^2$实际上具有这样的物理意义：这表示了找到两个相接的空点位的概率。而$k_{ass}$则直接表示了调节其他影响因素的系数封装。

然后我们讨论常常发生在一个吸附位点与另一个相邻的吸附位点之间的$扩散反应$：
$$A^*+* \to * +A^*$$
它的速率常数表达式显然写为：
$$r_{dif}=k_{dif}\theta_{A}\theta_{*}$$
然后对于一个耦合/断裂反应：
$$A^*+B^*\leftrightarrow AB^* +*$$
它的速率常数表达式有：
$$r_{coupling}=k_{coupling}\theta_{A}\theta_{B}$$
$$r_{scission}=k_{scission}\theta_{AB}\theta_{*}$$

最后对于歧化反应：
$$AB^*+C^*\leftrightarrow 
A^*+BC^*$$
有：
$$r_{disorption}=k_{disorption}\theta_{AB}\theta_{C}$$




> [!info] 一个基元反应步的表观活化能
> 对于A与活化能$E_{A}$都与温度独立的情况，我们可以对$r=Ae^{-E_{A}/k_{B}T}$写出
> $$E^{apparent}_{A}=-\frac{\partial(\ln r)}{\partial\left( \frac{1}{k_{B}T} \right)}$$
> 然后由于随温度变化时对覆盖比的定量控制也十分困难，所以我们更近一步讨论：
> $$E^{apparent}_{A}=-\frac{\partial(\ln r)}{\partial\left( \frac{1}{k_{B}T} \right)}=-\frac{\partial(\ln k_{disorp}+\ln \theta_{AB}+\ln \theta _{C})}{\partial\left( \frac{1}{k_{B}T} \right)}$$
> 而如果我们近似地采取一般的速率常数分析,$k_{disprop}=A^{-E_{A}/k_{B}T}$：
> $$$E^{apparent}_{A}=-\frac{\partial(\ln k_{disorp}+\ln \theta_{AB}+\ln \theta _{C})}{\partial\left( \frac{1}{k_{B}T} \right)}=E_{A}-\frac{\partial(\ln \theta_{AB}+\ln \theta _{C})}{\partial\left( \frac{1}{k_{B}T} \right)}$$







 



