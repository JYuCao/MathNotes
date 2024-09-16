---
title: 一元函数积分学
markmap:
  colorFreezeLevel: 3
---
# 一元函数积分学
## 不定积分
### 原函数存在性
- 若$f(x)$在区间$I$上连续，则$f(x)$在区间I上必有原函数
- 若$f(x)$在区间$I$上有第一类间断点，则在$f(x)$区间$I$上没有原函数

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
> 3. 高辅P98例11（分母为三角函数相乘的处理方法）
> 3. 高辅P98例12（分母为三角函数相乘的处理方法）
>   - 满足$R(-\sin x,\cos x)=-R(\sin x,\cos x)$，凑$d\cos x$
>   - 满足$R(-\sin x,-\cos x)=R(\sin x,\cos x)$，凑$d\tan x$

#### 不定积分杂例

## 定积分
### 可积性
- 必要条件：若$\int_a^bf(x)dx$存在，则$f(x)$在$[a,b]$上有界
- 充分条件
    - 若$f(x)$在$[a,b]$上连续，则$\int_a^bf(x)dx$必定存在
    - 若$f(x)$在$[a,b]$上有界，且只有有限个间断点，则$\int_a^bf(x)dx$必定存在
    - 若$f(x)$在$[a,b]$上只有有限个第一类间断点，则$\int_a^bf(x)dx$必定存在

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

#### 定积分的计算
> 1. 高辅P107例2（周期性）
> 2. 高辅P108例4（周期性，证明了下列重要结论）<br>
> $\int_0^{2\pi} \cos^n xdx=4\int_0^{\frac{\pi}{2}}\sin^n xdx=4\int_0^{\frac{\pi}{2}}\sin^n xdx(n为偶数)$<br>
(使用华里士公式)<br>
> $\int_0^{2\pi} \cos^n xdx=\int_0^{2\pi}\sin^n xdx=0(n为奇数)$<br><br>
> 补充：$\int_0^\pi x\sin xdx=\frac{\pi}{2}\int_0^\pi\sin xdx=\pi$<br><br>
> 3. 高辅P109例7（构造变上限积分函数求解抽象积分）