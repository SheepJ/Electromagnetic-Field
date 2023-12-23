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

洛伦兹规范：<br>
$\nabla A + \mu \epsilon \frac{\partial \phi}{\partial t} =  0$ <br>




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
$\alpha$ 和 $\beta$ 表达式<br>
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
提一个 $e^{-j \beta_1 z}$ 出来，它的模为1，剩下的就欧拉公式展开，实虚部平方和开根<br>
注意极值点的位置会考。

驻波比：
$S = \frac{E_{1max}}{E_{1min}} = \frac{1+ \left| R\right|}{1- \left| R\right|}$

平均功率流密度：<br>
介质1中： $S_{1av} = e_z \frac{E_{im}^2}{2\eta_1}(1-R)^2$<br>
介质2中： $S_{2av} = e_z \frac{E_{im}^2}{2\eta_2}T^2$<br>

### 6.1.3 一般介质
反射系数和投射系数公式形式同理想介质一样，但是对应的波导都换成复数波导。说明反射投射波除了振幅大小变化，相位也发生了移动。
在计算时先计算 $\frac{\sigma}{w\epsilon}$ 判断是不是良导体或是良介质，结合CH5的公式简化计算。

损耗角 $\delta$ 有 $tan \delta = \frac{\sigma}{w \epsilon}$ <br>

## 6.2 斜入射

折射定律：
$\frac{\sin \theta_t}{\sin \theta_i} = \frac{k_1}{k2} = \frac{\sqrt{\mu_{r1} \epsilon_{r1}}}{\sqrt{\mu_{r2} \epsilon_{r2}}}$

### 垂直极化波

$R = \frac{\eta_2 \cos \theta_i -\eta_1 \cos \theta_t}{\eta_2 \cos \theta_i + \eta_1 \cos \theta_t} = \frac{\cos \theta_i - \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}{\cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ 

$T = \frac{2\eta_2 \cos \theta_i}{\eta_2 \cos \theta_i + \eta_1 \cos \theta_t} = \frac{2 \cos \theta_i}{\cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ 

(垂直入射的公式上每个前面乘一个cos)

在垂直入射的公式上 $\eta_2$ 前面乘 $\cos \theta_i$ 而 $\eta_1$ 乘一个 $\cos \theta_t$ <br>


### 平行极化波：
$R = \frac{\frac{\epsilon_2}{\epsilon_1}\cos \theta_i - \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}{\frac{\epsilon_2}{\epsilon_1} \cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ <br> 
$T = \frac{2\sqrt{\frac{\epsilon_2}{\epsilon_1}} \cos \theta_i}{\frac{\epsilon_2}{\epsilon_1}\cos \theta_i + \sqrt{\frac{\epsilon_2}{\epsilon_1} - \sin^2 \theta_i}}$ 

带角度的公式更常用。


## 6.3 全反射和全透射
全反射指反射系数模为1，全投射指反射系数模为0。

### 全反射
临界角 $\theta_c = \arcsin{\frac{n_2}{n_1}} = \arcsin{\sqrt{\frac{\epsilon_2}{\epsilon_1}}}$ <br>
反射角的正余弦值一般用折射定律和三角函数关系式求，因为折射角不存在。
入射角大于临界角会仍然会发生全反射，合成波是沿分界面方向传播，但振幅在垂直分界面方向按指数快速衰减，波主要存在分界面附近，称为`表面波`。 <br>
趋肤深度 $\delta = \frac{1}{\alpha}$ <br>
反射波和投射波系数仍然可以按照公式进行计算，结果将会附加一个相移项。入射波和反射波的合成看图分量相加。<br>
折射波的计算：假设 $\theta_t$ 存在，波矢量 $\left| k \right|$ 按照当前所处的介质来求， $e_k$ 则根据假定的角 $\theta_t$ 进行分量合成 $e_k = e_x sin \theta_t + e_z cos \theta_t$ 得到的结果应该是一个复数，直接代入透射波表达式进行化简，得到表面波<br>


### 全透射
布儒斯特角 $\theta_b = \arcsin \sqrt{\frac{\epsilon_2}{\epsilon_2 + \epsilon_1}} = arctan{\sqrt{\frac{\epsilon_2}{\epsilon_1}}}$ 只对平行极化波有效。
对于垂直极化波，必须要求 $\epsilon_2 = \epsilon_1$

这个特性可用于极化滤波

## 6.4 多层介质
等效波阻抗。1 2 3层介质， 2 3 层等效波阻抗为：
$\eta_{ef} = \eta_2 \frac{\eta_3 + j \eta_2 \tan \beta_2 d}{\eta_2 + j \eta_3 \tan \beta_2 d}$ <br>
d为第二层材料厚度 <br>

当左右两层材料相同时，若 $d = \frac{\lambda_1}{2 \sqrt{\epsilon_{r2}}}$ 则电磁波入射材料没有反射波，依据这个原理可以制作屏蔽罩。

# 7 导行电磁波

## 7.1
任意界面均匀波导系统的纵横场关系式P313 <br>
$H_x = - \frac{1}{k_c^2}(\gamma \frac{\partial H_z}{\partial x} - jw \epsilon \frac{\partial E_z}{\partial y})$ <br>

$H_y = - \frac{1}{k_c^2}(\gamma \frac{\partial H_z}{\partial y} + jw \epsilon \frac{\partial E_z}{\partial x})$ <br>

$E_x = - \frac{1}{k_c^2}(\gamma \frac{\partial E_z}{\partial x} + jw \epsilon \frac{\partial H_z}{\partial y})$ <br>

$E_y = - \frac{1}{k_c^2}(\gamma \frac{\partial E_z}{\partial y} - jw \epsilon \frac{\partial H_z}{\partial x})$ <br>

$k_c^2 = \gamma^2 + k^2$ <br>

减加加减，HHEE， 先 $\gamma$ 再 $jw \epsilon$ ，对x先x后y，对y先y后x

### TEM 波
$E_z$ 和 $H_z$ 分量都为0； 有 $k_c^2 = \gamma^2 + k^2 = 0$ <br>
所得到的 传播常数，相速度，等与无界空间均匀平面波的传播特性相同。

TEM 波在波导中不具备传播特性。


### TE 波 和 TM波
TE波 $E_z = 0$ ，TM波 $H_z = 0$ ， 从纵横场关系求得： <br>
$Z_{TM} = \frac{\gamma}{jw \epsilon}$ <br>
$Z_{TE} = \frac{jw \mu}{\gamma}$ <br>
电场磁场关系和前两章没有区别。<br>

$\gamma = \sqrt{k_c^2 - k^2}$ <br>
1. 当 $k < k_c$ 时， $\gamma$ 为实数，求得 $e^{- \gamma z}$ 是一个衰减因子，波无法传播出去，处于截止状态。

2. 当 $k > k_c$ 时， $\gamma = j \beta$ 为虚数， $\beta = \sqrt{k^2 - k_c^2}$ ，求得 $e^{- j \beta z}$ 是一个行波因子，波可以传播出去。

称 $k = k_c$ 为截止频率，相应的还有： <br>
截止角频率： $w_c = \frac{k_c}{\sqrt{\mu \epsilon}}$ <br>
截止波长： $\lambda_c = \frac{w \pi}{k_c}$ <br>
截止频率： $f_c = \frac{w}{2 \pi}$ <br>


## 7.2 矩形波导
### TM波
求解波动方程，用分离变量法，TM波边界条件为波导面上电场为0 <br>
$k_c^2 = k_x^2 + k_y^2$ <br>
$k_x = \frac{m \pi}{a}$ <br>
$k_y = \frac{n \pi}{b}$ <br>
m、n 是大于0的整数 <br>
$E(x,y) = E_m sin(\frac{m \pi}{a} x) sin(\frac{n \pi}{b} y)$ <br>
代入纵横场关系即可求出其他分量<br>

### TE波
边界条件变为磁场在波导面上法向偏导为0 <br>
求得 $H_z = H_m cos(\frac{m \pi}{a} x) cos(\frac{n \pi}{b} y)$ <br>

$m、n$ 的取值组合代表一个模式，TM波的m、n不能为0，TE波的m、n可以但不能同时为0 <br>
模式简并：相同一组m、n组合，TM波和TE波的截止波数k相等

### 传播参数
截止波数： $k_{cmn} = \sqrt{(\frac{m \pi}{a})^2 + (\frac{n \pi}{b})^2}$ <br>
截止频率： $f_{cmn} = \frac{k_{cmn}}{2 \pi \sqrt{\mu \epsilon}}$ <br>
截止波长： $\lambda_{cmn} = \frac{2 \pi}{k_{cmn}}$ <br>
传播常数： $\gamma_{mn} = \sqrt{k_{cmn}^2 - k^2}= \sqrt{(\frac{m \pi}{a})^2 + (\frac{n \pi}{b})^2 - w^2 \mu \epsilon}$ <br>
波导波长： $\lambda_{gmn} = \frac{2 \pi}{\beta_{mn}} = \frac{\lambda}{\sqrt{1 - (f_{cmn}/f)^2}}$ <br>
相速度： $v_{pmn} = \frac{w}{\beta_{mn}} = \frac{v_p}{\sqrt{1 - (f_{cmn}/f)^2}}$ <br>
波阻抗： $Z_{TM} = \frac{\beta_{mn}}{w \epsilon} = \eta \sqrt{1 - (\frac{f_{cmn}}{f})^2}$ <br>
$Z_{TE} = \frac{w \mu}{\beta_{mn}} = \frac{\eta}{\sqrt{1 - (f_{cmn}/f)^2}}$ <br>

### 主模
截止频率最低，工作频带最宽，TE波的m、n可以取0 ，当长边取1短边取0时得到最小的截止波数（假设a是长边，b是短边）<br>
$TE_{10}$ 的 $k_{c10} = \frac{\pi}{a}$ <br>

管壁电流的概念，切断管壁电流 <br>

单模传输，模式分布图 <br>

$TE_{10}$ 的传输功率：
$P = \frac{1}{2 Z_{TE_{10}}} \int \int E_m^2 sin^2(\pi / ax) dx dy = \frac{ab}{4 Z_{TE_{10}}} E_m^2$

## 7.3 谐振腔
在矩形谐振腔内波来回反射形成驻波，引入一个新的模式p用于表示驻波 <br>
$k_{mnp} = \sqrt{(\frac{m \pi}{a})^2+(\frac{n \pi}{b})^2+(\frac{p \pi}{l})^2}$ <br>

$TM_{mnp}$ 波m、n 不能为0， p可以为0； $TE_{mnp}$ 波m、n可以但不同时为0，p不能为0 <br>




# 8 电磁辐射
## 8.1 滞后位
观察点的位场变化滞后于源的变化，推迟的时间恰好是源的变化以速度 $ v = \frac{1}{\sqrt{\mu \epsilon}}$ 传播到观察点所需的时间，称为滞后现象。时间上的滞后可以转移到相位上。


## 8.2 电偶极子

### 近场区
时变电偶极子近场与静电偶极子一样，称为准静态场，电偶极子没有能力向外辐射（近似情况下）。

### 远场区
$E_{\theta} = j \frac{I l \eta_0}{2 \lambda r} sin \theta e^{- j k r}$ <br>
$H_{\phi} = j \frac{I l}{2 \lambda r} sin \theta e^{- j k r} $ <br>
没有相位差； <br>
远场是辐射场，电磁波沿径向r入射，<br>
是TEM波， $\eta_0 = 120 \pi $ <br>
具有方向性，跟 $\theta$ 有关 <br>
振幅随 r 增大而衰减 <br>

辐射功率： $P_r = 40 \pi^2 I^2 (\frac{l}{\lambda})^2$ <br>
辐射电阻： $R_r = 2 P_r / I^2 = 80 \pi^2 (\frac{l}{\lambda})^2$ <br>


## 8.3 天线
归一化方向性函数： $F(\theta, \phi)$ <br>
主瓣宽度： 
副瓣电平： 要求尽可能低 <br>
前后比： 优秀尽可能大 <br>
方向性系数： $D = \frac{4 \pi}{\int_0^{2 \pi} \int_0^{\pi} F^2(\theta, \phi) sin \theta d \theta d \phi}$ <br>
效率： 辐射功率与输入功率的比值；要尽可能增大辐射电阻，降低损耗电阻。 <br>
增益系数： $G = \eta_A D$ <br>

### 对称天线
$F(\theta, \phi) = \frac{cos(kl cos \theta) - coskl}{sin \theta}$ <br>
$E_{\theta} = j \frac{60 I}{r} F(\theta, \phi) e^{-jkr}$ <br>
记住归一化方向性函数和方向性系数就都可以求了。 <br>
电偶极子的电场、辐射电场公式不能再天线这直接套用。 <br>


### 天线阵
天线一定规律排列成一个阵列，获得期望的辐射方向性、更高的增益等。组成天线的独立的单元称为阵元。 <br>
得到电场模为 $\frac{60 I}{r} F(\theta, \phi) F_{ar}(\theta, \phi)$ <br>
即要多乘以一个阵因子 $F_{ar}(\theta, \phi)$ <br>


均匀直线阵会出现多个主瓣和副瓣。 <br>

# Tips

电介质，磁介质的极化磁化电荷怎么求 <br> 
$P = (\epsilon - \epsilon_0)E$ <br>
$\rho_s = P \cdot e_n$ <br>
体极化电荷： $\rho_P = - \nabla \cdot P$ <br>
$M = \frac{B}{\mu_0} - H$<br>
$J_s = M \times e_n$<br>
体磁化电流： $J_M = \nabla \times M$ <br>

如果知道P或者M就根据公式求，如果不知道就根据<br>
$D=\epsilon E = \epsilon_0 E + P$  求出P再用公式<br>


导体中不能存在静电场  <br>
电位移矢量点乘法向量等于面电荷密度 p67例2.42<br>

两个导体之间知道电势差，求解E可以先假设电荷q，用高斯定律，再把q换成电势差<br>
同心导体圆柱电场分布<br>