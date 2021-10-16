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
