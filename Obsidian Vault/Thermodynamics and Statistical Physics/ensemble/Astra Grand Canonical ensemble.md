
> [!abstract] 
> - 吸附现象
> - 有巨正则系综导出规范近独立粒子的平均分布
> - 建立在巨正则系综对玻色/费米分布适配上的涨落

首先是讨论巨正则系综情况的吸附现象（相较于催化理论常有的不考虑能量涨落），我们设吸附表面有$N_{0}$个吸附中心，每个吸附中心课吸附一个气体分子，被吸附的气体分子为$-\epsilon_{0}$,求达到平衡时的吸附率$\theta$=$N/N_{0}$与气体温度和压强的关系。
此时将气体看作热源与粒子源，当有N个分子被吸附的时候，能量为$-N\epsilon_{0}$(同时注意$\alpha=-\beta \mu$)
于是系统的巨配分函数为：
$$\Xi=\sum_{_{i=0}}^\infty \sum_{s}e^{-\alpha N-\beta E_{s}}\Omega=\sum_{N=0}^{N_{0}}e^{\beta(\mu+\epsilon_{0})N} \frac{N_{0}!}{N!(N_{0}-N)!}=[1+e^{\beta(\mu+\epsilon_{0})}]^{N_{0}}$$
配分函数=$\sum_{微观状态}该状态出现的权重$
在此我们也能回答这样一个问题：
# 配分函数究竟意味着什么？

它意味着所有可能状态的统计权重之和，更进一步为：
$$\Xi=\sum_{N}粒子数为N的状态数*每个状态权重$$
而对于被吸附分子的平均数为：
$$\overline{N}=-\frac{\partial}{\partial \alpha}\ln\Xi=\frac{kT\partial}{\partial \mu}\ln\Xi$$
其中化学势由[[Concretization of Entropy and sth needed]]给出。它是理想气体，这个设定的合理性事实上在《Fundamental ConCepts in Heterogeneous Catalysis》讨论。
$$e^{\mu/kT}=\frac{p}{kT}\left( \frac{h^2}{2\pi mkT} \right)^{3/2}$$
结果则有：
$$\theta=\frac{\overline{N}}{N_{0}}=\frac{1}{1+\frac{kT}{p}\left( \frac{2\pi mkT}{h^2} \right)^{3/2}e^{-\epsilon_{0}/kT}}$$





