

承接热容的话题，为了充分表示清楚热容，我们需要计算出确切晶格振动的模式密度（频率分布函数）
首先我们给出频率分布函数的定义：
$$g(\omega)=\lim_{ \Delta \omega \to 0} \frac{\Delta n}{\Delta\omega} $$
于是我们可以表示出在q空间中单位频率振动模式的数量：
$$\Delta n=\frac{V}{(2\pi)^3}\int dsdq$$
且
$$\Delta \omega=dq|\nabla_{q}\omega(q)|$$
于是代入有模式密度的一般表达式：
$$g(\omega)=\frac{V}{(2\pi)^3}\int \frac{dS}{|\nabla_{q} \omega(q)|}$$

# 一维单原子链的例子

具体而言，我们首先计算一维单原子链的模式密度函数作为例子。
$q$空间的密度约化为$\frac{L}{2\pi}$，其中$L=Na$为单原子链的长度，a为原子兼具，N为原子数目。
由此我们能表示$dq$与$d\omega$间隔内的振动模式数目分别为与累计为：$\frac{L}{2\pi}dq$,
$$\Delta n=2*\frac{L}{2\pi} \frac{dq}{d\omega}d\omega$$
其中因子2源于$\omega(q)$具有中心反演对称性，因此我们将$q>0$与$q<0$等价地积到一起。就有模式密度分布函数的：
$$g(\omega)=\frac{L}{\omega} \frac{1}{\frac{d\omega}{dq}}$$
然后具体到一维单原子链求解，只记入最近邻原子之间的相互作用时可以直接代入原有的频率表达式：
$$\omega(q)=\sqrt{ \frac{4\beta}{m} }|\sin \frac{1}{2}aq|=\omega_{m}|\sin \frac{1}{2}aq|$$
其中$\omega_{m}$为最大频率。
由此我们有：
$$g(\omega)=\frac{2N}{\pi}(\omega^2_{m}-\omega^2)^{-1/2s}$$










