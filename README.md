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
