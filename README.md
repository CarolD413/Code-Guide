# Python Questions with Detailed Comments and Notes

#### 2. 子文件路径
```
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

## Acknowledgments

Questions from:
* https://github.com/kenwoodjw/python_interview_question#python%E5%9F%BA%E7%A1%80
