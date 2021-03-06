# 问题求解与算法设计基础2 
>
## 1 RAPTOR进阶
>
### RAPTOR-数组变量
>
- 
>
## 2 求最大最小值
>
### 计算最大值
>
#### 以计算最大值为例
>
- 输入一组数据，输出其中的最大值
>
#### 生活中的例子
>
- 找出某网站微博最有影响力的博主
>
- 某年高考中的理科状元
>
- 某场球赛中进球最多的球员
>
- 手里扑克牌中牌面最大的牌 
>
### 计算最大值的方法
>
- 先假设这组数据中的第一个数为当前的最大值
>
- 其余的数依次与当前最大值进行比较
>
- 一旦发现后面的某个数大于当前的最大值，则用该数修改当前的最大值
>
## 2 线性查找
>
### 线性查找（Linear Search）
>
#### 不要求数据表是已排好序的
>
- 从线性数据表中的第一个（或最后一个）记录开始查找，依次将记录的关键字与给定的值进行比较
>
- - 当某个记录的关键字与给定的值相等时，即查找成功
>
- - 反之，查完全部记录都没有与之相等的关键字，则查找失败
>
#### 线性查找的性能
>
- 最好情况
>
- 最坏情况
>
- 平均情况
- - 查找次数是数据量的一半
>
### 小结
>
#### 查找策略与数据排序与否，数据自身属性有关
>
- 线性查找针对未排序数据
>
- 二分查找针对已排序数据，适用于不经常变动而查找频繁的有序列表
>
- 从平均情况来看，线性查找法需要与（一半）的数组元素与查找关键字进行比较。
>
- 二分查找要求查找表中的数据采用顺序存储结构，而且必须按关键字大小（有序）排列
>
### 查找算法
>
#### 查找（Search）算法和排序算法有密切的联系
>
- 因为许多查找算法依赖于要查找的数据集的有序程度
>
#### 基本的查找算法有以下4种：
>
- 线性查找，也称顺序查找
>
- 折半查找，也称二分查找
>
- 分块查找，也称索引线性查找
>
- 哈希查找
>
## 3 二分查找
>
### 二分查找（Binary Search）
>
#### 要求数据表是已排好序的
>
- 先将表的中间位置记录的关键字与查找关键字比较
>
- - 如果两者相等，则查找成功
- - 否则将表分成前、后两个子表，根据比较结果，决定查找哪个子表
>
### 二分查找的性能
>
- 每执行一次，都将查找空间减少一半，是计算机科学中分治思想的完美体现
>
- 比较次数少，查找速度快，平均性能好
>
- 最多所需的比较次数是第一个大于表中元素个数的2的幂次数
>
### 缺点
>
- 要求待查表按关键字有序排列
>
- 必须采用顺序存储结构，插入和删除数据需移动大量的数据
>
- 适用于不经常变动而查找频繁的有序表
>
## 4 分块查找
>
### 查找算法
>
#### 基本的查找算法有以下4种：
>
- 线性查找，也称顺序查找
>
- 二分查找，也称折半查找
>
- 分块查找，也称索引线性查找————线性查找的改进
>
- 哈希查找
>
### 分块查找的基本思想
>
- 将n个数据划分为m（m ≤ n）个数据块
>
- 每一个数据块中的数据不必有序
>
- 但块与块之间必须“按块有序”
>
- - 第1块中任一元素的关键字必须小于第2块中任一元素的关键字
- - 第2块中任一元素又都必须小于第3块中的任一元素，…
>
### 分块查找的基本步骤
>
#### 第1步：在块间查找，找到数据所在的块
>
- 块与块之间“按块有序”——线性或二分查找
>
#### 第2步：在一个数据块内进行查找
>
- 块中的数据非有序——线性查找
>
#### 如何找到数据所在的块呢？
>
#### 首先要建立一个块最大关键字表
>
- 抽取各块中的最大关键字及其块的起始地址构成索引表
>
- 由于表是分块有序的，所以索引表是一个有序表
>
![](https://github.com/lufeil/mooc/blob/master/programing_basic/5/pic/1.png)
>
#### 分块查找过程
>
- 1）用线性或二分查找法查找索引表，由最大关键字查出所在的块
>
- 2）用线性查找在块中查找
>
![](https://github.com/lufeil/mooc/blob/master/programing_basic/5/pic/2.png)
>
### 分块查找算法的分析
>
#### 优点
>
- 在表中插入或删除一个记录时，只要找到该记录所属块，就在该块中进行插入或删除运算，无需大量移动记录
>
- 平均查找次数比线性查找少，性能介于线性查找和二分查找之间
>
- 适用于顺序存储结构和线性链表
>
#### 主要代价
>
- 增加了一个索引表的存储空间，以及将初始表分块排序的运算
>
## 5 哈希查找
>
### 哈希查找
>
#### 哈希是hash的音译，也称散列
>
- 哈希查找是一种按关键字编址的快速检索方法 
>
#### 与其他查找方法的不同之处
>
- 哈希查找是通过对记录的关键字值进行某种运算，直接求出记录的地址
>
- 快——**关键字到地址**直接转换，无需反复比较
>
- 核心不在于如何“比较”，而在于如何“计算”
>
- 最能体现计算机科学**精髓**的查找方法
>
### 哈希查找的基本思想
>
#### 以按姓名作为关键字查找为例
>
- 对姓名中各个汉字的拼音首字母进行编号
>
- 用姓名中所有汉字的拼音首字母的编号值相加求和
>
#### 核心是设计哈希函数， 并构建哈希表
>
#### 哈希查找过程
>
- 由给定的关键字值key，根据哈希函数计算出对应的哈希地址H(key)
>
- 根据H(key)直接找到该记录的存储位置
>
- 本质是先将待查数据映射成一个哈希值，然后查找具有这个哈希值的数据
>
### 哈希冲突与解决
>
#### 当两个不同的数据的哈希值相同时，就会发生冲突（collision）
>
#### 处理哈希冲突的常用方法之一
>
- 链地址法
>
- - 将哈希值相同的数据存在一个链表中
- - 查找哈希表时，当查找到这个链表时，必须采用线性查找方法
>
### 哈希函数的典型构造方法
>
#### 构造方法有很多
>
#### 一种经典的构造方法——求模取余法
>
- H(key) = key % p
>
- p<=m，哈希表表长为m
>
- 余数（哈希地址）总是循环出现，呈周期性变化
>
### 哈希函数的典型构造方法
>
#### 求模取余法举例
>
![](https://github.com/lufeil/mooc/blob/master/programing_basic/5/pic/3.png)
>
### 哈希函数的常用设计方法
>
![](https://github.com/lufeil/mooc/blob/master/programing_basic/5/pic/4.png)
>
### 哈希表的特点
>
|一般的线性表|哈希表|
|:------|:------|
|在记录的存储地址与它的关键字之间不存在确定的对应关系|在记录的存储地址和它的关键字之间存在一个确定的对应关系|
|在表中查找记录时，需要进行一系列的关键字比较|每个关键字在表中有唯一的一个存储地址与之对应，直接由关键字找到存储地址|
|建立在“比较“的基础上，查找效率依赖于查找过程中所进行的比较次数|根据关键字直接计算出记录存放的地址查找效率高|
>
### 小结
>
#### 查找策略与数据排序与否，以及数据自身的属性有关
>
|查找方式|数据|
|:----|:-----|
|顺序查找|针对未排序数据|
|二分查找|针对已排序数据|
|分块查找|针对按块有序、块内无序的数据|
|哈希查找|通过计算数据的存储地址进行查找关键在于哈希函数的构造|
>

