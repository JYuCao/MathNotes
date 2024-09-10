---
title: 函数 极限 连续
markmap:
  colorFreezeLevel: 4
---

## 函数

### 概念与性质
#### 单调性

#### 奇偶性
- 连续奇函数的原函数都为偶函数，但连续偶函数的原函数有且仅有一个为奇函数
#### 周期性
- 周期函数的导函数为周期函数，原函数不一定是周期函数
- 周期函数的原函数算是周期函数的充要条件是其在一个周期上的积分为零
即 $F(x)=\int^{x}_{0}{f(t)dt}$是以T为周期的周期函数$\Leftrightarrow\int^{T}_{0}{f(t)dt}=0$
#### 有界性
- $f(x)$在$[a,b]$上连续$\Rightarrow f(x)$在$[a,b]$上有界；
- $f(x)$在$(a,b)$上连续，且$f(a^+)$和$f(a^-)$存在$\Rightarrow f(x)$在$(a,b)$上有界；
- $f^{'}(x)$在区间$I$（有限）上有界$\Rightarrow f(x)$在$I$上有界

### 常考题型
#### 复合函数
定义域、值域、复合函数和函数的相互转化等

#### 函数性态
连续、奇偶、周期、有界

- 变上限积分函数的奇偶性
> 1. 高辅P8注（变上限积分函数奇偶性）
> * $f(x)$奇$\Rightarrow \int^x_af(t)dt$偶
> * $f(x)$偶$\Rightarrow \int^x_0f(t)dt$奇 <br>
> &emsp;&emsp;&emsp;&nbsp;$\nRightarrow \int^x_af(t)dt$奇

## 极限
### 概念与性质
- 局部有界性
- 保号性
- 极限值与无穷小的转换：$\lim f(x)=A\Leftrightarrow f(x)=A+\alpha$

- 极限存在准则
  - 夹逼准则
  - 单调有界准则

### 无穷小
- 高阶、同阶、等价
- k阶：$\lim \frac{\beta(x)}{[\alpha(x)]^k}=C\neq 0$
- 性质
  - 有限个无穷小的和仍是无穷小
  - 有限个无穷小的积仍是无穷小
  - 无穷小量与有界量的积仍是无穷小

### 无穷大

### 常考题型
#### 极限的概念、性质及存在准则
> 1. 高辅P12例1及注
> 
> * 若$\lim_{n\rightarrow \infty}a_n=a$，则$\lim_{n\rightarrow \infty}|a_n|=|a|$，_反之不成立_
> * $\lim_{n\rightarrow \infty}a_n=0 \Leftrightarrow \lim_{n\rightarrow \infty}|a_n|=0$
> 2. 高辅P13例3（无穷小和无穷大乘积关系）
> 3. 高辅P14例6（不等式证明和数列收敛）

#### 求极限
- 常用极限
- 等价无穷小
- 洛必达法则
- 泰勒展开
- 夹逼准则
- 定积分的定义


## 连续