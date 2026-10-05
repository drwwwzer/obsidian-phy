
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
再进一步，


