
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
而后自然我们需要具体化$\Omega_{r}$的表达式并将它处理成容易计算的形式（strling近似），自然地我们想$\ln \Omega$，又因为$E^{(0)}\gg E_{s}$，这里想利用“小系统能量 ($E_s$) 相对于热源总能量很小”这一事实，所以最自然的展开点就是热源能量几乎不被扰动时的值，即展开点当在$E^{(0)}-E_{s}\to E^{(0)}$，我们将$\ln \Omega_{r}(E^{0}-E_{s})$展开在此时的保留前两项：
$$\ln \Omega_{r}(E^{(0)}-E_{s})=\ln \Omega_{r}(E_{0})+\frac{\partial\ln\Omega_{r}}{\partial E_{r}}(E_{r}-E^{(0)})=\ln \Omega_{r}(E_{0})+\frac{\partial\ln\Omega_{r}}{\partial E_{r}}(-E_{s})=\ln \Omega_{r}(E_{0})-\beta E_{s}$$
由于本式第一项显然是一个常数，于是我们可以将$\rho_{s}$的正比表示得到：
$$\rho_{s}\propto e^{-\beta E_{s}}$$
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



> [!info] 巨正则系综
> 



类似地我们容易讨论巨正则系综，它除去正则系综的特性之外，还与另一粒子源相关，即它的微观状态建立在能量为$E_{s}$的状态s时，粒子源与热源分别处在$N^{(0)}-N_{s}$与$E^{(0)}-E_{s}$，从而微观状态数可表示为：
$$\Omega_{r}(N^{(0)}-N_{s},E^{(0)}-E_{s})$$

类似地我们可以按$N_{r}=N^{(0)},E_{r}=E^{(0)}$展开此时的微观状态数，并由此观察得到此时处在状态s时的概率:
$$\rho \propto e^{-\alpha N_{s}-\beta E_{s}}$$，其中$\alpha=\frac{\partial \ln \Omega_{r}}{\partial N_{r}}=-\frac{\mu}{k_{B}T}$
当然记得注意，我们也只需要这种正比关系，系数由归一化给出：
$$\rho_{N,s}=\frac{1}{\Xi}e^{-\alpha N-\beta E_{s}}$$
其中，
$$\Xi=\sum_{N=0}^\infty \sum_{s}e^{-\alpha N-\beta E_{s}}$$
这就给出了一个具有确定体积$V$，温度$T$，与化学势$\mu$的系统处在粒子数$N$，能量$E_{s}$时的微观状态时的状态s上的概率。





在此基础上，我们讨论由巨正则系综理论推出的热力学公式：

首先是平均粒子数：
$$\overline{N}=\frac{1}{\Xi}\sum_{N=0}^\infty \sum_{s}Ne^{-\alpha N-\beta E_{s}}=\frac{1}{\Xi}\left( -\frac{\partial}{\partial \alpha} \right)\sum_{N=0}^\infty \sum_{s}e^{-\alpha N-\beta E_{s}}=\frac{1}{\Xi}\left( -\frac{\partial}{\partial \alpha} \right)\Xi=-\frac{\partial}{\partial \alpha}\ln\Xi$$
类似地亦有内能，亦即能量E的统计平均值：
$$U=\overline{E}=\frac{1}{\Xi}\left( -\frac{\partial}{\partial \beta} \right)\sum_{N=0}^\infty \sum_{s}e^{-\alpha N-\beta E_{s}}=-\frac{\partial}{\partial \beta}\ln\Xi$$
同时还有建立在能量基础上有：
$$\overline{Y}=\frac{1}{\Xi}\sum_{N}\sum_{s} \frac{\partial E}{\partial y}e^{-\alpha N-\beta E_{s}}=\frac{1}{\Xi} \left( -\frac{1}{\beta} \frac{\partial}{\partial y} \right)\sum_{N}\sum_{s}e^{-\alpha N-\beta E_{s}}=\frac{1}{\Xi}\left( -\frac{1}{\beta} \frac{\partial}{\partial y} \right)\Xi=-\frac{1}{\beta} \frac{\partial}{\partial y}\ln\Xi$$
然后是同时考虑热力学第一定律/能量角度与$\ln 配分函数$的微分出发：
一方面有$\beta\left( dU-Ydy+\frac{\alpha}{\beta}d\overline{N} \right)=-\beta d\left( \frac{\partial\ln\Xi}{\partial \beta} \right)+\frac{\partial\ln\Xi}{\partial y}dy-\alpha d\left( \frac{\partial}{\partial \alpha}\ln\Xi \right)$
另外有$\ln\Xi(\alpha,\beta,y)$，写它的全微分：$d\ln\Xi=\frac{\partial\ln\Xi}{\partial \beta}d\beta+\frac{\partial\ln\Xi}{\partial \alpha}d\alpha+\frac{\partial\ln\Xi}{\partial y}dy$







> [!info] axtra tips
> [[relation between  microcanonical and canonical ensemble]]
> 


