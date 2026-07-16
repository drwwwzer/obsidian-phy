
> [!abstract] 本篇综述
> 对于可逆性，如果我们参考应用型教材（Linear Algebra and its Applications，David C.Lay，...）的诸多等价定义，至少目前会认为过于繁琐而脱离理论核心。于是我们暂时采取《Linear Algebra Done Right》的理论姿态。


那么我们从这个问题开始——
什么是可逆？


> [!info] INVERTIBLE
> - 线性映射$$T\in\mathcal{L}(V,W)$$
> 被称为可逆的，
> 
> 如果存在线性映射$S\in\mathcal{L}(W,V)$使得ST等于V上的恒等映射且TS等于W上的恒等映射。



> [!info] 可逆性等价于单性与满性
> - 一个线性映射是可逆的当且仅当它既是单的又满的


> [!info] 算子
> - 向量空间到其自身的线性映射被称为算子
> - 记号$\mathcal{L}(V)$表示V上全体算子所组成的集合，即$$\mathcal{L}(V)=\mathcal{L}(V,V)$$


而建立在算子的定义之上，我们有一个重要的等价


> [!info] 在有限维的情形，单性等价于满性
> 设V为有限维的向量空间，并设$T\in\mathcal{L}(V)$,则以下陈述等价：
> - T是可逆的
> - T是单的
> - T是满的
