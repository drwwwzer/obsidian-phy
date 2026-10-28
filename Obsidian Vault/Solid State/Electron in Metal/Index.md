
> [!Abstract] 
> - 电导、热导、温差电、电流磁效应等输运过程最明显地表现了金属特征的一大方面。然而基于经典统计的电子表述无法解决电子热容与自由程无穷的问题。
> - 于是建立在能带理论与费米统计之上，我们能够讨论相对现代的输运理论。
> - 注：电子是十分经典的费米子。

在此我们不再赘述费米统计，详见[[Statistical Physics]]
我们希望在此描述清楚费米统计、费米能与化学势之间的物理图像。

- 第一，费米统计函数给出能量为$E$的本征态被一个电子占据的概率：$$f(E)=\frac{1}{e^{E-E_{F}/k_{B}T}+1}$$
- 第二，费米能指存在电子态与不存在电子态的能级分界层。而根据第一条性质，当一个本征态能量为距费米能几个$k_{B}T$之外的能量值时，其被占据的概率将急剧下降，特别当温度$T \to 0$时，这样的降速区间将同时趋近于0。 亦即此时所有$E<E_{F}$的本征态都被占满，而比此高的能量本征态都是空的。也就是说：![[Pasted image 20261027202341.png]]
- $T=0K$的极限下，费米能$E_{F}$就是电子此时填充的最高能级$E_{F}^0$
- 第三，化学势的定义为：
- $$\mu=\frac{\partial G}{\partial N}$$
这意味着，化学势在0K时的定义就是电子填充时导致的吉布斯自由能变化，因而也就是此时电子所能填充的唯一且最高的能级——费米能级。
在这个意义上，它们是同一的。
此时费米能由$N=\int^{E_{F}^0}_{0}N(E)dE$确定。

更进一步我们来讨论有限温度T的情况：
首先表示有限温度下的电子数量：
$$dN=f(E(k))\frac{V}{(2\pi)^3}dk$$
然后确定费米能，具体而言，费米能$E_{F}$可以由系统中的电子总数$N$表示为：$\sum_{i}f(E_{i})=N$。
对于有限能量情形，决定式为：
$$N=\int^{\infty}_{0}f(E)N(E)dE$$
为了方便起见，同时也表示$E$一下量子态的总数，我们引入$Q(E)$表示,并对决定式做分部积分：
$$Q(E)=\int^{E}_{0}N(E)dE$$
$$N=[f(E)N(E)]|_{0}^{\infty}-\int^{\infty}_{0} Q(E)\left( \frac{\partial f}{\partial E} \right)dE$$
第一项显然为零，因为$E$和$f(E)$分别在$E \to0$与$E \to \infty$取得0。
因此原式变为：
$$N=\int^{\infty}_{0}Q(E)\left( -\frac{\partial f}{\partial E} \right)dE$$
这个形式可以通过对$（\frac{\partial f}{\partial E}）$的操作近似积分。
$$\frac{\partial f}{\partial E}=\frac{1}{k_{B}T} \frac{1}{(e^{E-E_{F/k_{B}T}}+1)((e^-{E-E_{F/k_{B}T}}+1))}$$
这个函数具有类似$\delta$函数的性质。于是我们可以将原式变为：
$$N=\int^{\infty}_{-\infty}Q(E)\left( -\frac{\partial f}{\partial E} \right)dE$$
另一方面，对$Q(E)$在$E_{F}$附近展开为无穷级数，于是有：
$$N=Q(E_{F})\int^{\infty }_{-\infty}\left( -\frac{\partial f}{\partial E} \right)dE+Q'(E)\int^{\infty}_{-\infty }(E-E_{F})\left( -\frac{\partial f}{\partial E} \right)dE+\frac{1}{2}Q''(E_{F})\int^{\infty}_{-\infty}(E-E_{F})^2$$




