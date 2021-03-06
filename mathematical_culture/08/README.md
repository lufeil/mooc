# ”类比”的方法
>
## 1 什么是合情推理
>
- 推理是人思维活动的一个过程，是根据一个或几个已知的命题，来推断确定一个新的命题的思维过程。
>
- 数学离不开推理，推理一般包括两种类型：**合情推理**和**逻辑推理**
>
### 逻辑推理
>
- 是从事实和命题出发，严格符合逻辑法则的推理方式。主要指演绎推理、反证法、穷举法、数学归纳法、举反例。
>
- 在前提正确、逻辑法则也正确的情况下，逻辑推理的结论一定正确。
>
### 合情推理
>
- 是从事实和命题出发，合乎经验、直觉等情理的推理方式。主要指通过观察、实验、比较等方法，进行联想、类比、归纳、猜测等，得到新命题的推理形式。
>
- （不完全）归纳和类比是常用的合情推理。
>
- 合情推理的结论可能正确，也可能不正确，还要依靠逻辑推理去证明或者证否。
>
## 2 什么是类比
>
- 类比是一种推理方法，这种推理方法根据两个（或两类）对象之间在某些方面的相同或者类似，从而推出它们在某些方面也可能相同或者类似。
>
- 类比推理是一种“合情推理”，不是证明，它无法保证已知相同的属性与推出的属性之间有必然的联系；但它是活的新思路、新发现的一种方法、一种手段。 
>
#### 脑袋大脖子粗，不是大款就是伙夫。 
>
### 鲁班发明锯子 
>
- 就采用了类比的方法
>
## 3 插值问题中的类比
>
- 问题：有函数不知其式，在α处取值a，在β处取值b，在γ处取值c，问函数解析式为何？
>
- 类比：有物不知其数，三三数之剩a，五五数之剩b，七七数之剩c，问物几何？
>
- 类比的问题已经解决，单因子构件凑成法。 s = 70a + 21b + 15c + 105k （k∈Z）
>
### 现问题的解法：  
>
- 先做函数p(x)，使在α处值为1，在β，γ处值均为0；
- 再做函数q(x)，使在β处值为1，在α，γ处值均为0；
- 再做函数r(x)，使在γ处值为1，在α，β处值均为0。
>
- 即
>
- p(α) = 1    p(β) = p(γ) = 0
- q(β) = 1    q(α) = q(γ) = 0
- r(γ) = 1    r(α) = r(β) = 0
>
- 那么 
>
#### f(x) = a·p(x) + b·q(x) + c·r(x) 
>
- 就是所求的函数。
>
#### 原问题
- 有物不知其数，三三数之剩a，五五数之剩b，七七数之剩c，问物几何？
>
#### 现问题
- 有函数不知其式，在α处取值a，在β处取值b，在γ处取值c，问函数解析式为何？ 
>
#### 原问题的解：s = 70a + 21b + 15c + 105k （k∈Z）
>
#### 现问题的解：f(x) = a·p(x) + b·q(x) + c·r(x) 
>
#### 下面求出符合前面设计要求的函数p(x)，q(x)，r(x)。
>
- 设 p(x) 是一个多项式，则据条件p(β) = p(γ) = 0 知，
- 它有两个以此因式 x-β，x-γ，可令
>
- p(x) = λ·(x-β)·(x-γ) 
>
- 再用条件 p(α) = 1 去求待定系数 λ。把 x=α 代入上式。
- 得 1 = λ·(α-β)·(α-γ) 
>
- 故 p(x) = (x-β)·(x-γ)/((α-β)·(α-γ)) 
>
- **同理可求出** q(x) ， r(x)
>
- 把 p(x)，q(x)，r(x) 代入 f(x) 
>
### 可推广到任意有限点的插值公式
>
#### 用一个连续的函数去拟合离散的测量结果
>
### 华罗庚 联想到解决上述类似问题的方法
>
- 把上述解决问题的基本思想称为“单因子构件凑成法”，并概括成如下的“合成原则”：
>
- 要做出具有平行的、类似的几个性质 A,B,C 的一个数据结构，而 A,B,C 分别以某种量 α，β，γ 刻划，这时可用“单因子凑成构件法”：
- 先作 B,C 不发生作用，A 取单位量的构件；再作 C,A 不发生作用，B 取单位量的构件；再作 A,B 不发生作用，C 取单位量的构件。
>
- 然后用这些构件按照要求凑出所求的结构。
>
- 这个原则在有些书里称为：
>
### “孙子——华原则”
>
- 孙子是指与《孙子算经》中的题目有关，华是指与华罗庚有关。
>
- 体现了“**化繁为简**”的思想。
>
## 4 分割问题中的类比1
>
### 1 问题的提出和解决思路 
>
#### 5个平面最多把空间分为多少个部分？
>
- 从“抓三堆”游戏中学到的数学思想，可以先把问题一般化，再把问题特殊化，逐渐去找规律。
>
#### 问题一般化
>
- n个平面最多把空间分为多少个部分？
>
- 可记n个平面最多把空间分为F(n)个部分；再令 n = 1,2,3,... 把问题特殊化。 
>
- F(1) = 2, F(2) = 4, F(3) = 8
>
- F(4) = ?
>
## 5 分割问题中的类比2
>
### 2 四个平面分空间 
>
- 怎样描述“平面相交情况最复杂，才能把空间分割出的部分数最多”呢？——数学语言可以做到。
>
- 两句话：
>
- 一句话是，n个平面中每个平面与其余的n-1个平面都相交，且任意三个平面都只交于一点；
>
- 另一句话是，n个平面中每个平面都不过它以外任意三个平面的交点。
>
- 四面体的四个面无限延展以后所成的四个平面，相交情况最复杂，从而是把空间分割出的部分数最多的情况。
>
#### 类比3条直线分割平面的情形
>
- 有限面积的有1个，有公共顶点的有3个，有公共边的有3个。
>
#### 四面体分割类比
>
- 有限空间的有1个，有公共顶点的有4个，有公共棱的有6个，有公共面的有4个，此外没有了
>
#### 不一定正确，因为是类比，是合情推理，还需要逻辑证明。
>
- 四个平面最多把空间分为15个部分。
>
### 在“一般情形”下考虑问题：
>
- n个平面分割空间和n条直线分割平面。简称为“类比一般化”。
>
## 6 分割问题中的类比3
>
### 3 类比一般化
>
- n 条直线“处于一般位置”的要求是：任意两条直线都相交，任意三条直线都不共点。 
>
- n 个平面“处于一般位置”的要求是：任意两个平面都相交且任意三个平面都只交于一点，每个平面都不过它以外任意三个平面的交点。
>
- n 个点最多把直线分为 n+1 个位置。0 个点最多把直线分为一个部分。
>
#### 点分直线、直线分平面、平面分空间
>
- L(n)， f(n)， F(n) 分别表示 n个点分直线，n条直线分平面，n个平面分空间最多分得的部分数。
>
- 孤立的问题有时难于解决，而解决系列问题有时比解决孤立问题好入手。 
>
- 从第2行开始，每个数都可由它“**头顶上**”的数与“**左肩膀**”上的数相加而得到。
>
## 7 分割问题中的类比4
>
### 分析、推理 
>
- 3 条直线最多分平面为7个部分，4 条直线分平面时，与原来的3条直线分别相加，形成3个新交点，3个点分新直线为4部分。
>
- 4 + 7 = 11 
>
|分割元素个数|点分直线|直线分平面|平面分空间|
|:---------:|:------:|:------:|:--------:|
|0          |1       |1       |1         |
|1          |2       |2       |2         |
|2          |3       |4       |4         |
|3          |4       |7       |8         |
|4          |5       |(11)    |15        |
|5          |6       |(16)    |(26)      |
|...        |...     |...     |...       |
|n-1        |L(n-1)=n|f(n-1)  |F(n-1)    |
|n          |L(n)=n+1|f(n)    |F(n)      |
>
### 类比分析 n = 4 时平面分空间的情况
>
- 即求 F(4) = 15  
>
- 3 个平面最多分空间为8个部分，
>
- 再添加一个平面，这个平面与原来的3个平面都相交，并且不过原来3个平面的交点，从而不过原来任意两个平面的交线 
>
- 这样就交出了3条新直线，这3条直线把新添加的平面最多分为7个部分，这7个平面当中的每一个，都把它所穿过的，由前3个平面所分成的空间区域一分为二。
>
- 因此空间分割就增加了7个部分。而原来已经有8个部分，7 + 8 = 15，这就是 F(4) = 15 的来历。
>
- 从表格中发现的规律：从第2行开始，每个数都可由它“**头顶上**”的数与“**左肩膀**”上的数相加而得到。是正确的。
>
### 5 条直线分平面 和 5 个平面分空间的逻辑推理
>
- ...
>
## 8 分割问题中的类比5
>
### 一般情形的递推公式
>
- “n 条直线最多把平面分割成多少个部分”的表达式 
>
- f(n) = L(n-1) + f(n-1)
>
- “n 个平面最多把空间分割成多少个部分”的表达式
>
- F(n) = f(n-1) + F(n-1)
>
- 这两个递推公式与斐波那契数列有区别，但是思想是一致的。
>
#### 分析和推导一遍后一个公式：F(n) = f(n-1) + F(n-1)
>
- 实际上只要沿用上面推理叙述的框架：
>
- 把“3个平面”换为“n-1个平面”
>
- 把“8个部分”换为“F(n-1)个部分”
>
- 把“3条新直线”换为“n-1条新直线”
>
- 把“7个部分”换为“f(n-1)个部分”
>
- 把“15”换为“F(n)”
>
- 就完成证明了。
>
- 在n-1个平面把空间分为F(n-1)个空间的基础上，再添加一个平面，这个平面与原来的n-1个平面都相交，并且又不过原来任意3个平面的交点，
>
- 从而不过原来任意两个平面的交线，这样就交出了n-1条新直线，n-1条新直线把新添加的平面最多分成f(n-1)个部分，
>
- 其中每一个部分把它所穿过的由前面n-1个平面分成的空间区域一分为二，多出f(n-1)个区域，原来有F(n-1)个区域，
>
- 所以n个平面分空间，最多分的空间 F(n) = f(n-1) + F(n-1)
>
#### f(n) = L(n-1) + f(n-1) 的逻辑推导
>
- 
>
## 9 分割问题中的类比6
>
### 显式 f(n) = 1 + n·(n+1)/2 及 F(n) = (1/6)·(n³ + 5·n + 6)
> 
- 前面得到的是递推公式。
>
- 我们希望进一步得到像 L(n) = n + 1 那样的、关于 f(n) 及 F(n) 的显式表达式，即直接用 n 的解析式来表达 f(n) 及 F(n)。
>
- 利用 f(0) = 1 及递推公式 f(n) = L(n-1) + f(n-1) 得到一系列等式
>
- f(0) = 1
- f(1) = L(0)+f(0)
- f(2) = L(1)+f(1)
- f(3) = L(2)+f(2)
- ......
>
- f(n-1) = L(n-2)+f(n-2)
- f(n) = L(n-1) + f(n-1)
>
#### 等号两边分别相加、消去等号两边相同的项
>
- f(n) = 1 + L(0) + L(1) + L(2) + ... + L(n-2) + L(n-1)
>
#### 化简整理
>
- f(n) = 1 + ∑L(i) i=0 到 i=n-1，其中 L(i) = (i+1)
>
- f(n) = 1 + n(n+1)/2 
>
#### 同样可得 F(n) 的显式表达式 
>
- 
>





