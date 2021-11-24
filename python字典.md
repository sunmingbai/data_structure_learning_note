## 关于字典的创建  
字典核心 key-value  

### 字典创建  
#创建空字典后 key-value式的赋值  
a=dict()  
a['name']='ming'  
a['age']=18  
#直接在创建时赋值  
a=dict(name=ming,age=18)  
#直接在创建时写成标准形式    
a={'name':'ming', 'age':18}  
#可以基于二元tuple或者列表的列表来创建    
a=[['name','ming'],['age',18]]  
dict(a)  
#然后是比较特殊一些的形式  
#初始化时所有value都相同  
a=dict.fromkeys(keylist,0)  

#或者针对两个长度相同的列表，想一一对应创建字典  
#先通过zip转化为键值对  
a=['name','age']  
b=['ming',18]  
c=zip(a,b)  
dict(c)  
### 字典的查增删改   
a['name']

a['weight']=78

del a['age']

a['name']=siyi

#还可以判断某个key 是否在列表中  
'name' in a  
### dict method探索  
#第一类 取出key value 或者item的  
list(a.keys())  
list(a.values())  
list(a.items())  
#第二类 根据key获取value  
a.get(key) #如果没有对应键值对返回的是None  
a.setdefault(key,value) #如果找不到对应键值对就返回默认值  
### 应用  
两数之和的元素
https://leetcode-cn.com/leetbook/read/tencent/xxqfy5/
参考链接 http://c.biancheng.net/view/2212.html
