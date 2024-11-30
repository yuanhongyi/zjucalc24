# 模拟题分析与解答

依照【考情分析】，我给同学模拟了一些题目1-8为计算题，9为综合计算题，10-12为综合分析题

1-2属于极限部分  3-4属于导数部分  5-8属于积分部分

1.考察夹逼准则求极限

2.考察等价无穷小或者泰勒展开或者中值定理求极限

3.考察参数方程求导以及导数定义

4.考察复合函数求导以及导数定义

5.有理函数的不定积分，分部积分法

6.利用定积分定义求极限

7.定积分的几何应用，求曲线弧长

8.反常积分

9.定积分的几何应用，求旋转体体积

10.递推数列极限综合题

11.微分中值定理综合题，主要考察泰勒展开

12.函数与积分综合题，考察导数与单调性，积分不等式

10-12难度较大，但是我均做了铺垫

总体来说这张模拟卷的难度要高于期末考试，毕竟模拟总要难一点（别打我QWQ）

## 参考答案

TBD，有空再写（

1.计算极限

$$
\lim\limits_{x\to0}\dfrac{\sin(x^2\sin\dfrac{1}{x})}{x}
$$



---

2.计算极限

$$
\lim\limits_{x\to0}\dfrac{e^{(1+x)^{\frac{1}{x}}} - \left(1+x\right)^{\frac{e}{x}}}{x^2}
$$


---

3.设函数\(y = f(x)\)由参数方程\(\begin{cases}x = 1 + t^{3}\\y = e^{t^{2}}\end{cases}\)确定，求下面的极限：

$$\lim_{x\to+\infty}x\left[f\left(2+\frac{2}{x}\right)-f(2)\right]$$

---

4.设\(f(x)=\int_{0}^{x}\cos(x - t)^{2}\text{d}t\)，\(\varphi(x)=\begin{cases}\dfrac{x-\sin x}{x-\ln(1 + x)},&x\neq0\\0,&x = 0\end{cases}\)，求\(\dfrac{\mathrm{d}}{\mathrm{d}x}f(\varphi(x))\vert_{x = 0}\)

---

5.求不定积分

$$\int\ln\left(1+\sqrt{\dfrac{1+x}{x}} \right)\text{d}x $$

---

6.求下面的极限

$$
\lim\limits_{n\to+\infty}\dfrac{1}{n^4}\prod\limits_{k = 1}^{2n}(n^2+k^2)^{\frac{1}{n}}
$$

---

7.求曲线$f(x)$的弧长

$$
f(x) = \int_{-\sqrt{3}}^x\sqrt{3-t^2}dt
$$

---

8.设\(f(x)=\dfrac{1}{x + \sqrt{1 + x^{2}}}\)，其反函数记作\(f^{-1}(x)\)，求\(\int_{0}^{+\infty}f^{-1}(x)\mathrm{d}x\)

---


9.设\(t > 0\)，平面有界区域\(D\)由曲线\(y = \sqrt{x}e^{-x}\)与直线\(x = t\)，\(x = 2t\)及\(x\)轴围成，\(D\)绕\(x\)轴旋转一周所成旋转体的体积为\(V(t)\)，求\(V(t)\)的最大值。

---


10.设$(1+\sqrt{3})^n = a_n+\sqrt{3}b_n(a_n,b_n\in\mathbb{N}^+)$

(1)证明:$a_{n+1} = a_n+3b_n,b_{n+1} = a_n+b_n$

(2)求$\lim\limits_{n\to+\infty}\dfrac{a_n}{b_n}$


---



11.设函数\(f(x)\)在\([-a,a]\)上具有二阶连续导数，证明：

(1) 若\(f(0)=0\)，则存在\(\xi\in(-a,a)\)，使得\(f^{\prime\prime}(\xi)=\dfrac{1}{a^{2}}[f(a)+f(-a)]\)；

(2) 若\(f(x)\)在\((-a,a)\)内取得极值，则存在\(\eta\in(-a,a)\)使得
\(\left|f^{\prime\prime}(\eta)\right|\geqslant\dfrac{1}{2a^{2}}\left|f(a)-f(-a)\right|\)。


---


12.设函数\(f(x)\)具有二阶导数，且\(\vert f^{\prime\prime}(x)\vert\leq1\)

(1) 证明： 当\(x\in(0,1)\)时，\(\vert f(x)-f(0)(1 - x)-f(1)x\vert\leq\dfrac{x(1 - x)}{2}\)

(2) 证明：

$$\left\vert\int_{0}^{1}f(x)dx-\frac{f(0)+f(1)}{2}\right\vert\leq\frac{1}{12}$$

