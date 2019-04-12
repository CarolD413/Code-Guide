### np.array()
```py 
# 二维数组：嵌套序列（列表，元祖均可）
ar3 = np.array([[1,2,3],(‘a’,’b’,’c’)]) 
# 注意嵌套序列数量不一会怎么样
ar4 = np.array([[1,2,3],(‘a’,’b’,’c’,’d’)]) print(ar3,ar3.shape,ar3.ndim,ar3.size) # 二维数组，共6个元素
print(ar4,ar4.shape,ar4.ndim,ar4.size) # 一维数组，共2个元素
>> 
[[‘1’ ‘2’ ‘3’]
[‘a’ ‘b’ ‘c’]] (2, 3) 2 6
[[1, 2, 3] (‘a’, ‘b’, ‘c’, ‘d’)] (2,) 1 2
```
