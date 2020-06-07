# 编程数学知识

## 1. 集合

集合是一种数学概念。就像一个瓶子，里头装有一些数学上定义的元素。

- 例如，一个班上所有的学生可以构成一个集合，一个框里所有的鸡蛋也可以构成一个集合。
- 例如 ，$\{1,2,3,4\}$ 就是一个集合，里头装了4个数。
- 例如，所有的正整数构成一个集合，里头装了所有的正整数（集合里头的元素数目可以是无限个），常用$N^+$表示。
- 例如，所有的自然数构成一个集合，里头装了0到无穷大（正无穷大用 $+\infty$表示，负无穷大用 $-\infty$表示）的所有的整数，常用$N$ 来表示。
- 例如，所有的整数构成一个集合，里头装了从$-\infty$到 $+\infty$的所有整数，常用$Z$来表示。
- 例如，所有的整数，加上所有的有限或者循环的小数，构成一个集合，叫做有理数集合，常用$Q$ 来表示。
- 例如，所有的有理数，加上所有的无线不循环小数(例如$\sqrt{2}$ , $\pi$ 等)，构成一个集合，叫做实数，常用$R$ 来表示。

## 2.  函数

函数是一种映射，自变量 $ x$ 以一种方式对应到一个应变量 $y$ 。这种对应方式，通常用一个字母 $f$ 表示，例如 $y=f(x)$。能够写成 $y=f(x)$ 的函数，成为显式函数。不容易写成显式的函数，只能写成 $f(x,y)=0$ 的函数，成为隐式函数。根据$ x$ 和 $y$ 的对应关系，可以分成3三种情况。

![映射](.\figure\映射.svg)

- 一个$ x$ 对应一个 $y$ (例如 $y=2x+1$)，这种函数研究得最多。

- 多个$ x$ 对应一个 $y$ 的 (例如 $ y= x^2$ 就是两个$ x$对应一个$y$，$ x=1$ 和 $x=-1$ 时，都是 $y=1$)。

- 一个$x$ 对应多个 $y$ (例如 $x^2+y^2=1$，这种类似的隐函数，当$x=0$ 时，有 $y=1$ 和 $y=-1$ 两种情况)，这种函数在几何曲线、曲面的代数表示中非常多。

函数中常用 $x,y,z$ 表示自变量或者因变量。用$a,b,c$等表示系数或者要求解的参数。

### 2.1. 一次函数

$$
\begin{cases} 
y=a \cdot x +b \\ a \neq 0
\end{cases}\tag{2.1}
$$

### 2.2. 二次函数

$$
\begin{cases} 
y=a \cdot x^2 +b \cdot x + c \\ a \neq 0
\end{cases}\tag{2.2}
$$

### 2.3. $n$ 次多项式函数
$$
\begin{cases} 
   y=a_{n} \cdot x^n +a_{n-1} \cdot x^{n-1} +a_{n-2} \cdot x^{n-2} + \ldots + a_{1} \cdot x + a_{0} \\
   a_{n} \neq 0
   \end{cases}\tag{2.3}
$$

其中，
$$
x^0 = 1 \quad \mbox{for} \quad x \neq 0 \tag{2.4}
$$

### 2.4. 反比例函数

$$
\begin{cases} 
   y= \frac{a \cdot x +b}{c \cdot x+d} \\
   c \neq 0 \\
   c \cdot x+d \neq 0
   \end{cases}\tag{2.5}
$$

### 2.5. 分式函数

用的较少，一般用反比例函数。
$$
\begin{cases} 
   y=\frac{a_{n} \cdot x^n +a_{n-1} \cdot x^{n-1} +a_{n-2} \cdot x^{n-2} + \ldots + a_{1} \cdot x + a_{0}}{b_{n} \cdot x^n +b_{n-1} \cdot x^{n-1} +b_{n-2} \cdot x^{n-2} + \ldots + b_{1} \cdot x + b_{0}} \\
   b_{n} \neq 0 \\
   b_{n} \cdot x^n +b_{n-1} \cdot x^{n-1} +b_{n-2} \cdot x^{n-2} + \ldots + b_{1} \cdot x + b_{0} \neq 0
   \end{cases}\tag{2.6}
$$

### 2.6. 三角函数
![三角函数](.\figure\三角函数.svg)

根据上图单位圆上几个要素和勾股定理 $a^2+b^2=r^2 $ 定义。
$$
\sin(\theta) = \frac{a}{r} \\
      \cos(\theta) = \frac{b}{r} \\ 
      \tan(\theta) = \frac{a}{b} = \frac{\sin(\theta)}{\cos(\theta)} \\\tag{2.7}
      \cot(\theta) = \frac{b}{a} = \frac{\cos(\theta)}{\sin(\theta)} \\
$$

三角形相关的定理：

- 三角形边长规律：任意两边之和大于第三边（两点之间，直线最短）
$$
\begin{cases} 
AB+BC>AC \\
BC+CA>AB\\
CA+AB>BC
\end{cases}
$$

- 正弦定理
$$
\frac{\sin{\alpha}}{BC}=\frac{\sin{\beta}}{AC}=\frac{\sin{\gamma}}{AB} \tag{2.8}
$$

- 余弦定理
$$
\begin{cases} 
\cos{\alpha}=\frac{AB^2+AC^2-BC^2}{2AB \cdot AC}  \Longleftrightarrow BC^2 =AB^2+AC^2-2AB \cdot AC \cdot \cos{\alpha} \\
\cos{\beta}=\frac{AB^2+BC^2-AC^2}{2AB \cdot BC}  \Longleftrightarrow AC^2 =AB^2+BC^2-2AB \cdot BC \cdot \cos{\beta}  \\
\cos{\gamma}=\frac{AC^2+BC^2-AB^2}{2AC \cdot BC}  \Longleftrightarrow AB^2 =AC^2+BC^2-2AC \cdot BC \cdot \cos{\gamma}
\end{cases} \tag{2.9}
$$

说道单位圆和三角函数，就避免不了一个概念: 弧度。

我们已经知道的角度表示，例如 90°是直角，一个圆周是360°。弧度的概念和单位元上的弧长是相关的。

数学上定义1 rad为一个弧度，在单位圆上，1 rad 的角度对应的扇形的弧长和半径相等。圆的周长是 $2\pi r$，所以一个圆周360度，对应的弧度是 $2\pi$。

90°对应的弧度是 $\pi/2$。

### 2.7. 指数函数
$$
\begin{cases} 
y=a^x \\
a \neq 0
\end{cases} \tag{2.10}
$$
上式中，$a$ 为底数，$x$ 为指数， $y$ 为幂。
      
### 2.8. 对数函数

$$
\begin{cases} 
y=\log_a^x \\
a > 0 \\
x > 0
\end{cases} 
\Longleftrightarrow x=a^y \tag{2.11}
$$
上式中，$a$ 为底数，$x$ 为真数，$y$ 为对数。对数函数一般只讨论底数 $a>0$  的情况，此时真数 $x$ 必须大于0.
当 $a=e \approx 2.71828$ 时，即对数函数的底数为$e$ 时，对数函数有个特殊的表示方法。
$$
\begin{cases} 
y=\log_e^x=\ln{x} \\
x > 0
\end{cases}
\Longleftrightarrow x=e^y \tag{2.12}
$$

## 3. 向量

向量是一种有方向的量，例如位移（有往东、南、西、北的方向）、速度（不同方向的速度导致的位移效果不一样）、力（不同方向的力会使物体向不同的方向运动）。向量的分析通常有几何方法和代数方法。向量分析中，向量具有平移不变性，即向量关注的是起点和终点之间的差量，而起点在哪里，不在考虑之内。向量的两个最基本的属性，就是方向和模长(向量的长度)。

### 3.1. 向量几何分析法

向量的几何分析法，一般就是利用垂直，平行四边形法则（三角形法则），用图形的方法，分析向量的图形关系。

#### 3.1.1. 向量加法合成

![向量几何加法](.\figure\向量几何加法.svg)

上图中，按照向量加法的三角形法则，$\vec{AB}+\vec{BC}=\vec{AC}$ ，从图形的角度来说，就是两个向量$\vec{AB}，\vec{BC}$ ，前者$\vec{AB}$ 的终点$B$ ，和后者$\vec{BC}$的起点$B$ 在同一位置时，向量的加法的结果就是由前者$\vec{AB}$ 的起点$A$ ，指向后者$\vec{BC}$的终点$C$，即向量$\vec{AC}$，整体上像一个首尾串。图像上看起来像一个三角形。

上图中，按照向量加法的平行四边形原则，就是将 $\vec{BC}$ 平移到 $\vec{AB'}$ ，由于 $\vec{BC}$ 和 $\vec{AB'}$ 是直接平移的，是相同的向量，即平行且相等，所以四边形 $ABCB'$ 是平行四边形。那么$\vec{AB}+\vec{BC}=\vec{AB}+\vec{AB'}=\vec{AC}$ ，相当于用两个向量，通过平移构成平行四边形。这两个向量加法的结果是，从四边形中两个向量共同的起点$A$ 出发的一条对角线  $\vec{AC}$。

#### 3.1.2. 向量分解

向量的分解其实是向量加法的一个逆过程。通常使用平行四边形法则，将一个向量分解到两个已知的方向上。向量的减法，可以将其中那个符号为负的向量反向，变成向量的加法。

![向量几何分解](.\figure\向量几何分解.svg)

上图中，知道一个要分解的向量 $\vec{AC}$ ，和要分解的两个方向，方向1和方向2，那么分解的过程就是过向量 $\vec{AC}$ 的终点$C$作方向1和方向2的平行线，最终会形成一个平行四边形，那么$\vec{AC}$ 就被分解成了$\vec{AB}$ 和 $\vec{AD}$，且满足 $\vec{AC} = \vec{AB}+\vec{AD}$。向量的分解结果之与向量$\vec{AC}$，分解方向1和方向2有关。随着方向1和方向2的不同，向量$\vec{AC}$ 就有对应的不同的分解结果。最常见的分解方向为方向1和方向2相互垂直。

### 3.2. 向量的数乘

向量的数乘，是向量最简单的一个操作，就是将一个向量乘以一个实数$a$，向量数乘的结果是模长为原向量的$a$ 倍，方向不变。$a$ 是正数时，结果向量和原向量同向；$a$ 是复数是，结果向量和原向量反向。$a>0$时，$a\vec{AB}$ 和$\vec{AB}$ 的方向相同，前者的模长是后者的$a$ 倍；$a<0$时，$a\vec{AB}$ 和$\vec{AB}$ 的方向相反，前者的模长是后者的 $\rvert{a}\lvert$ 倍。

### 3.3. 向量代数分析法

向量的代数分析法，一般就是建立一个直角坐标系，根据在坐标系中的向量的起点和终点，构建一个由起点指向终点的向量。在以该坐标轴为基向量方向的情况下，该向量的坐标表示就是用终点坐标减去起点坐标。

在直角坐标系中表示向量，一般会将与坐标轴同方向的几个向量定义成基向量，例如 $\vec{e_1}$ 表示方向和$ x$ 轴正方向同向的单位向量；$\vec{e_2}$ 表示方向和$ y$ 轴正方向同向的单位向量；$\vec{e_3}$ 表示方向和$ z$ 轴正方向同向的向量。这3个基向量，$\vec{e_1},\vec{e_2},\vec{e_3}$ 就是向量分解时的分解方向。

单位向量的长度是1，方向可以由用户定义。
$$
\begin{cases} 
\lvert \vec{e_1}\rvert =1 \\
\lvert \vec{e_2}\rvert =1 \\
\lvert \vec{e_3}\rvert =1 
\end{cases}\tag{3.1}
$$
向量的常见分解，是将一个向量分解到直角坐标系的几个坐标轴上去，操作方法就是投影。

#### 3.3.1. 向量分解

![向量代数分解](.\figure\向量代数分解.svg)

如上图的左边子图，例如一个向量$\vec{OA}$ 在二维坐标系 $xoy$ 中沿着两个坐标轴分解。$\vec{ox}$方向的定义为基向量 $\vec{e_1}$ ，$\vec{oy}$方向的定义为基向量 $\vec{e_2}$ ，将$\vec{OA}$ 沿着 $\vec{ox}$ 和$\vec{oy}$ 的方向分解，按照几何分解方法的结论，以 $\vec{ox}$ 和$\vec{oy}$ 为边，$\vec{OA}$ 为对角线，做出一个平行四边形，就可以得到分解结果向量$\vec{OB}$ 和 $\vec{OC}$ 。当坐标系 $xoy$ 为直角坐标系时，分解$\vec{OA}$时作的平行四边形就更简单，就是往 $\vec{ox}$ 和$\vec{oy}$ 坐标轴做垂线，即投影。
$$
\begin{cases} 
\vec{OA} = \vec{OB} + \vec{OC} \\
\vec{OB} = b\cdot \vec{e_2}\\
\vec{OC} = a\cdot \vec{e_1}
\end{cases}  \Longleftrightarrow \vec{OA}=a\cdot \vec{e_1} + b\cdot \vec{e_2} \tag{3.2}
$$
当选定了两个要分解到的两个基向量$\vec{e_1},\vec{e_2}$ 方向，就可用上面的分解方法，得到类似于 $\vec{OA}=a\cdot \vec{e_1} + b\cdot \vec{e_2}$ 的向量表示。另外一种更简单的坐标表示即 $(a, b)$ ，配合两个基$\vec{e_1},\vec{e_2}$。在一套选定的基$\vec{e_1},\vec{e_2}$ 的情况下，所有的向量都用坐标表示。有了坐标，向量就可以用坐标分量乘以对应的基向量，然后加起来，得到最终的向量。

如上图的右边子图，例如一个向量$\vec{OA}$ 在三维坐标系 $oxyz$中沿着三个坐标轴分解，几何方法稍微麻烦些。但是在直角坐标系中。向量分解到三个坐标轴方向上，按照上述二维直角坐标系中的规律，将$\vec{OA}$ 往三个坐标轴上投影，在 $\vec{ox}$ ，$\vec{oy}$， $\vec{oz}$ 投影得到的长度分别为 $a,b,c$ ，则$\vec{OA} = a \cdot \vec{e_1} + b \cdot \vec{e_2}+c \cdot \vec{e_3}$，则$\vec{OA}$ 的在基$\vec{e_1},\vec{e_2},\vec{e_3}$下， 坐标表示为$(a,b,c)$。

#### 3.3.2. 向量加法合成 

有了向量代数分析法中的向量分解，将向量先分解为目标坐标系中的坐标，然后根据向量的加法，合并相同基的项，直接得到加法合成后的向量坐标。

![向量代数加法](.\figure\向量代数加法.svg)
$$
\begin{cases}

\begin{cases} 
\vec{OA_1} = \vec{OB_1} + \vec{OC_1} \\
\vec{OB_1} = b_1\cdot \vec{e_2}\\
\vec{OC_1} = a_1\cdot \vec{e_1}
\end{cases}  \Longleftrightarrow \vec{OA_1}=a_1\cdot \vec{e_1} + b_1\cdot \vec{e_2} \\
\\

\begin{cases} 
\vec{OA_2} = \vec{OB_2} + \vec{OC_2} \\
\vec{OB_2} = b_2\cdot \vec{e_2}\\
\vec{OC_2} = a_2\cdot \vec{e_1}
\end{cases}  \Longleftrightarrow \vec{OA_2}=a_2\cdot \vec{e_2} + b_2\cdot \vec{e_2}
\end{cases} \Longleftrightarrow 

\begin{cases} 
\vec{OA} = \vec{OA_1} +\vec{OA_2} &= a_1\cdot \vec{e_1} + b_1\cdot \vec{e_2} + a_2\cdot \vec{e_1} + b_2\cdot \vec{e_2} \\ & = (a_1+a_2)\cdot \vec{e_1} + (b_1+b_2)\cdot \vec{e_2}
\end{cases} \tag{3.3}
$$
所以 $\vec{OA_1}，\vec{OA_2}$ 的加法的代数分析方法为：

- 得到$\vec{OA_1}，\vec{OA_2}$的在基$\vec{e_1},\vec{e_2}$下的坐标表示$(a_1,b_1)$，$(a_2,b_2)$。

- 将$\vec{OA_1}，\vec{OA_2}$的坐标对应的分量加起来，得到向量加法结果向量$\vec{OA}$的坐标 $(a_1+a_2,b_1+b_2)$。

- 根据结果坐标和坐标所在的基对应相乘，得到结果向量 $\vec{OA}=(a_1+a_2)\cdot \vec{e_1} + (b_1+b_2)\cdot \vec{e_2}$。

- 非要得到向量的几何表示，可以根据$(a_1+a_2)\cdot \vec{e_1}$ 和 $(b_1+b_2)\cdot \vec{e_2}$ 构成平行四边形，根据平行四边形原则，得到结果向量$\vec{OA}$。

比较根据$\vec{OA_1}，\vec{OA_2}$ 直接构成平行四边形，通过几何分析法，得到$\vec{OA_1}，\vec{OA_2}$ 相加的结果$\vec{OA}$。这和上面代数分析法结果是一样的。

### 3.4. 向量的內积 (点乘)

向量的內积，也常常被称为点乘。向量的內积可以用几何分析法和代数分析法来做。內积常用在判断两个向量的相似性（两个向量的夹角）、物理学里头的功的定义（力和位移的內积）。

几何分析法是向量內积的基础。

#### 3.4.1. 几何分析法

![向量內积](.\figure\向量內积.svg)

$\vec{OA}$ 和 $\vec{OB}$ 的內积 $\vec{OA} \cdot \vec{OB}$ 的结果是一个标量(就是没有方向，只有大小的数值)。具体操作如上图，平移是的两个向量的起点相同，然后将从一个向量$\vec{OB}$ 的终点$B$ 作另一个向量$\vec{OA}$ 的垂线 $BH$ ，然后将 模长$\lvert \vec{OH} \rvert$ 和模长$\lvert \vec{OA} \rvert$ 相乘，即得到一个数值$\lvert \vec{OH} \rvert \cdot\lvert \vec{OA} \rvert$ 就是 $\vec{OA} \cdot \vec{OB}$ 。

定义$\vec{e_1},\vec{e_2}$为直角坐标系中分别与$x$轴和$y$轴平行的两个基向量，根据以上分析，则有：
$$
\begin{cases}

\vec{OA} \cdot \vec{OB} = \lvert \vec{OH} \rvert \cdot\lvert \vec{OA} \rvert  = \lvert \vec{OA} \rvert \cdot\lvert \vec{OB} \rvert \cdot \cos{\theta} \\
\vec{e_1}\cdot \vec{e_2}= 1\cdot 1\cdot \cos{\frac {\pi}{2}} = 0 \\
\vec{e_1}\cdot \vec{e_1}= 1\cdot 1\cdot \cos{0} = 1 \\
\vec{e_2}\cdot \vec{e_2}= 1\cdot 1\cdot \cos{0} = 1 \\
\end{cases} \tag{3.4}
$$


#### 3.4.2. 代数分析法

根据向量內积的几何分析法的推论中的 $\vec{e_1}\cdot \vec{e_2}= 1\cdot 1\cdot \cos{\frac {\pi}{2}} = 0$ ，即垂直的两个向量的內积为0。

![向量內积_代数](.\figure\向量內积_代数.svg)

那么两个向量$\vec{OA}$ 和 $\vec{OB}$ 的內积可以为：

- 获取$\vec{OA}$ 和 $\vec{OB}$ 在直角坐标系基  $\vec{e_1}, \vec{e_2}$下的坐标 $(a_1,b_1)$ 和  $(a_2,b_2)$ 

- 将$\vec{OA} \cdot \vec{OB}= (a_1 \cdot \vec{e_1} + b_1\cdot \vec{e_2})\cdot (a_2 \cdot \vec{e_1} + b_2\cdot \vec{e_2})$ 按照普通代数乘法展开

- 展开得到 $\vec{OA} \cdot \vec{OB}= a_1b_1\cdot\vec{e_1}\cdot\vec{e_1} +a_2b_2\cdot\vec{e_2}\cdot\vec{e_2}+ a_1b_2\cdot\vec{e_1}\cdot\vec{e_2}+ a_2b_1\cdot\vec{e_2}\cdot\vec{e_1}$ ，带入向量內积几何分析法时候的结论 
  $$
  \begin{cases}
  
  \vec{e_1}\cdot \vec{e_2}= 1\cdot 1\cdot \cos{\frac {\pi}{2}} = 0 \\
  \vec{e_1}\cdot \vec{e_1}= 1\cdot 1\cdot \cos{0} = 1 \\
  \vec{e_2}\cdot \vec{e_2}= 1\cdot 1\cdot \cos{0} = 1 \\
  \end{cases} \tag{3.5}
  $$
  有 $\vec{OA} \cdot \vec{OB}= a_1b_1\cdot\vec{e_1}\cdot\vec{e_1} +a_2b_2\cdot\vec{e_2}\cdot\vec{e_2}=a_1b_1+a_2b_2$ 

综上所述，向量的內积，可以用直角坐标系下的坐标表示，然后将相乘向量的坐标分量对应相乘，最后求和即可。

### 3.5. 向量的叉积  (叉乘)

向量的叉积，也常常被称为叉乘。向量的叉积也可以用几何分析法和代数分析法来做。叉积常用在判断两个向量是否垂直（也可以用来求两个向量的夹角）、物理学里头的矩的定义（力和力臂的叉积）、快速求和两个向量构成的平面相垂直的向量方向。

几何分析法是向量叉积的基础。

#### 3.5.1. 几何分析法

![向量叉积_几何](.\figure\向量叉积_几何.svg)

上图中，两个向量$\vec{OA}$ 和 $\vec{OB}$ 进行叉积，得到向量 $\vec{OC}$ ， $\vec{OC}$ 的定义如下：

- $\vec{OC} = \vec{OA} \times \vec{OB}$

-  $\vec{OC}$ 同时与$\vec{OA}$ 和 $\vec{OB}$ 垂直，形成一个三维的空间。

- $\vec{OC}$的模长 $\lvert \vec{OC} \rvert =\lvert \vec{OA} \rvert \cdot \lvert \vec{OB} \rvert \cdot \sin{\theta}$

- $\vec{OC}$ 的方向符合右手法则。右手法则为：大拇指和食指处于手掌平面内，且相互垂直；中指弯曲成90度，和掌面垂直；大拇指指向$\vec{OA}$ 的正方向；食指指向$\vec{OB}$ 所在侧或者方向；则中指的方向即为$\vec{OC}$ 的方向。

根据向量叉积的几何定义，在如上的右手法则的垂直坐标系中，假设$\vec{e_1},\vec{e_2},\vec{e_3}$ 分别表示 $\vec{ox},\vec{oy},\vec{oz}$ 这3个方向的单位向量，向量叉积的有如下推论:


$$
\begin{cases}
\vec{e_1} \times \vec{e_2}=\vec{e_3}\\
\vec{e_2} \times \vec{e_3}=\vec{e_1}\\
\vec{e_3} \times \vec{e_1}=\vec{e_2}\\

\vec{e_1}\cdot \vec{e_1}= 1\cdot 1\cdot \sin{0} = 0 \\
\vec{e_2}\cdot \vec{e_2}= 1\cdot 1\cdot \sin{0} = 0 \\
\vec{e_3}\cdot \vec{e_3}= 1\cdot 1\cdot \sin{0} = 0 \\

\vec{OA} \times \vec{OB}= -\vec{OB} \times \vec{OA}

\end{cases} \tag{3.6}
$$


#### 3.5.2. 代数分析法

根据上述总结的坐标系基向量$\vec{e_1},\vec{e_2},\vec{e_3}$ 的叉乘规律，对三维空间中的任意两个向量$\vec{OA} ,\vec{OB}$ 的叉乘，可以按照如下步骤：

- 获取两个向量$\vec{OA} ,\vec{OB}$ 在基为$\vec{e_1},\vec{e_2},\vec{e_3}$ 的直角坐标系中的坐标 $(a_1,b_1,c_1)$ 和 $(a_2,b_2,c_2)$ 
- 将$\vec{OA} ,\vec{OB}$ 表示为 $\vec{OA}= a_1 \cdot \vec{e_1}+b_1 \cdot \vec{e_2}+c_1 \cdot \vec{e_3}$ 和$\vec{OB}= a_2 \cdot \vec{e_1}+b_2 \cdot \vec{e_2}+c_2 \cdot \vec{e_3}$
- 将$\vec{OA}\times\vec{OB} = (a_1 \cdot \vec{e_1}+b_1 \cdot \vec{e_2}+c_1 \cdot \vec{e_3}) \times (a_2 \cdot \vec{e_1}+b_2 \cdot \vec{e_2}+c_2 \cdot \vec{e_3}) $ 按照代数乘法展开
- $\vec{OA}\times\vec{OB} $展开，并将坐标系基向量$\vec{e_1},\vec{e_2},\vec{e_3}$ 的叉乘规律代入： 

$$
\begin{cases}
\vec{OA}\times\vec{OB}  & = a_1b_1 \cdot \vec{e_1} \times \vec{e_1} + a_2b_2 \cdot \vec{e_2} \times \vec{e_2} + a_3b_3\cdot \vec{e_3} \times \vec{e_3} \\ & + \ a_1b_2 \cdot \vec{e_1} \times \vec{e_2} + b_1a_2 \cdot \vec{e_2} \times \vec{e_1} \\ & + \ a_1c_2\cdot \vec{e_1} \times \vec{e_3} +  c_1a_2 \cdot \vec{e_3} \times \vec{e_1} \\ & + \ b_1c_2 \cdot \vec{e_2} \times \vec{e_3} + c_1b_2\cdot \vec{e_3} \times \vec{e_2} \\ & = (b_1c_2-c_1b_2)\vec{e_1} + (c_1a_2-a_1c_2)\vec{e_2} + (a_1b_2- b_1a_2)\vec{e_3} 
\end{cases} \tag{3.7}
$$

代数的方法能够更适合编程和数值计算。

## 4. 复数

复数在代数方程领域，主要是扩展了高次代数方程的根的形式。例如当一元二次方程的$\Delta$小于0的时候，是没有实根的。
$$
\begin{cases} 
ax^2+bx+ c &=0 \\ 
\quad \quad \mbox{for} \quad \quad  \Delta &< 0
\end{cases} \tag{4.1}
$$
这个时候，复数就派上用场了。复数中的一个重要概念，虚数单位 $i$ 的定义就如下：
$$
\begin{cases} 
& i^2 & = & -1 \\ 
& \sqrt[2]{-1} & = &i
\end{cases}\tag{4.2}
$$
常见的复数为 $c= a+b\cdot i$ ，其中 $a$ 和 $b$ 为实数，$a$ 为实部，$b \cdot i$ 为虚部。当 $b$ 为 0 是，$c$为 实数；当 $a$ 为 0 时，$c$ 为纯虚数。可见，复数的是包含实数的。所有的复数构成一个集合，用符号$C$ 表示。
    
对于$\Delta$小于0的一元二次方程，它虽然没有实根，但是它有两个复根，如下：
$$
\begin{cases} 
\Delta={b^2-4ac} < 0 \\
x_{1}= \frac{-b + i\sqrt{-(b^2-4ac)}}{2a}\\
x_{2}= \frac{-b - i\sqrt{-(b^2-4ac)}}{2a}
\end{cases}\tag{4.3}
$$
## 5. 代数方程和代数方程组

   基于以上对复数的定义，以及在一元二次方程无实根时的，它的复根的表示方法，有个重要结论：一般代数方程是几次，就有几个复根。这些复根中的一些根可以是虚部为0，退化成实根。一般有几个变量(成为几元)，就要几个方程才能求解。

### 5.1.  一元一次方程

$$
ax+b=0 \Longleftrightarrow x=-\frac{b}{a} \quad \mbox{for} \quad a\neq 0\tag{5.1}
$$

### 5.2.  一元二次方程

$$
\begin{cases} 
a \cdot x^2 +b \cdot x + c=0  \\ \mbox{for} \quad a\neq 0
\end{cases}
\Longleftrightarrow

\begin{cases} 
\begin{cases} 
\Delta={b^2-4ac} \ge 0 \\
x_{1}= \frac{-b + i\sqrt{-(b^2-4ac)}}{2a}\\
x_{2}= \frac{-b - i\sqrt{-(b^2-4ac)}}{2a}
\end{cases}
\\
\\
\begin{cases} 
\Delta={b^2-4ac} < 0 \\
x_{1}= \frac{-b + i\sqrt{-(b^2-4ac)}}{2a}\\
x_{2}= \frac{-b - i\sqrt{-(b^2-4ac)}}{2a}
\end{cases}
\end{cases} \tag{5.2}
$$



### 5.3. 一元高次方程

一元$n$次方程，$n$到了5次以上，就没有求根公式。一般是几次方程，就有几个复根。
$$
\begin{cases} 
   a_{n} \cdot x^n +a_{n-1} \cdot x^{n-1} +a_{n-2} \cdot x^{n-2} + \ldots + a_{1} \cdot x + a_{0} =0\\
   a_{n} \neq 0
\end{cases} \tag{5.3}
$$


### 5.4. 二元一次方程组

二元一次方程组，是非常基础的线性方程组。最典型的小学级别的问题就是鸡兔同笼问题，例如共 10只头，30只脚，求鸡和兔各有多少只。设鸡有$x$ 只, 兔有$y$ 只。列二元一次方程组。
$$
\begin{cases}
x&+\ y &=10 \\
2x&+ \ 4y &=30
\end{cases} \tag{5.4}
$$

### 5.5. 多元一次方程组
多元一次方程组，是计算机经常要求解的问题，在线性代数和矩阵论中讨论得非常多。多元线性方程组，在后期的讨论中，是一个非常重要的对象，会用矩阵来表示。

例如鸡，兔，鹅，鸭同笼，共 50只头；130只脚；单价是鸡20，兔100，鹅50， 鸭30，总价值 2800；单个利润为鸡5，兔30, 鹅10，鸭10，总利润为600。求鸡、兔、鹅、鸭各有多少只。设鸡、兔、鹅、鸭分别有 $x_1,x_2,x_3,x_4$只，列出4元一次方程组。
$$
\begin{cases}
x_1& +\ x_2 & + x_3 &+x_4 &=50 \\
2x_1&+\ 4x_2 & + 2x_3 &+2x_4 &=30\\ 
20x_1&+\ 100x_2 & + 50x_3 &+30x_4 &=2800\\ 
5x_1&+\ 30x_2 & + 10x_3 &+10x_4 &=600\\ 
\end{cases} \tag{5.5}
$$


### 5.6. 多元多次方程组

多元多次方程，几乎可以不考虑，很难求解。可能可以通过计算机进行数值求解。

## 6. 矩阵和线性方程组

由线性方程组和向量空间的需求，提出了矩阵的概念和应用。

- 线性方程组里头，例如上例中的4元一次方程组，公式5.5。这种写法中，$x_1,x_2,x_3,x_4$ 大量重复出现，写法上不够简洁。每个方程和其他的方程也有一定的关系。所以需要用一种更简洁的方式来表达。
  
- 向量里头，在一个选定了基向量的空间中，任何一个向量可以用该空间的基向量的线性组合来表示。例如在3维空间中，线性组合的3个系数就是这个向量在这组基(3个基向量)下的坐标。有几个基就有几个坐标分量。每个基也是一个向量，这个向量在其他的基下，也有其对应的坐标表示(3个分量)，那么这3个基在另一组基下的表示，就构成了一个$3\times3$ 的矩阵。这个涉及到线性变化，空间姿态变化等，以后再研究。

### 6.1. 矩阵的定义

矩阵就是一个$n$ 维的方块，2维的矩阵最常见，其表示方法为：
$$
\left[
 \begin{matrix}
   1 & 2 & 3 \\
   4 & 5 & 6 \\
   7 & 8 & 9
  \end{matrix}
  \right] \tag{6.1}
$$
在二维矩阵中，称横排为行，竖排为列。对于一个矩阵$A$ ，其中某个元素常用 $A_{ij}$来表示，$A_{ij}$表示第$i$行，第$j$列的元素。
$$
A =\left[
 A_{ij}
  \right] \tag{6.2}
$$

### 6.2. 矩阵的乘法

矩阵的乘法是为了线性方程组和向量变换服务。例如矩阵$A_{3\times4}$ 和矩阵 $B_{4\times5}$ 相乘得到矩阵 $C_{3\times5}$，表示为：
$$
C_{3\times5} =A_{3\times4}\cdot B_{4\times5} \tag{6.3}
$$
矩阵乘法的特点：

- 前面的举证的行数列数，要等于后面矩阵的行数。

- 以式6.3为例，结果矩阵$C$中的，$C_{ij}$ 是由矩阵$A$ 的第 $i$ 行和 矩阵 $B$ 的第 $j$ 列这两个4维向量作內积得到。 

$$
C_{ij} =\sum_{k=1}^4 A_{ik}  \cdot B_{kj} \tag{6.4}
$$

矩阵乘法的通式为：
$$
\begin{cases}
C_{m\times l} =A_{m\times n}\cdot B_{n \times l}  \\
C_{ij} =\sum_{k=1}^n A_{ik}  \cdot B_{kj}
\end{cases}\tag{6.5}
$$

### 6.3. 矩阵用于线性方程组

对于式5.5所描述的方程组，可以简化成三个矩阵相乘。

- $4 \times 4$的系数矩阵$A$
  $$
  A_{4 \times 4} = \left[
   \begin{matrix}
     1 & 1 & 1 &1 \\
     2 & 4 & 2 & 2 \\
     20 & 100 & 50 & 30 \\
     5& 30& 10&10
    \end{matrix}
    \right] \tag{6.6}
  $$

- $4 \times 1$的自变量矩阵$X$
  $$
  X_{4 \times 1} = \left[
   \begin{matrix}
     x_1 \\
     x_2 \\
     x_3 \\
     x_4
    \end{matrix}
    \right] \tag{6.7}
  $$

- $4 \times 1$的非齐次项矩阵$b$
  $$
  b_{4 \times 1} = \left[
   \begin{matrix}
     50 \\
     30 \\
     2800 \\
     600
    \end{matrix}
    \right] \tag{6.8}
  $$

- 式5.5所描述的4元一次方程组，就可是用矩阵相乘表示：
  $$
  A_{4 \times 4} \cdot X_{4 \times 1} = b_{4 \times 1} \tag{6.9}
  $$
  这样表示后，看起来像一元一次方程，求解过程也可以有点像一元一次方程，把方程两边同时 除以 系数矩阵 $A_{4 \times 4} $，就可以得到未知量$X_{4 \times 1}$的值。

  只不过矩阵中的算法，叫方程两边同时左乘以系数矩阵 $A_{4 \times 4} $的逆矩阵$A_{4 \times 4}^{-1}$。
  $$
  X_{4 \times 1} =A_{4 \times 4}^{-1} \cdot b_{4 \times 1} \tag{6.10}
  $$

### 6.4. 矩阵用于线性空间变换

以最简单的二维空间的线性变化为例。坐标一般用列向量表示。列向量相当于一个$n \times 1$的矩阵。

![线性变换](.\figure\线性变换.svg)

如上图，我们知道一个向量$\vec{O_1A}$ 在坐标系 $xO_1y$ 下的坐标 $(x_1,y_1)$。 假设$xO_1y$ 坐标下，沿 $O_1x$ 和 $O_1y$ 两个坐标轴的基向量分别为 $\vec{e_x^1}$ 和 $\vec{e_y^1}$，则有
$$
\vec{O_1A} =x_1\vec{e_x^1} +  y_1\vec{e_y^1}=
\left[
 \begin{matrix}
   \vec{e_x^1} &
  \vec{e_y^1} \end{matrix}
  \right] 
  
  \cdot
  
 \left[
 \begin{matrix}
   x_1 \\
   x_2 \\
  \end{matrix}
  \right] \tag{6.11}
$$
基向量$xO_1y$ 坐标下基向量$\vec{e_x^1}$ 和 $\vec{e_y^1}$ ，他们也是坐标系$xO_0y$ 下的普通向量。

获取$\vec{e_x^1}$ 和 $\vec{e_y^1}$ 在$xO_0y$ 下的坐标，分别为 $(r_{xx},r_{xy})$和 $(r_{yx},r_{yy})$。假设$xO_0y$ 坐标下，沿 $O_0x$ 和 $O_0y$ 两个坐标轴的基向量分别为 $\vec{e_x^0}$ 和 $\vec{e_y^0}$，则有
$$
\begin{cases}
\vec{e_x^1} = \left[
 \begin{matrix}
   \vec{e_x^0} &
  \vec{e_y^0} \end{matrix}
  \right] 
  
  \cdot
  
 \left[
 \begin{matrix}
   r_{xx} \\
   r_{xy} \\
  \end{matrix}
  \right] \\
  
  \vec{e_y^1} = \left[
 \begin{matrix}
   \vec{e_x^0} &
  \vec{e_y^0} \end{matrix}
  \right] 
  
  \cdot
  
 \left[
 \begin{matrix}
   r_{yx} \\
   r_{yy} \\
  \end{matrix}
  \right]
  \end{cases} \Longleftrightarrow 
  
  \left[
 \begin{matrix}
   \vec{e_x^1} &
  \vec{e_y^1} \end{matrix}
  \right] =   \left[
 \begin{matrix}
   \vec{e_x^0} &
  \vec{e_y^0} \end{matrix}
  \right] \cdot \left[
 \begin{matrix}
   r_{xx} & r_{yx} \\
  r_{xy} &r_{yy} \end{matrix}
  \right] \tag{6.12}
$$
相当于两个坐标系$xO_0y$ 和$xO_1y$ 的基向量之间，有个矩阵的变换公式。这个变换就是线性变化。
$$
\vec{O_1A} =x_1\vec{e_x^1} +  y_1\vec{e_y^1}=\left[
 \begin{matrix}
   \vec{e_x^1} &
  \vec{e_y^1} \end{matrix}
  \right] 
  
  \cdot
  
 \left[
 \begin{matrix}
   x_1 \\
   x_2 \\
  \end{matrix}
  \right] = \left[
 \begin{matrix}
   \vec{e_x^0} &
  \vec{e_y^0} \end{matrix}
  \right] \cdot \left[
 \begin{matrix}
   r_{xx} & r_{yx} \\
  r_{xy} &r_{yy} \end{matrix}
  \right] \cdot 
   \left[
 \begin{matrix}
   x_1 \\
   x_2 \\
  \end{matrix}
  \right] +   \left[
 \begin{matrix}
   \vec{e_x^0} &
  \vec{e_y^0} \end{matrix}
  \right] \cdot  \left[
 \begin{matrix}
   p_x \\
   p_y \\
  \end{matrix}
  \right] \\
  = \left[
 \begin{matrix}
   \vec{e_x^0} &
  \vec{e_y^0} \end{matrix}
  \right] \cdot (\left[
 \begin{matrix}
   r_{xx} & r_{yx} \\
  r_{xy} &r_{yy} \end{matrix}
  \right] \cdot 
   \left[
 \begin{matrix}
   x_1 \\
   x_2 \\
  \end{matrix}
  \right] + \left[
 \begin{matrix}
   p_x \\
   p_y \\
  \end{matrix}
  \right])\tag{6.13}
$$
由此可见，如果知道一个向量在$xO_1y$下的坐标$(x_1,y_1)$，想要求出来这个向量在另外一个坐标系$xO_0y$下的坐标$(x_0,y_0)$，直接将这个$(x_1,y_1)$当作一个列向量，乘以一个变换矩阵，然后加上坐标系的平移量，就可以算出来$(x_0,y_0)$。
$$
\left[
 \begin{matrix}
   x_0 \\
   x_0 \\
  \end{matrix}
  \right] =\left[
 \begin{matrix}
   r_{xx} & r_{yx} \\
  r_{xy} &r_{yy} \end{matrix}
  \right] \cdot 
   \left[
 \begin{matrix}
   x_1 \\
   x_2 \\
  \end{matrix}
  \right] + \left[
 \begin{matrix}
   p_x \\
   p_y \\
  \end{matrix}
  \right]\tag{6.14}
$$
为了把平移项的加法也移到矩阵乘法中，定义了一种叫其次坐标和其次变换矩阵。
$$
\left[ 
\begin{matrix}   
x_0 \\
x_0 \\
1  \end{matrix}
\right] 
=
\left[ 
\begin{matrix}   
r_{xx} & r_{yx} &  p_x\\  
r_{xy} &r_{yy} & p_y 
\\ 0& 0& 1
\end{matrix}  
\right] \cdot    
\left[ 
\begin{matrix}   
x_1 \\   
x_2 \\ 
1  
\end{matrix}  
\right]\tag{6.15}
$$
其次坐标，就是建立一个列向量，最后一个元素为1，前面两项为坐标分量。

其次变换矩阵，就是$T_0^1$
$$
T_0^1 ==\left[ \begin{matrix}   r_{xx} & r_{yx} &  p_x\\  r_{xy} &r_{yy} & p_y \\ 0& 0& 1\end{matrix}  \right] \tag{6.16}
$$
$r$ 代表两个坐标系之间的旋转信息，$p$ 代表两个坐标系啊之间的平移信息。

## 7. 代数方程对应的几何

几何中的点线面，其实就是坐标满足一定规律的点的集合。

### 7.1. 平面方程

在三维空间中，过点$(x_0,y_0,z_0)$，且和方向向量$(a,b,c)$ 垂直的平面，这个平面上的任一点$(x,y,z)$ 满足
$$
(\left[
 \begin{matrix}
   x \\
   y \\
   z
  \end{matrix}
  \right] -
  \left[
 \begin{matrix}
   x_0 \\
   y_0 \\
   z_0
  \end{matrix}
  \right]) \cdot 
  \left[
 \begin{matrix}
   a \\
   b \\
   c
  \end{matrix}
  \right]  =0 
  \Longleftrightarrow  ax+by+cz -(ax_0+by_0+cz_0) =0
  
  \tag{7.1}
$$
其中$ax_0+by_0+cz_0$ 为一个常数项。

所以平面方程可以一般化为 
$$
ax+by+cz+d =0   \tag{7.2}
$$
其中$(a,b,c)$ 为该平面的法矢方向（垂直于平面的方向）。

### 7.2. 圆方程

在二维平面上，圆是一个非常完美的图形。

定义圆之前，首先要定义一个被称为距离的概念。在代数解析几何中，直角坐标系中两个坐标间的距离，可以使用勾股定理推理处理。

两个点，$A$:$(x_0,y_0)$ 和 $B$:$(x_1,y_1)$之间的距离 $d$ 推理如下：

![勾股定理](.\figure\勾股定理.svg)
$$
d = \sqrt {(x_0-x_1)^2+(y_0-y_1)^2} \tag{7.3}
$$
如果将起点为$B$，终点为$A$ 的线段，当成一个向量，那么这个向量 $\vec{BA}$的模长就是式7.3的距离公式。

圆的定义就是到某一个点$(x_0,y_0)$ 的距离始终等于半径$r$的所有点构成的集合。

所以圆的方程为 
$$
r = \sqrt {(x-x_0)^2+(y-y_0)^2}    \Longleftrightarrow  r^2 = (x-x_0)^2+(y-y_0)^2 \tag{7.4}
$$

### 7.3. 球面方程

球和圆的原理是一样的，只不过圆是二维平面上的，球是三维空间中的。

球的定义就是到某一个点$(x_0,y_0,z_0)$ 的距离始终等于半径$R$的所有点的集合。
$$
R = \sqrt {(x-x_0)^2+(y-y_0)^2+(z-z_0)^2 }    \Longleftrightarrow  R^2 = (x-x_0)^2+(y-y_0)^2+(z-z_0)^2 \tag{7.5}
$$


### 7.4. 柱面方程

### 7.5. 抛物线方程
### 7.6. 椭圆方程
### 7.7. 双曲线方程
## 8. 旋转变换和一般的矩阵线性变换
## 9. 导数
## 10. 微分
## 11. 梯度
## 12. 迭代和梯度下降
## 13. 一般性凸优化
## 14. 不定积分
## 15. 定积分
## 16. 集合
## 17. 均值和方差
## 18. 正态分布
## 19. 概率和概率密度函数
## 20. 卷积和相关
## 21. 神经网络
## 22. 神经网络拓扑
## 23. 支持向量机( support vector machine, 缩写为 SVM)
## 24. 数字滤波
## 25. 级数
## 26. 傅里叶变换


