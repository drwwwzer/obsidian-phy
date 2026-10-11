
对于固体而言，热容的贡献一般由两方面组成：
- 晶格热振动引起的晶格热容
- 电子热运动引起的电子热容

对于较高温度的情形，电子热容的影响较小，我们首先讨论晶格热容。
根据经典统计，每个简谐振动的平均能量是$k_{B}T$，我们考虑最简单的由N个原子构成的固体情形，它有3N个简谐振动模，总的平均能量为$\overline{E}=3Nk_{B}T$。热容就此为一个不变的常数：$3Nk_{B}$。
但对于很多材料，在低温情形下热容并不会随温度变化保持不变。这种特异情况的解释首先由爱因斯坦提出。
根据量子理论，谐振子的能量本征值是量子化的：
$$E_{j}=\left( n_{j}+\frac{1}{2} \right)\hbar \omega_{j}$$
简谐近似下各简正坐标代表的振动相互独立，它们的简正性证明由此得到：[[]]
故而这些振子我们首先考虑它们作为近独立的子系存在/考虑正则系综理论直接写出它们能量的统计平均值：
$$\overline{E_{j}}=\frac{1}{2}\hbar \omega_{j}+\frac{\sum_{n_{j}}n_{j}\hbar\omega_{j}e^{-n_{j}\hbar\omega_{j}/k_{B}T}}{\sum_{n_{j}}e^{-n_{j}\hbar \omega_{j}/k_{B}T}}$$
根据统计物理，取$\beta=\frac{1}{k_{B}T}$，我们可以改写上式为一个更容易表示的写法：
$$\overline{E_{j}}=\frac{1}{2}\hbar \omega_{j}+\frac{\partial}{\partial \beta}\ln \sum_{n_{j}}e^{-n_{}\hbar \omega_{j}/k_{B}T}$$
这里的求和式子容易求出：$\sum_{n_{j}}e^{-n_{}\hbar \omega_{j}/k_{B}T}=\frac{1}{1-e^{-\beta \hbar \omega_{j}}}$
代入则有：
$$\overline{E_{j}}(T)=\frac{1}{2}\hbar \omega_{j}+\frac{\hbar\omega_{j}e^{-\beta \hbar \omega_{j}}}{1-e^{-\beta \hbar \omega_{j}}}=\frac{1}{2}\hbar \omega_{j}+\frac{\hbar\omega_{j}}{e^{\beta\hbar \omega_{j} }-1}$$
前一项即为零点能，后一项代表平均热能。
于是我们容易得到热容表达式：
$$\frac{d\overline{E_{j}}T}{dT}=k_{B} \frac{\left( \frac{\hbar\omega_{j}}{k_{B}T} \right)^2e^{\hbar\omega_{j}/k_{B}T}}{(e^{\hbar \omega_{j}/k_{B}T}-1)^2}$$
主要的区别在于，这展示出了量子理论值与振动频率有关。

对于高温极限的情况，
$k_{B}T\gg \hbar \omega_{j},亦即 \frac{\hbar\omega}{k_{B}T}\ll1$
我们有$$\frac{d\overline{E_{j}}}{dT}=k_{B} \frac{\left( \frac{\hbar\omega}{k_{B}T} \right)^2\left( 1+\frac{\hbar\omega_{j}}{k_{B}T}+\dots \right)}{\left[ \frac{\hbar\omega_{j}}{k_{B}T}+\frac{1}{2}\left( \frac{\hbar\omega_{j}}{k_{B}T} \right)^2+\dots \right]^2}=k$$
这很自然，因为当振子的能量远远大于能量子$\hbar \omega$时，量子化效应就会小得可以忽略。——具体而言，高温/低温在该体系下完全由每个振子占有多少个能量子来决定，当一个振子占有的能量在几百上千能量子情况下，相邻能级$\Delta E=\hbar \omega$就小到可以看作连续。

而对于低温极限情况，即$\frac{\hbar\omega}{k_{B}T}\gg1$时，则有：
$$\frac{d\overline{E_{j}}}{dT}=k_{B}\left( \frac{\hbar\omega}{k_{B}T}  \right)^2e^{-\hbar \omega_{j}/k_{B}T}$$
此时对于所有振子很难分配到能量子，于是振动被冻结在基态，很难被热激发，因而对晶格热容的贡献趋向于零。

至此我们分析完了频率为$\omega_{j}$的振子对热容量的贡献，晶体中包含有3N个简谐振动，总能量应该为它们能量的和。
对于爱因斯坦模型假设晶格中各原子的振动可以被看作是相互独立的，且所有原子都具有同一频率$\omega_{0}$。这能反映出$C_{v}$在低温时下降的基本趋势，但在低温范围时其理论值下降太陡而不符合实验。

再进一步，对于实际晶体而言，相互独立的振动是不现实的。同时，不同的晶格振动采取格波的形式在晶格中传播，对应到每个振子频率都可能不相同。由此，德拜假设固体为各向同性的固体，并引入频率分布来讨论此问题。
弹性介质的振动模正以波的形式出现。在此情况下，对于一定的波数矢量$q$，将出现一个纵波与两个横波，但这并不重要。重要的是，由此不同波矢的横纵波形式构成了晶格的全部振动模。
正如先前已有的讨论，根据周期性边界条件，波矢$q$的并不是任意的，它们在q空间形成均匀分布的格点，在体积元$dk=dk_{x}dk_{y}dk_{z}$中，q值数目为：
$$\frac{V}{(2\pi)^3}dk$$
实际上，$\frac{V}{(2\pi)^3}$即为波矢值的“密度”。
![[Pasted image 20261005205111.png]]

可能疑问在于，对于离散的波矢$q$如何讨论它的分布？进一步，由于$V$是一个宏观的体积，允许的$q$值在$q$空间是十分密集的，由此它可以被看作是准连续的，对于这样准连续分布的变量，我们可以把相应数目写为：
$$\Delta n=g(n)\Delta \omega$$
$g(\omega)$就往往被称为频率的频率分布函数，或称为振动模的态密度函数，它具体地描述了一个晶体中振动模频率的分布情况。
又由于我们先前讨论晶格热容中，振动模的热容只取决于它的频率：
$$\omega=k_{B} \frac{\left( \frac{\hbar\omega}{k_{B}T} \right)^2e^{\hbar \omega/k_{B}T}}{(e^{\hbar \omega/k_{B}T}-1)^2}$$
于是我们能够写出晶体热容：


$$C_{V}(T)=k_{B} \frac{\int\left( \frac{\hbar\omega}{k_{B}T} \right)^2e^{\hbar\omega/k_{B}T}}{(e^{\hbar \omega/k_{B}T}-1)^2}g(\omega)d\omega$$


由此能求到德拜模型晶体的频率分布函数。
对于弹性波有纵波：
$$\omega=C_{l}q$$
对于弹性波有横波：
$$\omega=C_{t}q$$
我们首先考虑纵波的情况，对于从$\omega$到$\omega+d\omega$内的纵波，波数容易写出：
$$q=\frac{\omega}{C_{l}}\to q+dq=\frac{\omega+d\omega}{C_{l}}$$
我们讨论在$q$空间中占据着半径为$q$，厚度为$dq$的球壳，从球壳体积与$q$的分布密度$\frac{V}{(2\pi)^3}$得到纵波的数目为：
$$\frac{V}{(2\pi)^3}4\pi q^2dq=\frac{V}{2\pi^2C^3_{l}}\omega^2d\omega$$
类似地可写出横波的数目：
$$2*\frac{V}{2\pi^2C^3_{t}}\omega^2d\omega$$
于是我们就能得到总的频率分布：
$$g(\omega)=\frac{3V}{2\pi^2\overline{C^3}}\omega^2$$
然后热容处理可以平均。其中有：
$$\frac{1}{\overline{C}^3}=\frac{1}{3}\left( \frac{1}{C^3_{l}}+\frac{2}{C^3_{t}} \right)$$
根据弹性理论，$\omega$可取从0到$\infty$的任意值，它们对应于无限长到任意短的波，显然对于这样的振动模积分有无限数目（理想连续介质理所应当）。然而实际晶体是由原子组成的，如果晶体包括N个原子，自由度就有3N个。这尤其体现了德拜模型的局限性。
这种局限性容易得到其适用范围：当波长远远大于微观尺度时，德拜宏观处理的方法理应适用，然而当波长与微观可比时以上宏观模型将有谬误。

德拜的处理方法是假设$\omega$大于某一$\omega_{m}$的短波实际上是不存在的，而以下的情况均能应用弹性波的近似。
当然，这种假设的上限如何确定也成为了至关重要的一点——我们可以由实际晶格的自由度确定如下：
$$\int^{\omega_{m}}_{0}g(\omega)d\omega=\frac{3V}{2\pi^2\overline{C}^3}\int^{\omega_{m}}_{0}\omega^2d\omega=3N$$
由此我们可以得到这个上限：
$$\omega_{m}=\overline{C}\left[ 6\pi^2\left( \frac{N}{V} \right) \right]^{1/3}$$
由此我们可以得到热容表达式：
$$C_{V}(T)=\frac{3k_{B}V}{2\pi^2\overline{C}^3} \int^{{\omega_{m}}}_{0} \frac{\left( \frac{\hbar\omega}{k_{B}T} \right)^2e^{\hbar\omega/k_{B}T}}{(e^{\hbar \omega/k_{B}T}-1)^2}\omega^2d\omega$$
于是有：
$$C_{V}(T)=9R\left( \frac{1}{\omega_{m}} \right)^3\int^{\omega_{m}}_{0} \frac{\left( \frac{\hbar\omega}{k_{B}T} \right)^2e^{\hbar\omega/k_{B}T}}{(e^{\hbar \omega /k_{B}T}-1)^2}\omega^2d\omega =9R\left( \frac{kT}{\hbar \omega_{m}} \right)^3\int^{\hbar \omega_{m/k_{B}T}} \frac{\xi^4e^\xi}{(e^\xi-1)^2}d\xi$$
其中$R=Nk_{B}$，$\xi=\frac{\hbar\omega}{k_{B}T}$
由此，我们观察到德拜热容函数只包含一个参数$\omega_{m}$，另外我们可以
$$\Theta_{D}=\frac{\hbar\omega_{m}}{k_{B}}$$
于是有德拜热容的表达式：
$$9R\left( \frac{T}{\Theta_{D}} \right)^3\int^{ \Theta_{D}/T } \frac{\xi^4e^\xi}{(e^\xi-1)^2}d\xi$$
德拜热容的低温极限特别有意义，。正如前述在一定的温度下，
德拜热容在低温的极限是严格成立的。


最主要的点在于晶体与非晶体振动模式密度的不同频谱图。

![[Pasted image 20261011131823.png]]
晶体来讲，锐利结构是与范霍夫节点相关的。而非晶体而言，它会变得圆滑。
![[Pasted image 20261011131833.png]]
拉曼光谱