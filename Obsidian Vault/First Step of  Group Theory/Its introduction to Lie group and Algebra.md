
> [!abstract] 
> Contents


群是这么一种$代数结构$，它仅仅由一种运算与一种集合构成，与任意一种代数结构一样$（example:Linear \ Map）$它需要如下四个关键性质：
$$1.结合律：\forall a_{1}、a_{2}、a_{3}\in A,有(a_{1}a_{2})a_{3}=a_{1}(a_{2}a_{3})$$
$$2.乘法封闭性：\forall a_{1}、a_{2}\in A,a_{1}a_{2}\in A$$
$$3.单位元：\exists a_{0}\in A,s.t.\forall a\in A,a_{0}a=aa_{0}=a$$
$$4.乘法逆元：\forall a\in A,\exists a^{-1}\in A,s.t.aa^{-1}=a_{0}$$
在此，我们借用高翔（引）的旋转矩阵例，从SO（3）来引出其上的李代数$SO(30)$

 我们先讨论对于任意旋转矩阵$R$，它有：
 $$RR^T=I$$
 假设它表征某个位姿随时间变化而变化的相机，类似的我们有
 $$R(t)R^T(t)=I$$
 对它求导：
 $$\dot{R(t)}R^T(t)+R(t)\dot{R^T(t)}=0$$
 整理有：
 $$\dot{R(t)}R^T(t)=-(\dot{R(t)}R^T(t))^T$$
 于是我们得到了这么一个反对称矩阵$\dot{R(t)}R^T(t)$
 以叉乘$a\ X\ b=\Arrowvert e_{1},e_{2},e_{3}\Arrowvert$
$$$$
> [!info] beginning


