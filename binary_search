# -*- coding: utf-8 -*-
"""
Created on Sat Oct 16 16:52:29 2021

@author: mings
"""

# 配套算法图解的实现
# 实现二分查找
# 输入： list->nums，要找的对象target
# 输出，target在list中的下标 
def binary_search(nums,target):
    # initailize
    low=0
    high=len(nums)-1
    print(high)
    while low<=high:
        print(low,high)
        mid=int((low+high)/2)
        print(mid)
        guess=nums[mid]
        if guess==target:
            return mid
            break
        elif guess>target:
            low=low
            high=mid-1
        else:
            low=mid+1
            high=high         

# 注意nums必须是有序的
nums=[1,3,5,9,10,24,40,47,99]
target=47
print('Target\'s position:',binary_search(nums, target))
