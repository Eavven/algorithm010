## 本周主题

>### 一、递归

>### 二、分冶

>### 三、回溯

### 一、递归

第一层 terminator，第二层 current level，第三层 drill down，第四层 清理

抛弃人肉递归以及递归树，找最近重复子问题，数学归纳法思维


```python
def recursion(level,param1,param2,……):
    # recursion terminator
    if level > MAX_LEVEL:
        process_result
    return 
    
    #process logic in current level
    process(level,data)

    #drill down
    self.recursion(level+1,p1,)
    
    #reverse the current level status if needed
```


```python
def recursion(level,param1,param2……):
    if level > MAX_LEVEL:
        process_result
    return

    process(level,data)
    
    self.recursion(level+1，p1，)
```

### 二、回溯

回溯法是一种探索所有潜在可能性找到解决方案的算法。如果当前方案不是正确的解决方案，或者不是最后一个正确的解决方案，则回溯法通过修改上一步的值继续寻找解决方案。


```python

```
