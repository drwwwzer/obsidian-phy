

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
其次我们来介绍一下德拜近似下的两种色散关系下能够推导的模式密度：$\omega=cq$
其一是代入则有：
$$g(\omega)=\frac{V}{(2\pi)^3} \frac{1}{c} 4\pi \left( \frac{\omega}{c} \right)^2=\frac{V}{2\pi^2c^3}\omega^2$$
其二是建立在另一种情况上我们分别讨论三维二维一维情况：
$$\omega=cq^2$$
对于三维情况的q空间，等频率面为球面，半径正为$$q=\sqrt{ \frac{\omega}{c} }$$
我们容易得到相应的球面上的|$\nabla_{q}\omega$|：
$$|\nabla_{q}\omega|=\frac{d\omega}{dq}=2cq$$
这是一个常数，因此我们有此时的模式密度：
$$g(\omega)=\frac{V}{(2\pi)^3}\int \frac{dS}{|\nabla_{q}\omega|}=\frac{V}{(2\pi)^3} \frac{1}{|\nabla_{q}\omega|}\int dS=\frac{V}{(2\pi)^3} \frac{1}{2cq}4\pi q^2=\frac{V}{(w\pi)^2} \frac{1}{c^{3/2}}\omega^{1/2}$$
由此对于二维情况有：
$$g(\omega)=\frac{S}{(2\pi)^2} \frac{1}{2cq} 2\pi q=\frac{S}{4\pi c}$$
对一维情况有：
$$g(\omega)=\frac{L}{2\pi} \frac{1}{2cq} *2=\frac{L}{2\pi \sqrt{ c }}\omega^{-1/2}$$

综上所述，在色散关系给定时，我们能够给出相应维度下模式密度函数的表达式推导，具体而言在三二一维情况下模式密度函数就分别与频率的$\frac{1}{2}，0，-\frac{1}{2}$次方成比例。
再进一步根据上述提及过的模式密度的一般表达式，我们可以看到在$\omega(q)$对$q$的梯度为零的地方，$q(\omega)$应显示出某种奇异性。这样的使得$\nabla q\omega(q)=0$的点被称为$范霍夫奇点$
这样的奇点联系到具体的实际晶体中大都与布里渊区的高对称点对应，而这样临界点的数目则是由晶体的拓扑性质决定的。













