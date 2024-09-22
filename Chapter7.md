---
title: 无穷级数
markmap:
  colorFreezeLevel: 3
---

# 无穷级数
## 常数项级数
### 概念
- 级数与部分和
- 部分和极限存在，则级数收敛，反之则发散

### 性质
1. 若级数$\sum_{n=1}^\infty u_n$收敛于$S$，则级数$\sum_{n=1}^\infty ku_n$收敛于$kS$
2. 若$\sum_{n=1}^\infty u_n$和$\sum_{n=1}^\infty v_n$分别收敛于$S,\sigma$，则$\sum_{n=1}^\infty u_n\pm v_n$收敛于$S\pm\sigma$
    - 收敛$\pm$发散必发散
    - 发散$\pm$发散不一定发散
3. 级数中去掉、加上或改变有限项，不会改变级数的敛散性
4. 收敛级数加括号后仍收敛且和不变
    - 若级数加括号后收敛，原级数不一定收敛
    - 若级数加括号后发散，原级数一定发散    
5. 若级数$\sum_{n=1}^\infty u_n$收敛，则$\lim_{n\rightarrow\infty}u_n=0$
    - 若$\lim_{n\rightarrow\infty}u_n=0$，则级数不一定收敛
    - 若$\lim_{n\rightarrow\infty}u_n\neq0$，则级数一定发散

### 级数审敛准则
#### 正项级数
- 基本定理：$\sum_{n=1}^\infty u_n$收敛$\Leftrightarrow S_n$有界
- 比较判别法
- 比较判别法的极限形式：设$\lim_{n\rightarrow\infty}\frac{u_n}{v_n}=l(0\leq l\leq+\infty)$
    - 若$0<l<+\infty$，则$\sum_{n=1}^\infty u_n$与$\sum_{n=1}^\infty v_n$同敛散
    - 若$l=0$，则$\sum_{n=1}^\infty v_n$收敛$\Rightarrow\sum_{n=1}^\infty u_n$收敛，$\sum_{n=1}^\infty u_n$发散$\Rightarrow\sum_{n=1}^\infty v_n$发散
    - 若$l=+\infty$，则$\sum_{n=1}^\infty v_n$发散$\Rightarrow\sum_{n=1}^\infty u_n$发散，$\sum_{n=1}^\infty u_n$收敛$\Rightarrow\sum_{n=1}^\infty v_n$收敛

- 常用级数：
    - $\sum_{n=1}^\infty\frac{1}{n^p}$当$p>1$时收敛，$p\leq1$时发散
    - $\sum_{n=1}^\infty q^n$当$q<1$时收敛，$q\geq1$时发散

- 比值法：若$\lim_{n\rightarrow\infty}\frac{u_{n+1}}{u_n}=\rho$，则$\sum_{n=1}^\infty u^n=\left\{
    \begin{aligned}
      收敛,\rho<1,\\
      发散,\rho>1,\\
      不一定,\rho=1.
    \end{aligned}
  \right.$

- 根值法：若$\sqrt[n]{u_n}=\rho$，则$\sum_{n=1}^\infty u^n=\left\{
    \begin{aligned}
      收敛,\rho<1,\\
      发散,\rho>1,\\
      不一定,\rho=1.
    \end{aligned}
  \right.$
- 积分判别法：设$f(x)$是$[1,+\infty)$上单减非负的连续函数，且$a_n=f(n)$，则$\sum_{n=1}^\infty a_n$与$\int_1^{+\infty}f(x)dx$同敛散

#### 交错级数
- 莱布尼茨准则：${u_n}$单调减且$\lim_{n\rightarrow\infty}u_n=0$，则$\sum_{n=1}^\infty(-1)^{n-1} u_n$收敛

#### 任意项级数
- 绝对收敛与条件收敛
- 绝对收敛的级数一定收敛
- 条件收敛的级数所有正项或负项构成的级数一定发散
- 绝对$\pm$绝对$=$绝对
- 绝对$\pm$条件$=$条件
- 条件$\pm$条件$=$条件或绝对

### 常考题型
#### 正项级数敛散性的判定
> 1. 高辅P203例1(4)（积分判别法）
> 2. 高辅P203例2（放缩，代换，泰勒）
> 3. 高辅P204例3（比较判别法极限形式）

#### 交错级数敛散性的判定
> 1. 高辅P205例1(2)（三角函数变形）<br>
> $sin(x)=sin(n\pi+(x-n\pi))=(-1)^nsin(x-n\pi)$

#### 任意项级数敛散性的判定
> 1. 高辅P206例2（多情况）<br><br>
> 2. 高辅P206例3
> 3. 高辅P207例4<br>
> 思路：拆成多个简单级数进行判断
> 4. 高辅P208例7（直接求和看极限）<br>
> 等价无穷小代换只适用于正项级数

#### 证明题和综合题
> 1. 高辅P209例1（利用收敛数列有界性）
> 2. 高辅P210例3
> 3. 高辅P211例6（泰勒公式）

## 幂级数
### 收敛半径、收敛区间、收敛域
- 阿贝尔定理
    - 若$\sum_{n=0}^\infty a_nx^n$当$x=x_0(x_0\neq 0)$时收敛，则当$|x|<|x_0|$时，$\sum_{n=0}^\infty a_nx^n$绝对收敛
    - 若$\sum_{n=0}^\infty a_nx^n$当$x=x_0$时发散，则当$|x|
    >$|x_0|$时，$\sum_{n=0}^\infty a_nx^n$发散

- $\sum_{n=0}^\infty a_nx^n$的敛散性只有三种可能
    1. 对任何$x\in(-\infty,+\infty)$都收敛
    2. 仅在$x=0$处收敛
    3. 存在一个正数$R$，当$|x|<R$时绝对收敛，当$|x|>R$时发散

- 收敛半径和收敛域
    - 如果$\lim_{n\rightarrow\infty}|\frac{a_{n+1}}{a_n}|=\rho$，则$R=\frac{1}{\rho}$
    - 如果$\lim_{n\rightarrow\infty}|\sqrt[n]{|a_n|}|=\rho$，则$R=\frac{1}{\rho}$

### 性质
- 有理运算
- 分析性质
    - 连续性：和函数在收敛域连续
    - 可导性：和函数在收敛区间$(-R,R)$内可导，求导后收敛半径不变
    - 可积性：和函数在收敛域可积，积分后收敛半径不变

### 函数的幂级数展开
- 泰勒级数与麦克劳林级数
- 常用展开式
- 直接展开法和间接展开法

### 常考题型
#### 求收敛区间及收敛域
- 利用公式($a_n$已给出时)
- 阿贝尔定理($a_n$未给出时)

> 1. 高辅P215例1(4)（无法使用公式的情况）<br>
> 考虑带加减$(-1)^n$的幂级数，可以分解为奇次项和偶次项构成的两个幂级数<br><br>
> 注意：对只有偶次项或奇次项的幂级数求收敛半径，公式得到的值要开平方根<br><br>
> 2. 高辅P217例2（阿贝尔定理）
> 3. 高辅P217例3（根据收敛区间求参数）

#### 将函数展开为幂级数

