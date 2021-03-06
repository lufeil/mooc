# 韩信点兵与中国剩余定理 
>
## 1 ”韩信点兵”的故事和《孙子算经》中的题目
>
### 韩信点兵的故事
>
- 五五数之剩一、六六数之剩五、七七数之剩四、十一数之剩十，韩信凭这些就可以计算出士兵的总数
>
### 《孙子算经》中的物不知数
>
- 今有物不知其数，三三数之剩2，五五数之剩3，七七数之剩2，问物几何？
>
## 2 从另一问题入手
>
### 由浅入深，从另一问题入手
>
- 今有物不知其数，
- 二二数之剩1，
- 三三数之剩2，
- 四四数之剩3，
- 五五数之剩4，
- 六六数之剩5，
- 七七数之剩6，
- 八八数之剩7，
- 九九数之剩8，
- 问物几何？
>
### 筛法：
>
- 按照条件一步一步地过筛子，逐步筛选出符合条件的。
>
- “二二数之剩1”的数，即“用2除余1”的数为：
- 1,3,5,7,9,11,13,15,17,19,21,23,25,......
>
- “三三数之剩2”的数，即“用3除余2”的数为：
- 5,11,17,23,......
>
- “四四数之剩3”的数，即“用4除余3”的数为：
- 11,23,......
>
- 再从中挑“五五数之剩4”的数，......
>
- 一直筛选下去，就可以得到结果。
>
### 公倍数法
>
#### 1 化繁为简
>
- “带余除法”是指整数的如下除法：a = bq + r
>
- **带余除法是通常整数除法的推广**
>
- x+1 = 2(n₁+1)
- x+1 = 3(n₂+1)
>
#### 2 寻找规律
>
- x+1 = k·\[2,3,4,5,6,7,8,9] = k·2520, k = 1,2,3,...
>
- 即 x = 2520k-1, k = 1,2,3,...
>
- 这就是原问题的全部解，有无穷多个解，其中第一个解释2519；我们只取正数解，因为“物体的个数”总是正整数。
>
## 3 《孙子算经》中”有物不知其数” 问题的解答
>
### 问题：
>
- 今有物不知其数，三三数之剩2，五五数之剩3，七七数之剩2，问物几何？
>
### 筛法
>
- 用3除余2：2, 5, 8, 11, 14, 17, 20, 23, 26, 29, ...
>
- 用5除余3：8, 23, ...
>
- 用7除余2：23, ...
>
#### 由此得到，23是最小的一个解。
>
### 公倍数法
>
- 设要求的数为x，则依题意，得联立方程组
>
- ⑴ x = 3·n₁ + 2  
- ⑵ x = 5·n₂ + 3
- ⑶ x = 7·n₃ + 2 
>
- 思路：方程的左边加上或减去一个合适的数，从而使左边分别是3,5,7 的公倍数。
>
- 从第3个等式入手 x + 5 = 7·(n₃ + 1) 
>
- x + 5 + 7·l = 7·(n₃ + 1 + l)，将l = 1,2,3,...代入试算、分析。
>
- **最后发现**，为使三个等式右边分别是3,5,7 的倍数，最小的加数是82(l=11,5+7l = 82)
>
- 三个等式两边均加82来求解，有
>
- ⑴ x + 82 = 3·(n₁ + 28)  
- ⑵ x + 82 = 5·(n₂ + 17)
- ⑶ x + 82 = 7·(n₃ + 12)
>
- x + 82 = k·\[3,5,7] = k·105 
>
- x = 105·k - 82, k = 1,2,3,...
>
- **但是82来之不易**；并且如果题目中的余数变了，就得重新试算，所以该方法在某种程度上**缺乏一般性**，为使它具有一般性，要做根本的修改。
>
## 4 单因子构件凑成法
>
- 下面采用一种新的思路来求解方程组中的x：
>
- ⑴ x = 3·n₁ + 2  
- ⑵ x = 5·n₂ + 3
- ⑶ x = 7·n₃ + 2 
>
- 把这里的x改记为s：
>
- ⑴ s = 3·n₁ + 2  
- ⑵ s = 5·n₂ + 3
- ⑶ s = 7·n₃ + 2 
>
- 对方程组做两方面的简化，得到三组方程:
>
- ⑴ x = 3·n₁ + 1  
- ⑵ x = 5·n₂ 
- ⑶ x = 7·n₃ 
>
- ⑴ y = 3·n₁  
- ⑵ y = 5·n₂ + 1
- ⑶ y = 7·n₃ 
>
- ⑴ z = 3·n₁  
- ⑵ z = 5·n₂
- ⑶ z = 7·n₃ + 1 
>
- 对第一个方程组
>
- ⑴ x - 70 = 3·(n₁ - 23)  
- ⑵ x - 70 = 5·(n₂ - 14) 
- ⑶ x - 70 = 7·(n₃ - 10) 
>
- x - 70 = k₁·\[3,5,7] = k₁·105
- x = 105·k₁ + 70 
>
- 第二个方程组
>
- ⑴ y - 21 = 3·(n₁ - 7)  
- ⑵ y - 21 = 5·(n₂ - 4) 
- ⑶ y - 21 = 7·(n₃ - 3) 
>
- y - 21 = k₂·\[3,5,7] = k₂·105
- y = 105·k₂ + 21
>
- 第三个方程组
>
- ⑴ z - 15 = 3·(n₁ - 5)  
- ⑵ z - 15 = 5·(n₂ - 3) 
- ⑶ z - 15 = 7·(n₃ - 2) 
>
- z - 15 = k₃·\[3,5,7] = k₃·105
- z = 105·k₃ + 15
>
- x 是被3除余1的数，y是被5除余1的数，z是被7除余1的数 
>
- x = 105·k₁ + 70
- y = 105·k₂ + 21 
- z = 105·k₃ + 15
>
- 凑出 s = 2·x + 3·y +2·z，s 不就是我们需求的数吗？
>
- 用3去除s时，3·y 和 2·z 都余0，除x余1，除2·x不就余2了吗？
>
- 类似，用5去除 s ，用7 除 s ，
>
- s = 2·x+3·y+2·z 
- = 2·(105k₁+70) + 3·(105k₂+21) + 2·(105k₃+15)
- = (70·2+21·3+15·2) + 105·(2k₁+3k₂+2k₃)
- = 70·2+21·3+15·2+105·k
- k = -2,-1,0,1,2,3,...
>
- **这就是《孙子算经》中“物不知数”一题的解，有无穷多解，最小的正整数解是23（k = -2 时）。**
>
### 单因子构件
>
- 每个单因子构件，都是用某一个数去除余1，用另两个数去除均余0的情况。再根据题目要求余数分别是2,3,2的情况，凑成题目的解答：
>
- s = 2x + 3y + 2z
>
- 然后计算得出解答的另一种表达形式：
>
- s = 70·2+21·3+15·2+105·k
>
- 所以上述方法叫“单因子构件凑成法”。
>
- 这种方法的优点是：对于问题叙述中“改变余数”后推广的一大批新问题，都不再需要重新计算，可以立即解决。
>
### 推广后的问题
>
- 有物不知其数，三三数之剩a，五五数之剩b，七七数之剩c，问物几何？
>
- 解为 s = 70a + 21b + 15c + 105k （ k ∈ Z, k 的选取应使 s > 0）。
>
### 歌诀
>
- 70 与 3 对应，被3除余1，被5,7除余0
- 21 与 5 对应，被5除余1，被3,7除余0
- 15 与 7 对应，被7除余1，被3,5除余0
- 105 被3,5,7除都余1
>
- 明朝数学界程大位在《算法统宗》中把上式总结为一首通俗易懂的歌诀：
>
- 三人同行七十稀，五树梅花廿一枝，
- 七子月圆正半月，除百零五便得知。
>
- 正半月是 15 。
>
## 5 中国剩余定理
>
- 公元1247年，南宗数学家秦九韶，将《孙子算经》中的物不知其数推广，得到称为“大衍求一术”的方法，在《数书九章》中发表。
>
- 称之为“中国剩余定理”（Chinese remainder theorem）
>
### 该定理用现在的语言表述如下：
>
- 设 d₁,d₂,d₃,...,dn 两两互素，x 分别被 d₁,d₂,d₃,...,dn 除所得的余数为 r₁,r₂,r₃,...,rn，则x可表示为
>
- x = k₁·r₁ + k₂·r₂ + ... + kn·rn + k·D
>
- 其中 D 是 d₁,d₂,d₃,...,dn 的最小公倍数，ki 是  d₁,d₂,d₃,...,dn 中去除 ki 的公倍数，且被 di 除所得余数为1，k是任意整数。
>
- **d₁,d₂,d₃,...,dn 必须两两互素**。
>
- 上面推广的“三三数之剩a，五五数之剩b，七七数之剩c”的“物不知数”问题中，与定理里各符号相对应的是：
- d₁ 为 3, d₂ 为 5, d₃ 为 7 ；
- r₁ 为 a, r₂ 为 b, r₃ 为 c ；
- k₁ 为 70, k₂ 为 21, k₃ 为 15 ；
- D 为 105.
>
- 苏联数学家 尤里-马季亚谢维奇 解决了希尔伯特提出的23个问题中的第10个问题，关键的地方用到了中国剩余定理。
>
## 6 有趣的应用
>
- 某单位有100把锁，分别编号为1,2,3,...,100.现在要对钥匙编号，使外单位的人看不懂，而本单位的人一看见锁的号码就知道该用哪一把钥匙。
>
- 方法很多，一种就是利用中国剩余定理。
>
### 方法一
>
- 把锁的号码分别被3,5,7去除所得的三个余数当做钥匙的号码。
>
- 例如：**8**号锁的钥匙编号是**231**。8被3除余2,8被5除余3,8被7除余1.
>
- 类似地，**23**号锁的钥匙编号是**232**，**45**号锁的钥匙编号是**003**，**52**号锁的钥匙编号是**123**。
>
- 因为只有100把钥匙，不超过105，所以**锁的号与钥匙的号是一一对应的**。
>
### 方法二
>
- 刚才得到的钥匙编号**加一常数**。
>
### 方法三
>
- 每过一个月更换常数。
>
