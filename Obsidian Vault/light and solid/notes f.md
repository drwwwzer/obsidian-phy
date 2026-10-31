
目的关键：

最主要的问题是对具体的处理方法讨论的内容不够熟悉，所以我的重点在于：
复现。


1.论文进展

由于对于相关话题的不够熟悉，暂时还无法说有一个想做的方向。于是我想先可以来拆拆看这篇博士论文的工作具体有哪些东西。
主要其实包括了PRA与PRB的工作。
OP的我还没看
首先是半导体布洛赫方程SBEs
一维带相位项的半导体布洛赫方程、二维速度规范下的半导体布洛赫方程
然后是
首先是气体强场的三步半经典模型。
固体强场的
SFA：对SBEs的近似
时频分析。
双色反旋圆极化激光场指的是基频场 + 其 q 次谐波场组成的两色场,两个分量同为圆偏振但旋向相反(一个左旋、一个右旋),频率比为 1:q,故记作 1:q CRB 场



2.计算方法练习
目标，首先复现两篇论文里氧化锌和二硫化钼能带和的偶极矩的DFT计算，

第二是对于SBEs实现的数值方法，这方面老师之前似乎讲过不用我们自己来写，所以我只是找了一些开源来读来看。
CUED：适合学习模型 SBEs 和 ODE 组织
[项目仓库](https://github.com/ccmt-regensburg/CUED)；[方法论文：Wilhelm et al., PRB 103, 125419 (2021)](https://doi.org/10.1103/PhysRevB.103.125419)。
源码入口：[main.py](https://github.com/ccmt-regensburg/CUED/blob/master/cued/main.py)；[参数解析](https://github.com/ccmt-regensburg/CUED/blob/master/cued/utility/params_parser.py)。
 4.2 sbewh： Wannier 数据到 SBEs 
[项目仓库](https://github.com/mathunje/sbewh)；[Thümmler et al., CPC 320, 109958 (2026)](https://doi.org/10.1016/j.cpc.2025.109958)；[作者预印本](https://arxiv.org/abs/2508.07869)。
在 Wannier–Houston／随动框架下传播 Wannier 化的 SBEs，读取 Wannier90 生成的 `.tb` 数据；采用自适应步长 RK4/5，并提供高次谐波谱及布居等分析脚本。C++20 实现，提供 CPU／GPU 和并行路径，MIT 许可。
它为 DFT → Wannier 有效模型 → SBEs 提供具体参考；当前没有验证 ARES 能直接生成其所需数据，不能写成 ARES→sbewh 已打通。
所以我的重点集中在DFT基本计算和理论的了解上：
以参考书《Density Functional Theory  A Practical Introduction》为基础，在Si、Cu以及体心立方结构的ScAl上做k空间采样和截断能的优化。
依习题完成与样例分析来说大概完成了参考书的三分之一，剩余部分还需要大半个月。

3.问题与展望
正如上面所言，知识基础与计算方法还需要更进一步的了解。
最基本的，建立在已经有研究的基础上的工作尝试应该是更容易的，所以在现在的基础上来聊想要做什么的话，大体上我会倾向于论文中展望的第一第二点。
(1)进一步在理论上研究单层过渡金属二卤化物与强激光场相互作用中自旋 轨道耦合效应、能谷极化效应、高阶边带谱的偏振特性等。  (2)尝试研究拓扑材料的高次谐波等强场过程。
老师提过先前在这方面还有更进一步的的improve，老师这方面有什么考虑和研究倾向吗

