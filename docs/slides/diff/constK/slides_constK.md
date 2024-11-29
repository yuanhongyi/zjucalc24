# 中值定理10

## 常数K值法

### 简要介绍

涉及中值定理的题，往往需要构造辅助函数，然而有一些辅助函数的构造又令人费解。常数K值法是适用于一类中值定理题目的构造方法，通过将中值变元之外的常数部分设为k，然后再利用**主元法或对称式**和**罗尔定理**就可以完成证明。

### 例题

#### 例1

$设f(x)为[a,b]上的可导函数，求证：\exists\varepsilon\in (a,b)满足：$

$$
f(b) - f(a) = f'(\varepsilon)(b-a)
$$

$证明1: 设k = \dfrac{f(b)-f(a)}{b-a} .........①，\iff 证明f'(\varepsilon) = k$
$由①得：f(b) - f(a) - k(b-a) =0$

$设F(x) = f(x) - f(a) - k(x - a)......(\textbf{主元法})$
$则F(b) = F(a) = 0$

$由罗尔定理: \exists\varepsilon\in(a,b)，F'(\varepsilon) = 0\iff f'(\varepsilon) = k$

!!! Tip
    使用主元法，往往观察到变量的对称性，而且有一个天然条件$F(a) = 0$

<br>

$证明2: 设k = \dfrac{f(b)-f(a)}{b-a} .........①，\iff 证明f'(\varepsilon) = k$
$由①得：f(b) - kb = f(a) - ka......(\textbf{对称式})$

$设F(x) = f(x) - kx \Rightarrow F(a) = F(b)$

$由罗尔定理: \exists\varepsilon\in(a,b)，F'(\varepsilon) = 0\iff f'(\varepsilon) = k$

!!! Tip
    构造对称式，有点像高中学的"同构"


#### 例2

$b>a>0，设f(x)为[a,b]上的可导函数，求证：\exists\varepsilon\in (a,b)满足：$

$$
\dfrac{bf(a)-af(b)}{b-a} = f(\varepsilon) - \varepsilon f'(\varepsilon)
$$


$设\dfrac{bf(a)-af(b)}{b-a} = k\Rightarrow bf(a) - af(b) = k(b-a)$


$同时除以ab\Rightarrow \dfrac{f(a)}{a} - \dfrac{k}{a} = \dfrac{f(b)}{b} - \dfrac{k}{b}$

$设F(x) = \dfrac{f(x)}{x} - \dfrac{k}{x} \Rightarrow F(a) = F(b)$
$\exists\varepsilon\in (a,b), F'(\varepsilon) = 0$

$F'(x) = \dfrac{xf'(x) - f(x)+k}{x^2}  \Rightarrow k = f(\varepsilon) - \varepsilon f(\varepsilon)$​

#### 练习

请用主元法完成例2

!!! Answer
    $\dfrac{bf(a) - af(b)}{b - a} = k$

    $bf(a) - af(b) = k(b - a)$

    $(1) \text{ 若令 } F(x) = [xf(a) - af(x)] - k(x - a)$

    $F(a) = 0 \quad F(b) = 0$

    $F'(x) = f(a) - af'(x) - k$

    $f(a) - af'(\varepsilon) = k$

    $\text{应该要证明 } k = f(\varepsilon) - \varepsilon f'(\varepsilon)$
    $\text{所以证明失败}$

    $xf(a) - af(x) = k(x - a)$

    $\text{求导以后要清去} f(a) \text{，所以要进行变形}$

    $\dfrac{f(a)}{a} - \dfrac{f(x)}{x} = \dfrac{k(x - a)}{ax}$

    $\text{令 } F(x) = \dfrac{f(a)}{a} - \dfrac{f(x)}{x} - k\left(\dfrac{1}{a} - \dfrac{1}{x}\right)$

    $F(a) = 0 \quad F(b) = 0$

    $f'(\varepsilon) = -\dfrac{\varepsilon f(\varepsilon) + f'(\varepsilon)}{\varepsilon^2} - \dfrac{k^2}{\varepsilon^2} = 0$



#### 练习

$b>a>0，设f(x)为[a,b]上的可导函数，求证\exists\varepsilon\in (a,b)\ s.t.$

$$
\dfrac{f(b) - f(a)}{b-a} = \dfrac{\varepsilon^2 f'(\varepsilon)}{ab}
$$

!!! Answer
    $设k = \dfrac{ab[f(b) - f(a)]}{b-a}$

    $则f(b) - f(a) = \dfrac{k(b-a)}{ab} = \dfrac{k}{a} - \dfrac{k}{b}\Rightarrow f(b)+\dfrac{k}{b} = f(a)+\dfrac{k}{a}$

    $设F(x) = f(x)+\dfrac{k}{x}\Rightarrow F(a) = F(b)\Rightarrow$
    $\exists\varepsilon\ s.t.\ F'(\varepsilon) = 0 \Rightarrow f'(\varepsilon) - \dfrac{k}{\varepsilon^2} = 0\Rightarrow k = \varepsilon^2f'(\varepsilon)$

#### 例3

$已知a<b<c, f(x)二阶可导，证明\exists\xi\in(a,b)，使$

$$
\dfrac{1}{2}f''(\xi) = \dfrac{f(a)}{(a-c)(a-b)}+\dfrac{f(b)}{(b-c)(b-a)}+\dfrac{f(c)}{(c-b)(c-a)}
$$

$设k = \dfrac{f(a)}{(a-c)(a-b)}+\dfrac{f(b)}{(b-c)(b-a)}+\dfrac{f(c)}{(c-b)(c-a)}$

$同乘(a-b)(b-c)(c-a)\Rightarrow f(a)(c-b)+f(b)(a-c)+f(c)(b-a) = k(a-b)(b-c)(c-a)$

$\textbf{以a为主元}$
$设F(x) = f(x)(c-b)+f(b)(x-c)+f(c)(b-x) - k(x-b)(b-c)(c-x)$
$F(a) = F(b) = F(c) = 0$

$由罗尔定理\exists m_1\in(a,b),m_2\in(b,c), F'(m_1) = F'(m_2) = 0$

$由罗尔定理\exists\xi\in(m_1,m_2),F''(\xi) = 0$​

$F''(x) = (c-b)f''(x) - (c-b)2k \Rightarrow f''(\xi) = 2k$

#### 例4

$设f在[a,b]上二阶可导，f(a) = f(b) = 0 求证：对于某个x\in(a,b)，存在\xi\in(a,b)，使得：$

$$
f(x) = \dfrac{f''(\xi)}{2}(x-a)(x-b)
$$

$设k = \dfrac{f(x)}{(x-a)(x-b)}(把x当作某个固定值c)$
$令F(t) = f(t) - k(t-a)(t-b)$

$F(a) = F(x) = F(b) = 0\Rightarrow \exists m_1\in(a,x),m_2\in(x,b)\ s.t.F'(m_1) = F'(m_2) = 0$

$\therefore\exists\xi\in(a,b) \Rightarrow F''(\xi) = 0即f''(\xi) = 2k$

#### 练习

设\(a_1 < a_2 < \cdots < a_n\)为\(n\)个不同的实数，\(f(x)\)在\([a_1, a_n]\)上有\(n\)阶导数，且
\(f(a_1) = f(a_2) = \cdots = f(a_n) = 0\)。求证：对\(\forall c \in [a_1, a_n]\)，\(\exists \xi \in (a_1, a_n)\)使得

$$
\frac{f(c)}{(c - a_1)(c - a_2)\cdots(c - a_n)} = \frac{f^{(n)}(\xi)}{n!}
$$

!!! Answer
    (1) 若\(c = a_k (k = 1,2,\cdots,n)\)，则\(f(c) = 0\)；从而，对\(\forall \xi \in (a_1, a_n)\)结论均成立。

    (2) 若\(c \neq a_k\) (对\(\forall k = 1,2,\cdots,n\))，记\(\dfrac{f(c)}{(c - a_1)(c - a_2)\cdots(c - a_n)} = k\)。

    令\(F(x) = f(x) - k(x - a_1)(x - a_2)\cdots(x - a_n)\)，则：\(F(x)\)在\([a_1, a_n]\)上有\(n\)阶导数

    且\(F(a_1) = F(a_2) = \cdots = F(a_n) = 0\)，\(F(c) = 0\)，即\(F(x)\)在\([a_1, a_n]\)有\((n + 1)\)个零点。

    由Rolle定理，\(\exists \xi \in (a_1, a_n)\)使得\(F^{(n)}(\xi) = 0\)；而\(F^{(n)}(x) = f^{(n)}(x) - n!k\)。

    因此，\(\exists \xi \in (a_1, a_n)\)使得\(f(c) = \dfrac{(c - a_1)(c - a_2)\cdots(c - a_n)}{n!}f^{(n)}(\xi)\)。



!!! Summary
    常数k值法通过把一大堆常数设成k，不仅简化了题面，还对构造函数有着辅助作用。构造函数需要观察函数的对称性质。
