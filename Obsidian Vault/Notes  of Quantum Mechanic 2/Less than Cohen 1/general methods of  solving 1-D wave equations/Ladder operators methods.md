
> [!info] Ladder operators
> 

我们首先将简谐势写成更一般的形式：$$V(x)=\frac{\hat{p}^2}{2m}+\frac{1}{2}m(\omega x)^2=\frac{1}{2m}(\hat{p}^2+(m\omega x)^2 )$$
梯形算子来源何处？我们首先介绍一个简单的性质：$$(a+bi)(a-bi)=a^2+b^2$$
于是我们写出算符$$\hat{a}_{\pm}=\frac{1}{\sqrt{ 2\hbar m\omega }}(\mp i\hat{p}+(m\omega \hat{x}))$$

然后我们讨论这样一个升降算符积$\hat{a}_{-}\hat{a}_{+}$：$$\hat{a}_{-}\hat{a}_{+}=\frac{1}{2\hbar m\omega}(m^2\omega^2\hat{x}^2+\hat{p}^2-im\omega( \hat{x}\hat{p}-\hat{p}\hat{x}))$$
我们知道$$[\hat{x},\hat{p}]=i\hbar$$
于是$$\hat{a}_{-}\hat{a}_{+}=\frac{1}{\hbar \omega}\hat{H}+\frac{1}{2}$$
相应的有$$\hat{a}_{+}\hat{a}_{-}=\frac{1}{\hbar\omega}\hat{H}  -\frac{1}{2}$$
它们的性质首先有：$$[\hat{a}_{-},\hat{a}_{+}]=1$$
有了这两对关系，我们来讨论升降算符分别的作用：
首先是降算符，首先我们有$\hat{H}\psi=E\psi$。对于$\hat{a}_{-}\psi$，我们需要讨论$\hat{H}(\hat{a}_{-}\psi)$的结果。
我们不妨对$(\hat{H}\hat{a}_{-})$右乘这个对易子， -((-+) - (+-))，于是有$$\hat{H}\hat{a}_{-}\psi=(E-\hbar \omega)\psi$$
同理有$$\hat{H}\hat{a}_{+}\psi=(E+\hbar \omega)\psi$$
这两个性质由此说明了算符名字的由来（升降算符/Ladder Operator）。

由此我们可以简单的讨论基态（ground state）的情况：什么是基态呢？基态就是降算符作用后为零的态，在这即为：$$\hat{a}_{-}\psi=0$$此时的$\psi$就被称为波函数的基态，记作$\psi_{0}$，我们将$\hat{a}_{-}$定义代入:$$\frac{1}{\sqrt{ 2\hbar m\omega }}( i\hat{p}+(m\omega \hat{x}))$$






