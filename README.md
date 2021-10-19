# data_structure_learning_note
## Chapter 1  
1. What is algorithm? What's the relationship between algorithm and data structure?数据结构与算法的关系    
*Algorithm*: method to solve question.  
*data stucture* can be a part of algorithm, and algorithms are based on special data structure.
2. What is 'O' mark, and the most often used types大O标识是什么  
*'O'*  is used to measure the time complexity of an algorithm, or in other words, the time needed to obtain answer, and usually we consider the worest condition.   
The most common 'O()' including: O(n), O(n^2), O(log(n)), O(n*log(n)), O(n!)
3. An introduction to Binary Search Algorithm一个二分查找的例子    
Typicallly, to find an element in a list, we need to compare len(list) ( **O(n)** ) times at the worest case. But, with the help of Binary Search, we can find the element with **log(n)** times search(编程实例见代码部分)   
## Chapter 2  
1. 数组和链表的区别  
数组：数组中的element的内存地址是挨着的，所以 引用起来比较方便，特别是顺序引用的时候，但是增删时比较慢（并且增加时可能没有预留足够内存空间而失败）  
链表：内存地址是分开的，然后第一个中有指向第二个的地址，第二个中有指向第三个的地址...所以增删起来比较方便（改变地址指向即可）,但引用时不方便，找元素都要从第一个开始找 
于是有
读取 O(1) O(N)
增加 O(N) O(1)
删除 O(N) O(1)
2. 选择排序算法
一个简单的O(n^2)排序算法，细节见代码实现
## Chapter 3  
1. 关于递归
  a. 基线条件
  b. 递归条件
2. 关于栈
  a. 压入
  b. 弹出
3. 从栈的角度理解递归
  a. 先不断压入
  b. 再不断弹出
递归的优势相当于自己明确了一个序   
## Chapter 4  
1. 什么是D&C
找到足够简单的基线条件->缩小原始问题的规模。直至触达基线条件
  a. 示例一：分田地
  b. 示例二：求和sum
  c. 快排算法：
    i. 挑选基准值
    ii. 基于基准值分为两个子数组
    iii. 对两个子数组各自采取类似的操作
    iv. 基准条件是len(子数组)=1 返回子数组
    v. 代码实现
    vi. 快排算法的复杂度：
      1) 最佳情况 O(lgn)栈，每层O(n)
      2) 最差情况 O(n)栈，每层O(n)
由此引申出来的：快排是平均意义上的O(nlgn)，然后合并排序总是O(nlgn)，但是为什么我们通常说快排是最快的算法呢？--O记号反应的是增长趋势与增长速度，前面其实还有隐藏系数--单位时间，在快速排序和合并排序比较的场景，这个常数影响比较大，导致快速排序是最快的   
## Chapter 5  
1. 散列表
  a. 一个key只能有一个value
  b. 最好不要有多个key对应相同的value
  c. 查询的速度是O(1)
2. 冲突的情况与散列表性能
散列嵌套链表的方式来应对冲突，但是又要尽量分散开来（这块没有应用场景，没有太理解）
性能上平均情况引用-增删都是O(1)，最差情况都是O(n)（这里的最差情况也没有理解） 
然后涉及底层的散列函数的设计也略过了  
## Chapter 6  
1. 什么是图
对连接的一种描述
2. 什么是广度优先搜索算法 BFS
顾名思义，广度优先，然后主要解决两类问题
  a. 从a->b有没有连接
  b. 从a->b的最短连接
3. 怎样实现
  a. 规则 先进先出+一层一层
  b. Dqueue+dict
  c. 代码实现补充一下
4. 复杂度是怎样
  a. O(V+E) 边数+人数  
## Chapter 7  
狄克斯特拉算法
从最短到最快算法，考虑各边的加权，从BFS->Dijkstra's Algorithm
https://houbb.github.io/2020/01/23/data-struct-learn-03-graph-dijkstra
S U   不断找到最近的最好的路径，然后搜索过程中不断扩充
代码实现：见代码库

## Chaper 8  
1. 首先给了一些案例，阐述贪婪算法的必要性：背包问题，集合问题（**这里有个代码实现记得补充**） 
2. 怎样鉴别np hard问题然后尽快采用近似 算法：类似集合覆盖问题、指定中间点的旅行商问题、大规模的遍历问题...

## Chapter 9  
动态规划： 从简单问题到复杂问题，复杂问题的结果从简单问题的解中产生   

## Chapter 10  
KNN的讲解   

## Chapter 11  
关于其他的算法/数据结构

