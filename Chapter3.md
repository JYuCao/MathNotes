---
title: 一元函数积分学
markmap:
  colorFreezeLevel: 3
---
# 一元函数积分学
## 不定积分
### 原函数存在性
- 若$f(x)$在区间$I$上连续，则$f(x)$在区间I上必有原函数
- 若$f(x)$在区间$I$上有第一类或无穷间断点，则在$f(x)$区间$I$上没有原函数
- 若$f(x)$在区间$I$上有震荡间断点，则在$f(x)$区间$I$上不一定有原函数

### 规律
- 区间上有原函数，被积函数不一定连续
- 原函数一定可导和连续

### 积分法
- 第一类换元
- 第二类换元
- 分部积分

### 常考题型
#### 计算不定积分
> 1. 高辅P97例8（配立方差）<br>
> 立方和（差）公式：$1\pm x^3=(1\pm x)(1\mp x+x^2)$
> 2. 高辅P97注（1进阶，综合）<br><br>
> 3. 高辅P97例9（分母为三角函数+常数的处理方法）<br>
> 三角函数万能代换：$\tan\frac{x}{2}=t$，则<br>
> $\int R(\sin x,\cos x)dx=\int R(\frac{2t}{1+t^2},\frac{1-t^2}{1+t^2})\frac{2}{1+t^2}dt$<br><br>
> 4. 高辅P98例11（分母为三角函数相乘的处理方法）
> 5. 高辅P98例12（分母为三角函数相乘的处理方法）
>   - 满足$R(-\sin x,\cos x)=-R(\sin x,\cos x)$，凑$d\cos x$
>   - 满足$R(-\sin x,-\cos x)=R(\sin x,\cos x)$，凑$d\tan x$<br><br>
> 6. 660P22 52（第一类换元）
> 7. 660P22 54（第一类换元）

#### 不定积分杂例
> 1. 660P61 176（不定积分原函数性质判定）
> 1. 660P70 199（不定积分原函数存在性）

## 定积分
### 可积性
- 必要条件：若$\int_a^bf(x)dx$存在，则$f(x)$在$[a,b]$上有界
- 充分条件
    - 若$f(x)$在$[a,b]$上连续，则$\int_a^bf(x)dx$必定存在
    - 若$f(x)$在$[a,b]$上有界，且只有有限个间断点，则$\int_a^bf(x)dx$必定存在
    - 若$f(x)$在$[a,b]$上只有有限个第一类间断点，则$\int_a^bf(x)dx$必定存在

### 规律
- 可导必连续，连续必可积，可积必有界
- 无界必不可积，有无数个间断点必不可积
- 有界不一定可积

#### 运算
- 可积$\pm$可积$=$可积
- 可积$\pm$不可积$=$不可积
- 不可积$\pm$不可积$=$不一定
- 可积$\times$可积$=$可积
- 可积$\times$不可积$=$不一定
- 不可积$\times$不可积$=$不一定

### 计算法
- 牛顿-莱布尼茨公式
- 换元积分
- 分部积分
- 利用奇偶性和周期性
- 公式

### 变上限积分
- $(\int_{\varphi(x)}^{\psi(x)}f(t)dt)'=f(\psi(x))\psi'(x)-f(\varphi(x))\varphi'(x)$
- $(\int_{\varphi(x)}^{\psi(x)}f(x,t)dt)'=\int_{\varphi(x)}^{\psi(x)}\frac{\partial f(x,t)}{\partial x}dt+f(x,\psi(x))\psi'(x)-f(x,\varphi(x))\varphi'(x)$
- $(\int_a^bf(x,t)dt)'=\int_a^b\frac{\partial f(x,t)}{\partial x}dt$

### 性质
#### 不等式
- 若$f(x)\leq g(x),x\in[a,b]$，则$\int_a^bf(x)dx\leq\int_a^bg(x)dx$
- 若$f(x)$在$[a,b]$上连续，则$m(b-a)\leq\int_a^bf(x)dx\leq M(b-a)$，
其中$m,M$分别为$f(x)$在$[a,b]$上的最小值与最大值
- $|\int_a^bf(x)dx|\leq\int_a^b|f(x)|dx$

#### 积分中值定理
- 积分中值定理：若$f(x)$在$[a,b]$上连续，则
$\int_a^bf(x)dx=f(\xi)(b-a),a<\xi<b$
- 广义积分中值定理：若$f(x),g(x)$在$[a,b]$上连续，且$g(x)$不变号，则
$\int_a^bf(x)g(x)dx=f(\xi)\int_a^bg(x)dx,a\leq\xi\leq b$

### 常考题型
#### 定积分的概念、性质及几何意义
> 1. 高辅P105注1（求n项连乘极限：取对数用定积分定义）
> 2. 高辅P106注（广义积分中值定理）
> 3. 660P62 177（定积分原函数性质判定）
> 4. 660P63 180（定积分原函数存在性）
> 5. 660P63 181（定积分原函数性质）

#### 定积分的计算
- 三角函数定积分公式
  - $\int_0^{\frac{\pi}{2}} f(\sin x)dx = \int_0^{\frac{\pi}{2}} f(\cos x)dx$
  - $\int_0^{\frac{\pi}{2}} f(\sin x)dx = \int_{\frac{\pi}{2}}^{\pi} f(\sin x)dx$
  - $\int_0^{\pi} f(\sin x)dx = 2\int_0^{\frac{\pi}{2}} f(\sin x)dx$
  - $\int_0^\pi x f(\sin x)dx=\frac{\pi}{2}\int_0^\pi f(\sin x)dx$
  - 华里士公式（点火公式）
  - 例2结论

> 1. 高辅P107例2（周期性）
> 2. 高辅P108例4（周期性，证明了下列重要结论）<br>
> $  \left\{
    \begin{aligned}
      \int_0^{2\pi} \cos^n xdx=4\int_0^{\frac{\pi}{2}}\sin^n xdx=4\int_0^{\frac{\pi}{2}}\sin^n xdx(n为偶数) \\
      \int_0^{2\pi} \cos^n xdx=\int_0^{2\pi}\sin^n xdx=0(n为奇数)
    \end{aligned}
  \right.$<br><br>
> 补充：$\int_0^\pi x f(\sin x)dx=\frac{\pi}{2}\int_0^\pi f(\sin x)dx$（其实可由4结论推出）<br><br>
> 3. 高辅P109例7（构造变上限积分函数求解抽象积分）<br><br>
> 4. 高辅P109例8（三角函数，利用变量代换计算定积分）<br>
> 一般地，$\int_a^bf(x)dx\overset{x=a+b-t}{====}\int_a^bf(a+b-t)dt$
> 5. 高辅P110例11（分部解抽象函数定积分）
> 6. 660P26 64（变量代换，方法同4）<br><br>
> 7. 高辅P111例12（凑因子解抽象函数定积分）
> 8. 高辅P111注（综合4,6）<br><br>
> 9. 660P24 59（换元分部）
> 10. 660P25 61（抽象函数换元）
> 11. 660P66 188（换元，平移变换）

#### 变上限积分的函数及其应用
- 连续性：函数在区间上可积，则变上限积分连续
- 可导性：
  - $f(x)$在区间上连续，变上限积分可导，导数值为$f(x_0)$
  - $x_0$处为可去间断点，变上限积分可导，导数值为$\lim_{x\rightarrow x_0}f(x_0)$
  - $x_0$处为跳跃间断点，变上限积分连续但不可导，
  偏导值分别为$f(x)$在$x_0$处的左右极限
- 奇偶性：函数和变上限积分奇偶性相反

> 1. 高辅P114例6（变上限的（广义）积分中值定理）<br>
> 常用方法：洛必达、等价无穷小、积分中值定理<br><br>
> 2. 高辅P116注（变上限积分函数最值，带绝对值）<br><br>
> 3. 高辅P116例10（由变上限积分方程求函数）<br><br>
> 4. 660P68 194（分段函数变上限积分函数的可导性）<br>
> $x_0\in(a,b),f(x)$在$[a,b]$除$x_0$外连续且在$[a,b]$有界，考察$\int_a^xf(t)dt$<br>
> - $F'(x)=f(x)(x\in[a,b],x\neq x_0)$
> - 若$x=x_0$是$f(x)$跳跃间断点，则$F'_{\pm}(x_0)$均存在但不相等$F'_{\pm}(x_0)=f(x_0^{\pm})$
> - 若$x=x_0$是$f(x)$可去间断点，则$F'(x_0)$存在但$F'(x_0)\neq x_0$或$F'(x_0)$无定义<br><br>


#### 积分不等式
- 变量代换
- 积分中值定理
- 变上限积分
- 柯西积分不等式（$(\int_a^bf(x)g(x)dx)^2\leq\int_a^bf^2(x)dx\int_a^bg^2(x)dx$）

> 1. 高辅P120例5（不等式：函数与变上限积分转换）
> 2. 高辅P120注（1plus）<br><br>
> 3. 高辅P121例6（柯西积分不等式）
> 4. 高辅P121注（3plus）<br><br>

## 反常积分
### 无穷区间的反常积分判别法
- 比较判别法
- 比较法的极限形式：$\lim_{x\rightarrow+\infty}\frac{f(x)}{g(x)}=\lambda$
  - 当$\lambda>0$时，$\int_a^{+\infty}f(x)$与$\int_a^{+\infty}g(x)$同敛散
  - 当$\lambda=0$时，若$\int_a^{+\infty}g(x)$收敛，则$\int_a^{+\infty}f(x)$也敛散
  - 当$\lambda=+\infty$时，若$\int_a^{+\infty}g(x)$发散，则$\int_a^{+\infty}f(x)$也发散
- 常用结论：$\int_a^{+\infty}\frac{1}{x^p}dx
  \left\{
    \begin{aligned}
      p>1, 收敛 \\
      p\leq1, 发散
    \end{aligned}
  \right.(a>0)$

### 无界函数的反常积分（瑕积分）判别法
- 比较判别法
- 比较法的极限形式（同无穷区间判别）
- 常用结论
  - $\int_a^b\frac{1}{(x-a)^p}dx
  \left\{
    \begin{aligned}
      p<1, 收敛 \\
      p\geq1, 发散
    \end{aligned}
  \right.$
  - $\int_a^b\frac{1}{(b-x)^p}dx
  \left\{
    \begin{aligned}
      p<1, 收敛 \\
      p\geq1, 发散
    \end{aligned}
  \right.$
### 常考题型
#### 反常积分的敛散性
> 1. 高辅P124例2（反常/瑕积分结合判别）
> 2. 高辅P124例3（瑕积分判别）<br>
> $\lim_{x\rightarrow0}x^\xi \ln x = 0(\xi为任意正常数)$<br>
> 上式中$\xi$可以取的非常小，哪怕是0.0001，整个式子也趋于0<br><br>
> 3. 660P27 68（反常积分敛散性求参数）<br><br>
> 4. 660P27 69（求反常积分，带$e^x$的变换）
> 5. 660P71 203（反常积分敛散性判别法）
> 6. 660P72 204（反常积分敛散性性质）


#### 反常积分的计算
> 1. 高辅P126例4（换元）

## 定积分应用
### 几何应用
- 平面图形的面积（$S=\iint_D1d\sigma$）
- 空间体的体积
  - 旋转体的体积
    - 二重积分法：$V=2\pi\iint_Dr(x,y)d\sigma$
    - 古尔丁定理：$V=2\pi r\cdot S$（r为形心到旋转轴的距离）
  - 已知横截面的面积（$V=\int_a^bS(x)dx$）
> 形心公式：$(\frac{\iint_Dxdxdy}{\iint_Ddxdy},\frac{\iint_Dydxdy}{\iint_Ddxdy})$

### 曲线弧长
- 直角坐标：$s=\int_a^b\sqrt{1+y'^2}dx$
- 参数方程：$s=\int_\alpha^\beta\sqrt{x'^2(t)+y'^2(t)}dt$
- 极坐标：$s=\int_\alpha^\beta\sqrt{r^2(\theta)+r'^2(\theta)}d\theta$

### 旋转体侧面积
- $S=2\pi\int_a^bf(x)\sqrt{1+f'^2(x)}dx$

### 物理应用
- 变力延直线所做的功
- 液体的压力
- 引力

### 常考题型
#### 几何应用
> 1. 高辅P129注（函数围成面积的最小值）
> 2. 660P28 70（摆线）
> 3. 660P28 71（星形线，答案含隐函数表示）
> 4. 660P73 208（质心）<br>
> $(\bar{x}, \bar{y})=(\frac{\int_\alpha^\beta x\sqrt{x'^2+y'^2}dt}{\int_\alpha^\beta \sqrt{x'^2+y'^2}dt},\frac{\int_\alpha^\beta y\sqrt{x'^2+y'^2}dt}{\int_\alpha^\beta \sqrt{x'^2+y'^2}dt})$


#### 物理应用
> 1. 660P29 74（体积、速度、功）
