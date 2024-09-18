---
title: 常微分方程
markmap:
  colorFreezeLevel: 3
---

# 常微分方程
## 一阶微分方程
- 可分离变量的方程：$\int g(y)dy=\int f(x)dx$
- 齐次方程：$\frac{dy}{dx}=\varphi(\frac{y}{x})$
- 线性方程：$y'+p(x)y=q(x)$
- 伯努利方程：$y'+p(x)y=Q(x)y^n$

> 求解齐次方程的方法：<br>
> 令$u=\frac{y}{x}$，则$y'=u+xu'$，从而将原方程化为$xu'=\varphi(u)-u$<br><br>
> 线性方程通解公式：<br>
> $y=e^{-\int p(x)dx}(\int Q(x)e^{\int p(x)dx}dx)+C$<br><br>
> 伯努利方程一般方法：<br>
> 令$u=y^{1-n}$，化简方程为一阶线性微分方程<br><br>

## 全微分方程：
- 偏积分
- 凑积分
- 线积分

> - $du(x,y)=P(x,y)dx+Q(x,y)dy$，通解为$u(x,y)=C$
> - 当$P(x,y),Q(x,y)$在单连通域$G$内具有连续偏导数时，方程是全微分方程的充要条件是<br>
> $$\frac{\partial P}{\partial y}=\frac{\partial P}{\partial x}$$

## 可降阶的高阶方程
- $y^{(n)}=f(x)$型
- $y''=f(x,y')$型
- $y''=f(y,y')$型

> - $y''=f(x,y')$型：只需令$y'=p,y''=p'$
> - $y''=f(y,y')$型：只需令$y'=p,y''=p\frac{dp}{dy}$

## 高阶线性微分方程
### 解的结构
#### 齐次方程与非齐次方程
- 齐次方程：$y''+p(x)y'+q(x)y=0$
- 非齐次方程：$y''+p(x)y'+q(x)y=f(x)$
#### 定理
- 定理1：若$y_1(x)$和$y_2(x)$是齐次方程(1)的两个线性无关的特解，那么$y=C_1y_1(x)+C_2y_2(x)$就是方程(1)的通解
- 定理2：如果$y^*$是非齐次方程(2)的一个特解，$y_1(x)$和$y_2(x)$是齐次方程(1)的两个线性无关的特解，则$y=C_1y_1(x)+C_2y_2(x)+y^*(x)$是非齐次方程(2)的通解
- 定理3：如果$y_1^*(x),y_2^*(x)$是非齐次方程(2)的两个特解，则$y(x)=y_1^*(x)-y_2^*(x)$是齐次方程(1)的解
- 定理4：如果$y_1^*(x),y_2^*(x)$分别是方程$y''+p(x)y'+q(x)y=f_1(x),\\ y''+p(x)y'+q(x)y=f_2(x)$的特解，则$y_1^*(x)+y_2^*(x)$是方程$y''+p(x)y'+q(x)y=f_1(x)+f_2(x)$的解

> 方程(1)的两个解线性无关的充要条件是它们只比不为常数

### 常系数齐次线性微分方程
- 解方程特征值，得到两根$r_1,r_2$
  - 若$r_1\neq r_2$，则齐次方程通解为$y=C_1e^{r_1x}+C_2e^{r_2x}$
  - 若$r_1=r_2$，则齐次方程通解为$y=(C_1+C_2x)e^{r_1x}$
  - 若$r_1=\alpha+i\beta,r_2=\alpha-i\beta$，则齐次方程通解为$y=e^{\alpha x}(C_1\cos{\beta x}+C_2\sin{\beta x})$

### 常系数非齐次线性微分方程
- 若非齐次方程中$f(x)=P_m(x)e^{\lambda x}$，则可设其特解为$y^*=x^kQ_m(x)e^{\lambda x}$
- 若非齐次方程中$f(x)=e^{\alpha x}[P_l(x)\cos\beta x+P_n(x)\sin\beta x]$，则可设其特解为$y^*=x^ke^{\alpha x}[R_m^{(1)}(x)\cos\beta x+R_m^{(2)}(x)\sin\beta x]$

### 欧拉方程
- $x^ny^{(n)}+p_1x^{n-1}y^{(n-1)}+\cdots+p_{n-1}xy'+p_ny=f(x)$
- 解法：令$x=e^t或t=\ln x$，化为$x^ky^{(k)}=D(D-1)\cdots(D-k+1)y$

> D代表对t的导数运算

## 常考题型