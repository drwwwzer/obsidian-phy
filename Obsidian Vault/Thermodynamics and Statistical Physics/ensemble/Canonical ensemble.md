
> [! abstract] 
> 思路其实与微正则系统类似。唯一不同在于正则系统具有系统与外界热源的能量交换，因而会产生能量的波动涨落。最主要的


首先是
$$E+E_{r}=E^{(0)}$$
对于状态处在能量为$E_{s}$的状态s时，热源可处在能量为$E^{(0)}-E_{s}$的状态，并可表示微观状态数：
$$\Omega_{r}(E^{(0)}-E_{s})$$
同时表示系统处在状态s时的概率$\rho_{r}$有正比于微观状态数：$\rho_{r}\sim\Omega_{r}(E^{(0)}-E_{s})$
为了具体化这样概率的表示，我们需要讨论微观状态数究竟如何表示？
其一是常见操作对于该形式的微观状态数展开保留到一阶小量（究竟为何）
其二是可自然写清楚：
$$\rho_{s}\propto \Omega_{r}(E^{(0)}-E_{s})\ \ \ （等概率假设）$$
而后自然我们需要具体化$\Omega_{r}$的表达式并将它处理成容易计算的形式（strling近似），自然地我们想$\ln \Omega$，又因为$E^{(0)}\gg E_{s}$我们将$\ln \Omega_{r}(E^{0}-E_{s})$展开保留前两项：
$$\ln \Omega_{r}(E^{(0)}-E_{s})=\ln \Omega$$




$\rho_{s}\propto e^{-\beta E_{r}}$


对于正则系综于是可以讨论$能量涨落$：
$$\overline{(E-\overline{E})^2}=\sum_{s}\rho_{s}(E_{s}-\overline{E})^2=\overline{E^2}-(\overline{E})^2$$
而对于正则分布情况又有：
$$\frac{\partial E}{\partial \beta}=\frac{\partial}{\partial \beta} \frac{\sum_{s}E_{s}e^{-\beta E_{s}}}{\sum_{s}e^{-\beta E_{s}}}=-\frac{\sum_{s}E_{s}^2e^{-\beta E_{s}}}{\sum_{s}e^{-\beta E_{s}}}+\frac{\left( \sum_{s}E_{s}e^{-\beta E_{s}} \right)^2}{(\sum_{s}e^{-\beta E_{s}})^2}=-[\overline{E^2}-(\overline{E})^2]$$
综合上面两式有：
$$\overline{(E-\overline{E})^2}=-\frac{\partial\overline{E}}{\partial \beta}=kT^2 \frac{\partial\overline{E}}{\partial T}=kT^2C_{V}$$
这将能量的自发涨落与内能随温度的变化率即热容联系在一起，由于LHS永正，故而定容热容永正，在热力学中有提及系统的平衡稳定条件正是$C_{V}$恒正。
另外由此可以给出能量的相对涨落：
$$\frac{\overline{(E-\overline{E})^2}}{(\overline{E})^2}=\frac{kT^2C_{V}}{(\overline{E})^2}$$



> [!info] axtra tips
> [[relation between  microcanonical and canonical ensemble]]
> 


