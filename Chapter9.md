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

#### 计算对弧长的线积分
> 1. 高辅P255例3（双纽线）
> 2. 高辅P255例4（化简空间曲线）

