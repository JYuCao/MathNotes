---
title: 向量代数与空间解析几何及多元函数在几何上的应用
markmap:
  colorFreezeLevel: 3
---

# 向量代数与空间解析几何
## 向量代数
### 数量积（点乘）
### 向量积（叉乘）
- 交换律：要变号
- $S=|\boldsymbol {a} \times \boldsymbol {b}|$表示平行四边形面积
### 混合积
- 轮换对称性和交换变号
- $ V_{平行六面体}=|(\boldsymbol {a} \boldsymbol {b} \boldsymbol {c})| $
- 判定三向量共面：$(\boldsymbol {a} \boldsymbol {b} \boldsymbol {c})=0$

### 常考题型
#### 向量运算

#### 向量运算的应用及向量的位置关系
> 1. 高辅P231例1（角平分线）<br>
> 求角平分线向量： $\boldsymbol {c} = \lambda(\frac{\boldsymbol {a}}{|a|}+\frac{\boldsymbol {b}}{|b|})$（$\lambda$用于确定模的大小）
> 2. 高辅P232例2（证明题，三点共线）

## 空间平面与直线
### 平面方程

### 直线方程

### 平面与直线的位置关系（平行、垂直、夹角）

### 点面距
- $d=\frac{|Ax_0+By_0+Cz_0+D|}{\sqrt{A^2+B^2+C^2}}$

### 点线距
- $d=\frac{|(x_1-x_0,y_1-y_0,z_1-z_0)\times(l,m,n)|}{\sqrt{l^2+m^2+n^2}}$

### 常考题型
#### 建立直线方程
> 一般式表示的直线求方向向量采用 __叉乘__<br><br>
> 1. 高辅P233例2（直线相交）
> 2. 660P232 659（空间曲线的切线方程）

#### 建立平面方程
> [平面束方程](https://www.bilibili.com/video/BV13j411b7PE/?spm_id_from=333.337.search-card.all.click&vd_source=0f675bd8d9f836748979b9492a924e4f)

#### 与平面和直线位置有关的问题

## 曲面与空间曲面
### 曲面方程
- 一般式

### 空间曲线
- 参数式
- 一般式（两曲面相交）

### 常见曲面
- 旋转面：设$L$为$yOz$面上一条曲线
    - 绕$y$轴旋转得$f(y,\pm\sqrt{x^2+z^2})=0$
    - 绕$y$轴旋转得$f(\pm\sqrt{x^2+y^2},z)=0$

- 柱面
- 二次曲面
  - 椭圆锥面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}=z^2$，圆锥面：$x^2+y^2=z^2$
  - 椭球面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}+\frac{z^2}{c^2}=1$，球面：$x^2+y^2+z^2=1$
  - 单叶双曲面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}-\frac{z^2}{c^2}=1$
  - 双叶双曲面：$\frac{x^2}{a^2}-\frac{y^2}{b^2}-\frac{z^2}{c^2}=1$
  - 椭圆抛物面：$\frac{x^2}{a^2}+\frac{y^2}{b^2}=z$，旋转抛物面：$z=x^2+y^2$
  - 双曲抛物面（马鞍面）：$\frac{x^2}{a^2}-\frac{y^2}{b^2}=z$

### 空间曲线投影

### 常考题型
#### 建立柱面方程
> 1. 高辅P238例2（求平行与某直线的柱面方程）

#### 建立旋转面方程
> 2. 高辅P239例2（直线绕轴旋转）<br>
> 第一步，将直线化为参数方程；第二步，求$x^2+y^2=f(t)$（若绕z轴）；第三步，将$t=g(z)$代入f(t)即可。

#### 求空间曲线的投影曲线方程

## 多元函数微分在几何上的应用
### 曲面的切平面与法线
- $F(x,y,z)=0$对应法向量$\boldsymbol {n}=(F'_x,F'_y,F'_z)$
- $z=f(x,y)$对应法向量$\boldsymbol {n}=(F'_x,F'_y,-1)$

### 曲线的切线与法平面
- 参数式：切向量为对应导数值
- 交面式：切向量为两曲面法向量的叉乘

### 常考题型
#### 建立曲面的切平面和法线方程
> 1. 高辅P240例2（直线在平面上，平面与曲面相切，求直线方程参数） 
> 2. 高辅P241例4（证明曲面为柱面）<br>
> 要证明曲面为柱面，只需证明曲面上任意一点的法向量垂直于定向量

#### 建立空间曲线的切线和法平面方程

## 方向导数与梯度
### 方向导数
- 定义：$\frac{\partial f}{\partial \boldsymbol{l}}|_{(x_0,y_0)}=\lim_{t\rightarrow0^+}\frac{f(x_0+t\cos\alpha, y_0+t\cos\beta)-f(x_0,y_0)}{t}$
- $\frac{\partial f}{\partial \boldsymbol{l}}=\frac{\partial f}{\partial x}\cos\alpha+\frac{\partial f}{\partial y}\cos\beta$

### 梯度
- $\boldsymbol{grad} z = \frac{\partial f}{\partial x}\boldsymbol{i}+\frac{\partial f}{\partial y}\boldsymbol{j}$

### 常考题型
#### 方向导数与梯度的计算
> 1. 高辅P244例2（方向导数定义判断存在性）
> 2. 高辅P245例5（方向导数证明二元函数存在最小点）
> 3. 660P229 649、650（圆和球的切向量方向导数）
> 4. 660P231 657（梯度和方向导数）
> 5. 660P232 660（方向导数与切向量）
