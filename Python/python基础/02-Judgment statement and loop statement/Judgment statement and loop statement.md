### 判断语句

#### if

```python
# 语法：
if 要判断的条件:
        条件成立时，要做的事情

```

```python
# 例子：
if 2>1:
    print('hello world')
```

#### 比较关系运算符

```python
'''
==	    检查两个操作数的值是否相等，如果是则条件变为真。	      
!=	    检查两个操作数的值是否相等，如果值不相等，则条件变为真。	  
>	    检查左操作数的值是否大于右操作数的值，如果是，则条件成立。	  
<	    检查左操作数的值是否小于右操作数的值，如果是，则条件成立。	  
>=	    检查左操作数的值是否大于或等于右操作数的值，如果是，则条件成立
<=	    检查左操作数的值是否小于或等于右操作数的值，如果是，则条件成立
'''
```



#### if-else

```python
# 语法：
if 判断语句:
    成立执行
else:
    不成立执行
```



```python
# 例子：
str = input("输入一个1~10之间的数字")
str = int(str)
if str >=1 and str<=10:
    print("你输入的数字是%d" % str)
else:
    print("你输入的数字不在规定范围，请重新输入")
```



#### elif

```python
if 条件1:
    事件1
elif 条件2:
	事件2
elif 条件3:
    事件3
else:
    都不满足执行
    
'''
elif必须和if一起使用，否则出错
else 一般用在最后，即所有条件都不满足时使用
'''
```





----

### 循环语句

#### while

```python
# 语法：
while 条件:
    条件满足时，做的事情1
    条件满足时，做的事情2
    条件满足时，做的事情3
    ...
```

```python
# 例子：
i = 1
sum = 0
while i<=100:
    sum = sum +i
    i += 1

print("1~100的累加和是：%d" % sum)# 1~100的累加和是：5050
```



#### for

```python
# 语法
for 临时变量 in 字符串or列表等可迭代对象:
    循环条件满足时执行
    
```

```python
# 例子
str = 'hello'
for i in str:
    print(i)
```



#### break `and`continue

```python
break 跳出这个循环
continue 跳出本次循环
```

```python
# 例子
str = [1,2,3,4,5]
for i in str:
    if i == 3:
        break
    print(i) # 1 \n 2
    
    
str = [1,2,3,4,5]
for i in str:
    if i == 3:
        continue
    print(i) # 1\n 2\n 4\n 5
```

