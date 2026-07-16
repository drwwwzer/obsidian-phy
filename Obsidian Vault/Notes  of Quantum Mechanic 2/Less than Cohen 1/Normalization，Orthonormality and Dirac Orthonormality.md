> [!info] Normalization
> 根据波函数的统计诠释，对于任意（是否？）量子力学体系的波函数都具有性质：$$\langle\psi|\psi\rangle=1$$

在此之后，我们介绍一种“近似正交归一”的方法：
 它的出发点在哪？我们从一个具体的情况，从尝试寻找动量算符的特征函数与特征值开始：$$-i\hbar\frac{d}{dx}f_{p}(x)=pf_{p}(x)$$
 容易解得$f_{p}(x)=Ae^{ipx/\hbar}$，但由于这个函数并不满足平方可积性，即有结论，动量算符在$Hilbert$空间中无特征函数。但，如果我们限制在实的特征值上，我们能够对这样的函数发现一种近似的正交归一。
 我们考虑与已知动量p相差不多的新动量p',即有$$\lmoustache_{-\infty}^{+\infty}f^{*}_{p'}(x)f_{p}(x)dx=|A|^2\lmoustache_{-\infty}^{+\infty}e^{i(p-p')x/h}dx=|A|^22\pi \hbar \delta(p-p')$$
 如果我们需要让它正交归一，易得$$A=\frac{1}{\sqrt{ 2\pi \hbar }}$$且此时$$\langle f_{p'}|f_{p}\rangle=\delta(p-p')$$
 
> [!info] Dirac Orthonormality
>"which is reminiscent of true orthonormality (Equation 3.10)—the indices are now continuousvariables, and the Kronecker delta has become a Dirac delta, but otherwise it looks just the same. I’llcall Equation 3.33 Dirac orthonormality"
>for continuous variables?






