# CH1 坐标系

## 坐标系
直角坐标，极坐标，求坐标  
矢量算符，标量算符，方向矢量的微分  
散度旋度  


# CH2 电磁场基本规律
### 静场  
静电场，静磁场的麦克斯韦方程

### 变化场  
电磁感应定律，变化电场产生变化磁场


### 麦克斯韦方程组


### 电磁场的矢势和标势
$B = \nabla \times A$  
$E = - \partial A / \partial t -\nabla \varphi$

### 波动方程  


# CH3 静场求解
对于静电场，当知道电荷分布时，根据点电荷电势分布叠加出电势分布，再根据 $E = - \nabla \varphi$ 求E会简单点  
求电势分布是求解拉普拉斯方程或泊松方程，定解需要边界条件。

静电场拉普拉斯（泊松）方程 + 边界条件  
静磁场拉普拉斯（泊松）方程 + 边界条件

稳恒电场  
稳恒电场与静电场很像，但是有一定区别。稳恒电场是由于电荷移动产生的，而静电场是由静止不动的电荷产生的。  
稳恒电场要考虑电导率。相比于静电场，其满足的方程和边界条件只需要用J替换D，用 $\sigma$ 替换 $\epsilon$

### 电路元件
#### 电容
同心内外圆柱壳电容<br> 
$C = \frac{2 \pi \epsilon}{ln{\frac{b}{a}}}$<br>
平行传输线电容  <br>
$C = \frac{\pi \epsilon}{ln{\frac{D}{a}}}$ <br>
多导体等效电容  <br>
部分填充电介质平板电容器电容 <br> 
平行板电容： $C = \frac{\epsilon S}{d}$
填充介质与未填充介质部分看做并联，电容相加
#### 电感
总内自感加外自感 <br>
同轴线缆电感： $L = \frac{\mu}{8 \pi} + \frac{\mu}{2 \pi} ln{\frac{b}{a}}$<br>
平行双线电感： $L = \frac{\mu}{4 \pi} + \frac{\mu}{\pi} ln{\frac{D}{a}}$<br>

#### 电阻

### 静电力
$F = \frac{\partial W}{\partial x}$ <br>
$W$ 为静电场能量

### 场能量
电场能量： $W_e = \frac{1}{2} \int \epsilon E^2 dV$ <br>
磁场能量： $W_m = \frac{1}{2} \int \mu H^2 dV$ <br>

# CH4 时谐电磁场
波动方程 <br>

时谐电磁场复数表示<br>
复数形式麦克斯韦方程和波动方程<br>
亥姆霍兹方程<br>
波阻抗<br>
$\eta = \sqrt{\frac{\mu}{\epsilon}}$<br>
复介电常数<br>
$\epsilon_c = \epsilon - j\frac{\sigma}{w}$<br>
复坡印亭定理，复坡印亭矢量<br>
$S_c = \frac{1}{2} E \times H^*$<br>
$S_{av} = Re[S_c]$<br>

# CH5 均匀平面波在无界空间的传播
## 5.1 在理想介质中传播


## 5.2 在导电媒介中传播，振幅会有衰减，电场磁场会产生相位差
波的表达式<br>
$E = e_x E_{xm}e^{-\alpha z} e^{-j\beta z}$<br>
$\alpha$ 是振幅衰减因子，$\beta$ 是相位因子<br>
$\alpha = w\sqrt{\frac{\mu \epsilon}{2} \sqrt{1 + (\frac{\sigma}{w \epsilon})^2} - 1}$<br>
$\beta = w\sqrt{\frac{\mu \epsilon}{2} \sqrt{1 + (\frac{\sigma}{w \epsilon})^2} + 1}$<br>

波阻抗表达式，产生的相位差表达式<br>
相速度，色散关系<br>
$\alpha$和$\beta$表达式<br>
能量密度<br>
$w_{eav} = \frac{\epsilon}{4} E_{xm}^2 e^{-2 \alpha z}$ <br>
$w_{mav} = \frac{\mu}{4} \frac{E_{xm}^2}{\left| \eta_c \right|} e^{-2 \alpha z}$ <br>
平均坡印亭矢量（记结果）<br>
$S_{av} = e_z \frac{\left| E \right|^2}{\left| \eta_c \right|} cos\phi$

### 5.2.1 特殊情况
#### 1. 良介质
$\gamma = jw \sqrt{\mu \epsilon(1- j\frac{\sigma}{w \epsilon})}$ <br>
近似方法要记住 $(1+x)^n = 1+nx$<br>
$\alpha = \frac{\sigma}{2} \sqrt{\frac{\mu}{\epsilon}}$ <br>
$\beta = w \mu \sqrt{\mu \epsilon}$ <br>
$\eta = \sqrt{\frac{\mu}{\epsilon}}(1-j\frac{\sigma}{w\epsilon})^{-\frac{1}{2}} = \sqrt{\frac{\mu}{\epsilon}}(1 + j\frac{\sigma}{2w\epsilon})$ <br>


#### 2. 良导体
$\alpha = \beta = \sqrt{\pi f \mu \sigma}$ <br>
$\eta = \sqrt{\frac{jw\mu}{\sigma}} = \sqrt{\frac{2\pi f \mu}{\sigma}}e^{j\frac{\pi}{4}}$<br>
趋肤效应，表面电流，表面电场，表面平均损耗功率 <br>



## 5.3 电磁波的极化
线极化波，圆极化波，椭圆极化波概念、产生条件 <br>
旋向判断方法：超前叉乘落后点乘波传播方向，结果小于0左旋，大于0右旋 <br>


# CH6 界面的反射和折射
## 6.1垂直入射
### 6.1.1 理想导体
反射波与入射波振幅相等，相位差 $\pi$ ，在计算时求反射波直接让 $E_{rm} = - E_{im}$ <br>
没有透射波

反射波和透射波合成驻波，电场和磁场的驻点不同。驻波表达式很好求，这里不赘述。<br>
求平均坡印亭矢量为0，即电磁波的能量没有传输出去。

注意反射波的传播方向会改变，透射波方向不变。透射波的波速（相位因子）会改变。<br>
### 6.1.2 理想介质
$R = \frac{\eta_2 - \eta_1}{\eta_2 + \eta_1}$ <br>

$T = \frac{2\eta_2}{\eta_2 + \eta_1}$<br>

入射波和反射波合成波既有驻波成分又有行波成分，称为行驻波。<br>
要掌握将合成波化成行波加驻波的形式，如<br>
$e^{-j \beta_1 z} + Re^{j \beta_1 z} = (1 - R)e^{-j \beta_1 z} + 2 R \cos \beta_1 z$<br>
当R>0时，凑出cos，当R<0时凑出sin<br> 
要掌握合成波振幅求法，如：
$\left| e^{-j \beta_1 z} + Re^{j \beta_1 z} \right| = \left| 1 + Re^{j2 \beta_1 z} \right|$<br>
提一个$e^{-j \beta_1 z}$出来，它的模为1，剩下的就欧拉公式展开，实虚部平方和开根<br>
注意极值点的位置会考。

驻波比：
$S = \frac{E_{1max}}{E_{1min}} = \frac{1+ \left| R\right|}{1- \left| R\right|}$

平均功率流密度：<br>
介质1中： $S_{1av} = e_z \frac{E_{im}^2}{2\eta_1}(1-R)^2$<br>
介质2中： $S_{2av} = e_z \frac{E_{im}^2}{2\eta_2}T^2$<br>

### 6.1.3 一般介质
反射系数和投射系数公式形式同理想介质一样，但是对应的波导都换成复数波导。说明反射投射波除了振幅大小变化，相位也发生了移动。
在计算时先计算 $\frac{\sigma}{w\epsilon}$ 判断是不是良导体或是良介质，结合CH5的公式简化计算。

## 6.2 斜入射

折射定律：
$\frac{\sin \theta_t}{\sin \theta_i} = \frac{k_1}{k2} = \frac{\sqrt{\mu_{r1} \epsilon_{r1}}}{\sqrt{\mu_{r2} \epsilon_{r2}}}$

### 垂直极化波

$R = \frac{\eta_2 \cos \theta_i -\eta_1 \cos \theta_t}{\eta_2 \cos \theta_i + \eta_1 \cos \theta_t} = \frac{\cos \theta_i - \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}{\cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ 

$T = \frac{2\eta_2 \cos \theta_i}{\eta_2 \cos \theta_i + \eta_1 \cos \theta_t} = \frac{2 \cos \theta_i}{\cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ 

$ (垂直入射的公式上每个前面乘一个cos)

在垂直入射的公式上$\eta_2$前面乘$\cos \theta_i$而 $\eta_1$乘一个$\cos \theta_t$


### 平行极化波：
$R = \frac{\frac{\epsilon_2}{\epsilon_1}\cos \theta_i - \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}{\frac{\epsilon_2}{\epsilon_1} \cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ <br> 
$T = \frac{2\sqrt{\frac{\epsilon_2}{\epsilon_1}} \cos \theta_i}{\frac{\epsilon_2}{\epsilon_1}\cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ 

带角度的公式更常用。


## 6.3 全反射和全透射
全反射指反射系数模为1，全投射指反射系数模为0。

### 全反射
临界角 $\theta_c = \arcsin{\frac{n_2}{n_1}} = \arcsin{\sqrt{\frac{\epsilon_2}{\epsilon_1}}}$ <br>
反射角的正余弦值一般用折射定律和三角函数关系式求，因为折射角不存在。
入射角大于临界角会仍然会发生全反射，合成波是沿分界面方向传播，但振幅在垂直分界面方向按指数快速衰减，波主要存在分界面附近，称为`表面波`。

### 全投射
布儒斯特角 $\theta_b = \arcsin \sqrt{\frac{\epsilon_2}{\epsilon_2 + \epsilon_1}}$ 只对平行极化波有效。
对于垂直极化波，必须要求 $\epsilon_2 = \epsilon_1$

这个特性可用于极化滤波

## 6.4 多层介质
等效波阻抗。1 2 3层介质， 2 3 层等效波阻抗为：
$\eta_{ef} = \eta_2 \frac{\eta_3 + j \eta_2 \tan \beta_2 d}{\eta_2 + j \eta_3 \tan \beta_2 d}$ <br>
d为第二层材料厚度 <br>

当左右两层材料相同时，若$d = \frac{\lambda_1}{2 \sqrt{\epsilon_{r2}}}$ 则电磁波入射材料没有反射波，依据这个原理可以制作屏蔽罩。

# 7 导行电磁波

## 7.1
任意界面均匀波导系统的纵横场关系式P313


## 7.2 矩形波导





# Tips

电介质，磁介质的极化磁化电荷怎么求  
如果知道P或者M就根据公式求，如果不知道就根据
$D=\epsilon E = \epsilon_0 E + P$  求出P再用公式


导体中不能存在静电场  
电位移矢量点乘法向量等于面电荷密度 p67例2.42

两个导体之间知道电势差，求解E可以先假设电荷q，用高斯定律，再把q换成电势差
同心导体圆柱电场分布