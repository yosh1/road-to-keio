# mathematics-studying
It is repository that I am studying mathematics . 

---

## MathJaxにおける数式を書くためのチートシート


### 数式の記述方法

コードブロックの言語指定に "math" を指定することでTeX記法を用いて数式を記述することができます。

> \`\`\`math
> e^{i\pi} = -1
> \`\`\`

```math
e^{i\pi} = -1
```

また、$$で囲むことで独立した段落として記述することもできます。

> \$\$ e^{i\theta} = \\cos\\theta + i\\sin\\theta \$\$

$$ e^{i\theta} = \cos\theta + i\sin\theta $$

その他にも数式を$で囲むことで埋め込み形式として記述できます

> \$ e^{\pi i}= -1 $はオイラーの等式として知られています

$ e^{\pi i}= -1 $はオイラーの等式として知られています

### 改行(\\\\)

数式の行末に\\\\(バックスラッシュ２つ)をつけることによって改行をすることができます。

### 四則演算

> \`\`\`math
> 1 + 2 = 3 \\\
> 2 - 3 = 5 \\\
> 3 \times 2 = 6 \\\
> 6 \div 3 = 2
> \`\`\`

```math
1 + 2 = 3 \\
2 - 3 = 5 \\
3 \times 2 = 6 \\
6 \div 3 = 2
```

### 分数
> \`\`\`math
\frac{1}{2} - \frac{1}{3} = \frac{1}{6} \\\
\frac{a+b}{2ab}
> \`\`\`

```math
\frac{1}{2} - \frac{1}{3} = \frac{1}{6} \\
\frac{a+b}{2ab}
```

### 上付き・下付き文字

#### 上付き文字
![ 2015-06-13 23.45.52.png](https://qiita-image-store.s3.amazonaws.com/0/18783/99ff010f-b0b3-d8ad-2130-d598420b9338.png " 2015-06-13 23.45.52.png")
> \`\`\`math
ax^2 + bx + c = 0 \\\
y = x^{\frac{1}{2}}
> \`\`\`

```math
ax^2 + bx + c = 0 \\
y = x^{\frac{1}{2}}
```

#### 下付き文字
![ 2015-06-13 23.46.03.png](https://qiita-image-store.s3.amazonaws.com/0/18783/78618862-1c61-000a-a46a-328d9f861b98.png " 2015-06-13 23.46.03.png")

> \`\`\`math
x_{n+1} = rx_n(1-x_n)
> \`\`\`

```math
x_{n+1} = rx_n(1-x_n)
```

### イコール(＝)を揃える
begin{align}とend{align}と&を用いることによってブロック内で改行前後の位置を揃える

> \`\`\`math
\begin{align}
f(x) &= x^2+3x+2 \\\
&= (x+1)(x+2)
\end{align}
> \`\`\`

```math
\begin{align}
f(x) &= x^2+3x+2 \\
&= (x+1)(x+2)
\end{align}
```


### 文字の間隔
#### 一般的なスペース
![ 2015-06-14 0.36.38.png](https://qiita-image-store.s3.amazonaws.com/0/18783/abe76a5f-f7ee-3576-81ae-4c920d9bf8a0.png " 2015-06-14 0.36.38.png")

> \`\`\`math
y \quad = ax \qquad + b
> \`\`\`

```math
y \quad = ax \qquad + b
```

### 調整可能なスペース
![ 2015-06-14 0.36.31.png](https://qiita-image-store.s3.amazonaws.com/0/18783/29e236b9-ddbd-f2f7-d432-c067f200e8d1.png " 2015-06-14 0.36.31.png")

> \`\`\`math
a \hspace{50pt} b \hspace{1cm} c
> \`\`\`

```math
a \hspace{50pt} b \hspace{1cm} c
```

#### 小さなスペース
![ 2015-06-14 0.35.55.png](https://qiita-image-store.s3.amazonaws.com/0/18783/2bcfcffb-e11e-7fc9-0f83-6692b494b396.png " 2015-06-14 0.35.55.png")
> \`\`\`math
a \! b \, c \: d \; e　\\\
a \!\! b \,\, c \:\: d \;\; e
> \`\`\`

```math
a \! b \, c \: d \; e　\\
a \!\! b \,\, c \:\: d \;\; e
```

### 括弧の大きさ
下に行くほど括弧が大きくなる
#### 左括弧

\bigl
\Bigl
\biggl
\Biggl

#### 右括弧
\bigr
\Bigr
\biggr
\Biggr

丸括弧()・角括弧[]・波括弧{}を使いたいときは、それぞれの括弧の後ろにつける

> \`\`\`math
a \Biggl(
b \biggl(
c \Bigl(
d \bigl(
e ( f + g )
\bigr)
\Bigr)
\biggr)
\Biggr)
> \`\`\`

```math
a \Biggl(
b \biggl(
c \Bigl(
d \bigl(
e ( f + g )
\bigr)
\Bigr)
\biggr)
\Biggr)
```

### 極限(lim)
![ 2015-06-14 0.27.25.png](https://qiita-image-store.s3.amazonaws.com/0/18783/89893342-e66f-d005-914c-a5b34e1480ea.png " 2015-06-14 0.27.25.png")

> \`\`\`math
\lim_{x \to \infty} f(x) \\\
\lim_{h \to 0} \frac{f(x+h)-f(x)}{h} \\\
\lim_{\substack{x \to \infty \\ y \to \infty}} f(x,y)
> \`\`\`

```math
\lim_{x \to \infty} f(x) \\
\lim_{h \to 0} \frac{f(x+h)-f(x)}{h} \\
\lim_{\substack{x \to \infty \\ y \to \infty}} f(x,y)
```

### 平方根(sqrt)
![ 2015-06-13 23.39.26.png](https://qiita-image-store.s3.amazonaws.com/0/18783/9c1eefeb-e11c-961f-5ae5-2b63f93cc721.png " 2015-06-13 23.39.26.png")

> \`\`\`math
\sqrt{a^2+b^2} \\\
\sqrt[3]{a}
> \`\`\`

```math
\sqrt{a^2+b^2} \\
\sqrt[3]{a}
```

### 三角関数(sin, cos, tan)
![ 2015-06-14 0.06.03.png](https://qiita-image-store.s3.amazonaws.com/0/18783/c3907e5a-625d-9261-ed4e-cd8b7fd7dc4e.png " 2015-06-14 0.06.03.png")

> \`\`\`math
\sin^2 x + \cos^2 x = 1
> \`\`\`

```math
\sin^2 x + \cos^2 x = 1
```

### 指数関数(e, exp)
![ 2015-06-14 0.04.49.png](https://qiita-image-store.s3.amazonaws.com/0/18783/4b8eab9f-cf4e-522e-12f5-6c1c2abc3e69.png " 2015-06-14 0.04.49.png")

> \`\`\`math
e^{i\pi} = -1 \\\
e^{i\theta} = \cos \theta + i \sin \theta
> \`\`\`

```math
e^{i\pi} = -1 \\
e^{i\theta} = \cos \theta + i \sin \theta
```


### 対数関数・自然対数(log, ln)
![ 2015-06-14 0.00.39.png](https://qiita-image-store.s3.amazonaws.com/0/18783/3c1356ff-7a1f-09b5-f1a0-4ec0935d51ce.png " 2015-06-14 0.00.39.png")
> \`\`\`math
\log_a \frac{x}{y} = \log_a x - \log_a y \\\
\ln \frac{x}{y}
> \`\`\`

```math
\log_a \frac{x}{y} = \log_a x - \log_a y \\
\ln \frac{x}{y}
```


### 積分・重積分・周回積分(∫)
#### 積分
![ 2015-06-13 23.52.30.png](https://qiita-image-store.s3.amazonaws.com/0/18783/88780272-47d4-779e-499e-4a9f559eb390.png " 2015-06-13 23.52.30.png")
> \`\`\`math
\int f(x)dx \\\
\int_{a}^{b}f(x)dx
> \`\`\`

```math
\int f(x)dx \\\
\int_{a}^{b}f(x)dx
```

#### 重積分
![ 2015-06-13 23.54.27.png](https://qiita-image-store.s3.amazonaws.com/0/18783/b30d0cf3-2bb5-8c25-2765-85331599ff30.png " 2015-06-13 23.54.27.png")
> \`\`\`math
\iint f(x,y)dxdy
> \`\`\`

```math
\iint f(x,y)dxdy
```

#### 周回積分
![ 2015-06-13 23.57.16.png](https://qiita-image-store.s3.amazonaws.com/0/18783/0fbd4f7d-cc29-4773-8898-596fffd2cbd6.png " 2015-06-13 23.57.16.png")

> \`\`\`math
\oint_C \frac{1}{z}dz
> \`\`\`

```math
\oint_C \frac{1}{z}dz
```

### 和・総和(シグマΣ)
![fix_sum.png](https://qiita-image-store.s3.amazonaws.com/0/18783/783c6c50-7a8e-dde3-9388-165758101119.png)

> \`\`\`math
\sum_{k=1}^{n} k = 1 + 2 + 3 + \cdots + n = \frac{n(n+1)}{2} \\\
\sum_{k=1}^{n} k^2 = 1^2 + 2^2 + 3^2 + \cdots + n^2 = \frac{n(n+1)(2n+1)}{6}
> \`\`\`

```math
\sum_{k=1}^{n} k = 1 + 2 + 3 + \cdots + n = \frac{n(n+1)}{2} \\
\sum_{k=1}^{n} k^2 = 1^2 + 2^2 + 3^2 + \cdots + n^2 = \frac{n(n+1)(2n+1)}{6}

```

### ギリシャ文字
![ 2015-06-14 0.42.37.png](https://qiita-image-store.s3.amazonaws.com/0/18783/be94d7d6-c958-ab64-39b4-4160eebe9a6b.png " 2015-06-14 0.42.37.png")

> \`\`\`math
i \hbar \frac{\partial \psi}{\partial t} = H \psi(x,t)
> \`\`\`

```math
i \hbar \frac{\partial \psi}{\partial t} = H \psi(x,t)
```


### 等号、不等号、演算子、集合
 ![figgg.png](https://qiita-image-store.s3.amazonaws.com/0/18783/68c764fa-e74c-66f6-8eeb-412937ef586a.png "figgg.png")

### 矢印記号
![figfig.png](https://qiita-image-store.s3.amazonaws.com/0/18783/92d370db-a049-24b2-bc78-754044ba8780.png)

> \`\`\`math
\begin{align}
\qquad &ax^2+bx+c = 0 \\\
\Leftrightarrow &\quad x^2 + \frac{b}{a}x = - \frac{c}{a} \\\
\Leftrightarrow &\quad x^2 + \frac{b}{2a} x + \frac{b^2}{4a^2} = \frac{b^2}{4a^2} - \frac{c}{a} \\\
\Leftrightarrow &\quad (x + \frac{b}{2a})^2 = \frac{b^2 - 4ac}{4a^2} \\\
\Leftrightarrow &\quad x + \frac{b}{2a} = \pm \frac{\sqrt{b^2-4ac}}{2a} \\\
\therefore &x = \frac{-b \pm \sqrt{b^2-4ac} }{2a}
\end{align}
> \`\`\`

```math
\begin{align}
\qquad &ax^2+bx+c = 0 \\
\Leftrightarrow &\quad x^2 + \frac{b}{a}x = - \frac{c}{a} \\
\Leftrightarrow &\quad x^2 + \frac{b}{2a} x + \frac{b^2}{4a^2} = \frac{b^2}{4a^2} - \frac{c}{a} \\
\Leftrightarrow &\quad (x + \frac{b}{2a})^2 = \frac{b^2 - 4ac}{4a^2} \\
\Leftrightarrow &\quad x + \frac{b}{2a} = \pm \frac{\sqrt{b^2-4ac}}{2a} \\
\therefore &x = \frac{-b \pm \sqrt{b^2-4ac} }{2a}
\end{align}
```


### アクセント記号(ベクトルなど)

![ 2015-06-14 20.51.24.png](https://qiita-image-store.s3.amazonaws.com/0/18783/b20cba33-bd92-05d0-d694-21f5556c05c3.png " 2015-06-14 20.51.24.png")

> \`\`\`math
\vec{A} = \vec{B} + \vec{C} \\\
F = m\ddot{x}
> \`\`\`

```math
\vec{A} = \vec{B} + \vec{C} \\
F = m\ddot{x}
```

### ドット(3点リーダー)

> \`\`\`math
> \left(
> \begin{array}{ccccc}
> a_{11} & \cdots & a_{1i} & \cdots & a_{1n}\\
> \vdots & \ddots &        &        & \vdots \\
> a_{i1} &        & a_{ii} &        & a_{in} \\
> \vdots &        &        & \ddots & \vdots \\
> a_{n1} & \cdots & a_{ni} & \cdots & a_{nn}
> \end{array}
> \right)![fix_sum.png](https://qiita-image-store.s3.amazonaws.com/0/18783/225d2e65-e9f0-b60e-97cd-a14f7c8ce21a.png)


> \`\`\`

```math

\left(
\begin{array}{ccccc}
a_{11} & \cdots & a_{1i} & \cdots & a_{1n}\\
\vdots & \ddots &        &        & \vdots \\
a_{i1} &        & a_{ii} &        & a_{in} \\
\vdots &        &        & \ddots & \vdots \\
a_{n1} & \cdots & a_{ni} & \cdots & a_{nn}
\end{array}
\right)
```

### 行列と行列式
> \`\`\`math
\begin{matrix}
a & b \\\
c & d 
\end{matrix}
> \`\`\`

```math
\begin{pmatrix}
a & b \\
c & d 
\end{pmatrix}
```
> \`\`\`math
\begin{pmatrix}
a & b \\\
c & d 
\end{pmatrix}

> \`\`\`

```math
\begin{bmatrix}
a & b \\
c & d 
\end{bmatrix}
```
> \`\`\`math
\begin{bmatrix}
a & b \\\
c & d 
\end{bmatrix}
> \`\`\`

```math
\begin{vmatrix}
a & b \\
c & d 
\end{vmatrix}
```
> \`\`\`math
\begin{vmatrix}
a & b \\\
c & d 
\end{vmatrix}
> \`\`\`

```math
\begin{Vmatrix}
a & b \\
c & d 
\end{Vmatrix}
```

> \`\`\`math
\begin{pmatrix}
a & b \\\
c & d 
\end{pmatrix}
> \`\`\`

```math
\begin{pmatrix}
a & b \\
c & d 
\end{pmatrix}

\times

\begin{vmatrix}
e & f \\
g & h 
\end{vmatrix}
```

### 場合分け

> \`\`\`math
f(x) = \left\\{
\begin{array}{ll}
1 & (x \geq 0) \\\
0 & (x \lt 0)
\end{array}
\right.
> \`\`\`

```math
f(x) = \left\{
\begin{array}{ll}
1 & (x \geq 0)\\
0 & (x \lt 0)
\end{array}
\right.
```

## 参考記事
http://medemanabu.net/latex/latex-commands-list/

