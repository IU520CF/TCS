### 注释

```python
# 我是python单行注释

'''
我是python
多行注释
'''
```



### 变量

```python
num1 = 100 # num1 就是一个变量
num2 = 200 # num2 也是一个变量
resule = num1 + num2 # 定义resule变量 并把num1变量和num2变量的和赋值给resule

# python 定义一个变量并赋值，那么它的类型就确定了，不需要开发者主动说明它的数据类型，系统会自动识别
print(type(resule))
# 可以使用 type(变量名)  查看变量的数据类型

```

### 标识符和关键字

```python
'''
    标识符
    标识符：开发人员在程序中自定义的一些符号和名称
    标识符是自己定义的，如变量名、函数名等
'''

'''
    标识符通用规则：
    标识符由字母、下划线、数字组成、且数字不能开头
    python 中的标识符是区分大小写的
'''

'''
    命名规则：
    驼峰命名法
'''

'''
    关键字
    python 中一些 具有特殊功能的标识符，就是所谓的关键字
    关键字，是python 已经使用了，所以不允许开发者自己定义和关键字相同的标识符
    查看关键字：
    1.方法一
    >>> import keyword
    >>> keyword.kwlist
    2.方法二 (推荐：打印后整齐)
    >>> help('keywords') 
    False               break               for                 not
    None                class               from                or
    True                continue            global              pass
    __peg_parser__      def                 if                  raise
    and                 del                 import              return
    as                  elif                in                  try
    assert              else                is                  while
    async               except              lambda              with
    await               finally             nonlocal            yield
'''
```

### 输出

```python
# python 中变量的输出

print('hello world') # 打印

# 在python print 输出语句中看到 % 操作符，就是python格式化输出
# %s 字符串
# %d 数字
age = 18
name = '小明'
print("我是%s, 年龄是%d" % (name, age))# 我是小明, 年龄是18

'''
    常用的格式化符号
    格式符号	转换
    %c	    字符
    %s	    字符串
    %d	    有符号十进制整数
    %u	    无符号十进制整数
    %o	    八进制整数
    %x	    十六进制整数（小写字母0x）
    %X	    十六进制整数（大写字母0X）
    %f	    浮点数
    %e	    科学计数法（小写'e'）
    %E	    科学计数法（大写“E”）
    %g	    ％f和％e 的简写
    %G	    ％f和％E的简写
'''


'''
    换行输出
    \n ：换行输出
'''
print('123456')
print('123\n456')
```

### 输入

```python
# python 输入
# 和 js页面输入框一样都是 input
uanme = input("请输入昵称") # 后台测试输入
print('你的昵称是%s' % uanme)
# 注意 input 输入的数据都是 字符串 类型
```

### 运算符

```python
'''
    运算符：
    1.算术运算符
    运算符	描述	    实例
    +	    加	    两个对象相加 a + b 输出结果 30
    -	    减	    得到负数或是一个数减去另一个数 a - b 输出结果 -10
    *	    乘	    两个数相乘或是返回一个被重复若干次的字符串 a * b 输出结果 200
    /	    除	    b / a 输出结果 2
    //	    取整除	返回商的整数部分 9//2 输出结果 4 , 9.0//2.0 输出结果 4.0
    %	    取余	    返回除法的余数 b % a 输出结果 0
    **	    指数	    a**b 为10的20次方， 输出结果 100000000000000000000

    2. 赋值运算符
    运算符	        描述	            实例
    =	            赋值运算符	    把 = 号右边的结果 赋给 左边的变量，如 num = 1 + 2 * 3，结果num的值为7

    3.复合赋值运算符

    运算符	描述	            实例
    +=	    加法赋值运算符	    c += a 等效于 c = c + a
    -=	    减法赋值运算符	    c -= a 等效于 c = c - a
    *=	    乘法赋值运算符	    c *= a 等效于 c = c * a
    /=	    除法赋值运算符	    c /= a 等效于 c = c / a
    %=	    取模赋值运算符	    c %= a 等效于 c = c % a
    **=	    幂赋值运算符	    c **= a 等效于 c = c ** a
    //=	    取整除赋值运算符	c //= a 等效于 c = c // a
'''
```

### 常见数据类型转换

```python
'''
常见数据类型转换

函数	                        说明
int(x [,base ])	            将x转换为一个整数
float(x )	                将x转换为一个浮点数
complex(real [,imag ])	    创建一个复数，real为实部，imag为虚部
str(x )	                    将对象 x 转换为字符串
repr(x )	                将对象 x 转换为表达式字符串
eval(str )	                用来计算在字符串中的有效Python表达式,并返回一个对象
tuple(s )	                将序列 s 转换为一个元组
list(s )	                将序列 s 转换为一个列表
chr(x )	                    将一个整数转换为一个Unicode字符
ord(x )	                    将一个字符转换为它的ASCII整数值
hex(x )	                    将一个整数转换为一个十六进制字符串
oct(x )	                    将一个整数转换为一个八进制字符串
bin(x )	                    将一个整数转换为一个二进制字符串
'''

# 将数据类型转换为 int 类型
str1 = '10'
num1 = int(str1)
print(type(num1))

# 处理浮点数，只留下整数部分 （不是四舍五入）
num2 = int(3.9879)
print(num2)

# int(要转换的变量,按几进制转换后显示)
resule = int(str1,32)
print(resule) # 32 结果显示进制数

```

