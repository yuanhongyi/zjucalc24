# 积分不等式 总纲

## 构造积分上限函数

设$f(x)$在$[a,b]$上连续、递增，证明：

$$
\int_a^b xf(x)\mathrm{d}x \geq \dfrac{a+b}{2}\int_a^b f(x)\mathrm{d}x
$$


**证明：设辅助函数**

\[
F(t)=\int_{a}^{t}xf(x)\mathrm{d}x-\frac{a + t}{2}\int_{a}^{t}f(x)\mathrm{d}x
\]

显然\(F(a) = 0\)。对任意\(t\in[a,b]\)，有

$$
F^{\prime}(t)=tf(t)-\frac{1}{2}\int_{a}^{t}f(x)\mathrm{d}x-\frac{a + t}{2}f(t)\\
$$

$$
=\frac{t - a}{2}f(t)-\frac{1}{2}\int_{a}^{t}f(x)\mathrm{d}x\\
$$

$$
=\frac{1}{2}\int_{a}^{t}[f(t)-f(x)]\mathrm{d}x, \quad x\in[a,t]
$$

因为\(f(x)\)单调递增，则\(F^{\prime}(t)\geq0\)，则\(F(t)\)单调递增，所以\(F(b)\geq F(a) = 0(b\geq a)\)。因此

\[
\int_{a}^{b}xf(x)\mathrm{d}x\geq\frac{a + b}{2}\int_{a}^{b}f(x)\mathrm{d}x
\]

!!! Tip

    也可以用积分中值定理


## 利用Lagrange

设$f(x)$在$[0,a]$上一阶连续可导，且$f(0)=0$，$f'(x)\le M$，证明：

$$
\left|\int_0^af(x)\mathrm{d}x\right|\le \dfrac{M}{2}a^2
$$


**证明：**

$$
\left|\int_0^af(x)\mathrm{d}x\right|\le \int_0^a|f(x)|\mathrm{d}x = \int_0^a|f(x)-f(0)|\mathrm{d}x = \int_0^a|f'(\xi)x|\mathrm{d}x
$$

$$
\le M\int_0^a|x|\mathrm{d}x = \dfrac{M}{2}a^2
$$

!!! Tip

    本题用Lagrange中值定理来联系函数值和导数值


## 利用分部积分

设$f(x)$在$[0,a]$上一阶连续可导，且$f(0)=0$，$f'(x)\le M$，证明：

$$
\left|\int_0^af(x)\mathrm{d}x\right|\le \dfrac{M}{2}a^2
$$

**证明：**

$$
\int_0^af(x)\mathrm{d}x = \int_0^af(x)\mathrm{d}(x-a) = \int_0^a(a-x)f'(x)\mathrm{d}x
$$

$$
\left|\int_0^af(x)\mathrm{d}x\right| = \left|\int_0^a(a-x)f'(x)\mathrm{d}x\right| \le \int_0^a(a-x)|f'(x)|\mathrm{d}x \le \dfrac{M}{2}a^2
$$

!!! Tip

    本题用分部积分来联系函数值和导数值
    增加常数让分部积分第一项等于0也是在定积分有关题目中经常使用的技巧


设\(f\)在\([0,1]\)有二阶连续导数，\(\vert f^{\prime\prime}(x)\vert\leqslant1\)，\(\forall x\in[0,1]\)。证明:

$$
\left|\int_{0}^{1}f(x)\mathrm{d}x-\frac{f(0)+f(1)}{2}\right|\leqslant\frac{1}{24}
$$

**我们注意到：**

\[
\left|\int_{0}^{1}f(x)\mathrm{d}x-\frac{f(0)+f(1)}{2}\right|=\left|\int_{0}^{1}f(x)d\left(x-\frac{1}{2}\right)-\frac{f(0)+f(1)}{2}\right|
\]

\[
=\left|\int_{0}^{1}\left(x-\frac{1}{2}\right)f^{\prime}(x)\mathrm{d}x\right|
\]

\[
=\frac{1}{2}\left|\int_{0}^{1}f^{\prime}(x)d\left(x-\frac{1}{2}\right)^{2}\right|
\]

\[
=\frac{1}{2}\left|\int_{0}^{1}f^{\prime\prime}(x)\left(x-\frac{1}{2}\right)^{2}\mathrm{d}x\right|
\]

\[
\leqslant\frac{1}{2}\int_{0}^{1}\left(x-\frac{1}{2}\right)^{2}\mathrm{d}x=\frac{1}{24}
\]

---

设 $f$ 在 $[0,1]$ 有一阶导数且$|f'(x) - f'(y)| \leq |x - y|$，证明：

\[
\left|\int_{0}^{1} f(x)\mathrm{d}x - \frac{f(0) + f(1)}{2}\right| \leq \frac{1}{12}.
\]


**证明：**

\[
\left|\int_{0}^{1} f(x)\mathrm{d}x - \frac{f(0) + f(1)}{2}\right| = \left|\int_{0}^{1} \left(x - \frac{1}{2}\right) f'(x)\mathrm{d}x\right|
\]

\[
= \left|\int_{0}^{1} \left(x - \frac{1}{2}\right) \left[f'(x) - f'\left(\frac{1}{2}\right)\right] \mathrm{d}x\right|
\]

\[
\leq \int_{0}^{1} \left|x - \frac{1}{2}\right|^2 \mathrm{d}x = \frac{1}{12}.
\]

## 利用Taylor展开式

设$f(x)$在$[0,1]$上二阶可导，$f''(x)\lt 0$，证明:

$$
\int_0^1f(x^2)\mathrm{d}x\le f(\dfrac{1}{3})
$$

**证明**

由泰勒公式，得

\[
f(t)=f\left(\frac{1}{3}\right)+f'\left(\frac{1}{3}\right)\left(t - \frac{1}{3}\right)+\frac{f''(\xi)}{2!}\left(t - \frac{1}{3}\right)^2
\]

其中\(\xi\)介于\(\dfrac{1}{3}\)与\(t\)之间，从而

\[
f(x^2)\leq f\left(\frac{1}{3}\right)+f'\left(\frac{1}{3}\right)\left(x^2 - \frac{1}{3}\right)
\]

积分得

\[
\int_{0}^{1}f(x^2)\mathrm{d}x\leq f\left(\frac{1}{3}\right)
\]

---

设$f(x)$在$[a,b]$连续可导，$f(a) = f(b) = 0,f'(x)\le M$，证明:

$$
\int_a^bf(x)\mathrm{d}x\le \dfrac{M}{4}(b-a)^2
$$

**证明**

$$
\text{ 令 } F(x)=\int_{a}^{x}f(t)\mathrm{d}t, \quad F^{\prime}(a)=F^{\prime}(b)=0, \quad F(a)=0, \quad F(b)=\int_{a}^{b}f(x)\mathrm{d}x.
$$

$$
F\left(\frac{a + b}{2}\right)=F(a)+F^{\prime}(a)\left(\frac{a + b}{2}-a\right)+\frac{F^{\prime \prime}(\xi_{1})}{2!}\left(\frac{a + b}{2}-a\right)^{2}
$$

$$
F\left(\frac{a + b}{2}\right)=F(b)+F^{\prime}(b)\left(\frac{a + b}{2}-b\right)+\frac{F^{\prime \prime}(\xi_{2})}{2!}\left(\frac{a + b}{2}-b\right)^{2}
$$

$$
\Rightarrow 0=\int_{a}^{b}f(x)\mathrm{d}x+\frac{(b - a)^{2}}{8}\left[F^{\prime \prime}(\xi_{2})-F^{\prime \prime}(\xi_{1})\right]
$$

$$
\Rightarrow\left|\int_{a}^{b}f(x)\mathrm{d}x\right|=\frac{(b - a)^{2}}{8}\left|F^{\prime \prime}(\xi_{2})-F^{\prime \prime}(\xi_{1})\right|\leq\frac{M}{4}(b - a)^{2} \text{. 证毕!}
$$

## 利用积分与求和统一

设$f'(x)$在$[0,1]$上连续，$|f'(x)|\le M$，证明：

$$
\left|\int_0^1f(x)\mathrm{d}x-\dfrac{1}{n}\sum_{k=1}^{n}f\left(\dfrac{k}{n}\right)\right|\le \dfrac{M}{2n}
$$

**证明：**

$$
\left|\int_{0}^{1} f(x)\mathrm{d}x - \frac{1}{n} \sum_{k = 1}^{n} f\left(\frac{k}{n}\right)\right| = \left|\sum_{i = 1}^{n} \int_{\frac{i - 1}{n}}^{\frac{i}{n}} f(x)\mathrm{d}x - \sum_{i = 1}^{n} \int_{\frac{i - 1}{n}}^{\frac{i}{n}} f\left(\frac{i}{n}\right)\mathrm{d}x\right|
$$

用Lagrange中值定理

$$
\le \sum_{i = 1}^{n} \int_{\frac{i - 1}{n}}^{\frac{i}{n}} \left|f(x) - f\left(\frac{i}{n}\right)\right|\le \sum_{i = 1}^{n} \int_{\frac{i - 1}{n}}^{\frac{i}{n}} M\left(\dfrac{i}{n}-x\right)\mathrm{d}x = \dfrac{M}{2n}
$$

!!! Tip
    把积分变成求和，把求和变成积分，统一以后用拉格朗日。


## Cauchy不等式

!!! Cauchy不等式

    设$f(x)、g(x)$在$[a,b]$上连续，我们有柯西不等式：

    $$
    \int_a^bf^2(x)\mathrm{d}x\int_a^bg^2(x)\mathrm{d}x\ge\left(\int_a^bf(x)g(x)\mathrm{d}x\right)^2
    $$

    证明: 方法很多，这里构造积分上限函数

    $$
    F(x)=\int_{a}^{x} f(t)\mathrm{d}t\cdot \int_{a}^{x} g(t)\mathrm{d}t - \left(\int_{a}^{x} f(t)g(t) \mathrm{d}t\right)^2, \quad F(a) = 0.
    $$

    $$
    \Rightarrow F^{\prime}(x)= f^2(x)\cdot \int_{a}^{x} g^2(t)\mathrm{d}t + \int_{a}^{x} f^2(t)\mathrm{d}t\cdot g^2(x) - 2\cdot \int_{a}^{x} f(t)g(t)\mathrm{d}t\cdot f(x)\cdot g(x)
    $$

    $$
    =\int_{a}^{x} \left(f^2(x)g^2(t)+f^2(t)g^2(x)-2f(t)g(t)f(x)g(x)\right) \mathrm{d}t=\int_{a}^{x} \left(f(x)g(t)-f(t)g(x)\right)^2 \mathrm{d}t \geq 0
    $$

    $$
    \Rightarrow F(x)  \geq F(a) = 0. 证毕！
    $$


设$f'(x)$在$[0,1]$连续，且$f(1)-f(0)=1$，证明：

$$
\int_0^1(f'(x))^2\mathrm{d}x\ge 1
$$

**证明：**

$$
\int_0^1(f'(x))^2\mathrm{d}x\int_0^1 1\mathrm{d}x\ge\left(\int_0^1f'(x)\mathrm{d}x\right)^2 = (f(1)-f(0))^2 = 1
$$