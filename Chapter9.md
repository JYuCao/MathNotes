---
title: 多元函数积分学及其应用
markmap:
  colorFreezeLevel: 3
---

# 多元函数积分学及其应用
## 三重积分与线面积分
### 三重积分
- 直角坐标：先一后二、先二后一
- 柱坐标：$\iiint_\Omega f(x,y,z)=\iiint_\Omega f(r\cos\theta,r\sin\theta,z)rdrd\theta dz$
- 球坐标：$\iiint_\Omega f(x,y,z)=\iiint_\Omega f(r\sin\varphi\cos\theta,r\sin\varphi\sin\theta,r\cos\varphi)r^2\sin\varphi drd\varphi d\theta$
- 利用奇偶性和对称性

### 对弧长的线积分（第一类）
- 积分与路径方向无关
- 直接法：$\int_Lf(x,y)ds=\int_\alpha^\beta f(x(t),y(t))\sqrt{x'^2(t)+y'^2(t)}dt$
- 奇偶性与对称性

### 对坐标的线积分（第二类）
- 积分与路径方向有关
- 直接法：$\int_LPdx+Qdy=\int_\alpha^\beta [P(x(t),y(t))x'(t)+Q(x(t),y(t))y'(t)]dt$
- 格林公式：$\oint_LPdx+Qdy=\iint_D(\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y})d\sigma$
- 补线用格林公式
- 利用线积分与路径无关
    - 若函数P, Q在D上有一阶连续偏导数
        - 线积分$\int_LPdx+Qdy$与路径无关
        - $\oint_LPdx+Qdy=0$
        - $\frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$
        - $P(x,y)dx+Q(x,y)dy=dF(x,y)$
    - 计算
        - 改换路径计算
        - 利用原函数计算
- 两类线积分的联系：$\oint_LPdx+Qdy=\oint_L(P\cos\alpha+Q\cos\beta)ds$
- 计算方法（空间）
    - 直接法
    - 斯托克斯公式

### 对面积的面积分（第一类）
- 与积分曲面的方向无关
- 直接法：$\iint_\Sigma f(x,y,z)dS=\iint_{D_{xy}}f[x,y,z(x,y)]\sqrt{1+z_x'^2+z_y'^2}dxdy$
- 奇偶性与对称性

### 对坐标的面积分（第二类）
- 与积分曲面的方向有关
- 直接法：曲面的上侧前侧和右侧为正面
- 高斯公式
- 补面用高斯公式
- 两类面积分的联系：$\iint_\Sigma (P\cos\alpha+Q\cos\beta+R\cos\gamma)dS=\iint_\Sigma(Pdydz+Qdzdx+Rdxdy)$

### 常考题型
#### 计算三重积分
> 1. 高辅P253例3（柱坐标）
> 2. 高辅P253例5（化简三重积分后求极限）
> 3. 高辅P254例6（三重积分交换次序）
> 4. 660P210 596（三重积分）<br>
> 先一后二看切面，先二后一看投影

#### 计算对弧长的线积分
> 1. 高辅P255例3（双纽线）
> 2. 高辅P255例4（化简空间曲线）

#### 计算对坐标的线积分
> 1. 高辅P257例4(2)（挖0点用格林）<br>
> P258注有多种特殊式，需留意
> 2. 高辅P258例6（格林公式证明题，以及求参数）
> 3. 高辅P260例9（格林公式，形心公式、轮换对称性、不等式）
> 4. 高辅P261例10（三维曲线的处理方法）
> 5. 660P214 609<br>
>   - 直接法：参数方程代换为一重积分
>   - 斯托克斯：要计算曲线法线方向向量
>   - 降维：代换x/y/z，化为二维曲线积分

#### 计算对面积的面积分
> 1. 660P211 600（利用形心公式）
> 2. 660P212 603（轮换对称性）

#### 计算对坐标的面积分
> 1. 高辅P266例5（直接法）<br>
> 高斯公式要求被导因子有连续一阶导数
> 2. 660P215 611（代换降维）
> 2. 660P230 653（第二类曲面积分奇偶性与第一类相反）

## 多元函数积分应用
### 应用
- 面积、体积、弧长
- 质量、质心、转动惯量
- 变力做功
- 向量场、通量

### 常考题型
#### 求几何量
> 1. 高辅P268例2（求面积：面积分、线积分？）
> 2. 高辅P269例3（求面积最大值）

#### 计算物理量
> 1. 高辅P270例3（求奇怪锥体的形心）
> 2. 660P215 613（转动惯量）

## 场论初步
### 梯度
- $\boldsymbol{grad} u = \frac{\partial u}{\partial x}\boldsymbol{i}+\frac{\partial u}{\partial y}\boldsymbol{j}+\frac{\partial u}{\partial z}\boldsymbol{k}$

### 散度
- $div\boldsymbol{A}=\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}+\frac{\partial R}{\partial z}$

### 旋度
- $\boldsymbol{rot} \boldsymbol{A}=
\begin{vmatrix}
\boldsymbol{i} & \boldsymbol{j} & \boldsymbol{k} \\
\frac{\partial}{\partial x} & \frac{\partial}{\partial y} & \frac{\partial}{\partial z}\\
P & Q & R
\end{vmatrix}$

### 常考题型
#### 梯度、散度、旋度的计算
