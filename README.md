# Python Questions with Detailed Comments and Notes

#### 2. 子文件路径
```python
def print_directory_contents(sPath):
"""
Given the path of a directory, 
this function returns the paths of all the files under the given directory
"""
import os
#os.listdir() returns a list containing the names 
#of the entries in the directory given by path
for s_child in os.listdir(s_path):
    s_child_path = os.path.join(s_path, s_child)
    if os.path.isdir(s_child_path):
        print_directory_contents(s_child_path)  
    #recursion until it's not a directory
    else:
        print(s_child_path)
  
```

#### 5. 现有字典 d= {'a':24,'g':52,'i':12,'k':33}请按value值进行排序?
```python
sorted(d.items(),key=lambda x:x[1])
```
#### 7.请反转字符串 "aStr"?
```python
print("aStr"[::-1])
```

#### 8.将字符串 "k:1 |k1:2|k2:3|k3:4"，处理成字典 {k:1,k1:2,...}
```python
str1 = "k:1|k1:2|k2:3|k3:4"
def str2dict(str1):
    result = {}
    for item in str1.split("|"):
        key, value = item.split(":",1)
        dict[key] = a[value]
    return result

#字典推导式
d = {k:int(v) for t in str1.split("|") for k, v in (t.split(":"), )}
```
## Acknowledgments

Questions from:
* https://github.com/kenwoodjw/python_interview_question#python%E5%9F%BA%E7%A1%80
