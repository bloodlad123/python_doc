(需要先安装Python环境和jupyter)
# Python培训

## 1. Python基础知识
- 变量：存储各种文件信息和数据
- 数据类型：文本类型数字类型
- 流程控制语句：控制批量处理文件的过程
- 函数：封装需要重复使用的代码
- 模块：办公自动化模块、openpyxl数据处理模块、pandas
### 1.1 Hello Python
print() 函数用于将指定的内容打印到标准输出（通常是控制台）。
- 打印字符串：
    print('Hello!欢迎来到Python世界！')
    - 如果你想在字符串中插入一个<font color="red">包含引号的字符</font>，可以：
  1) 使用反斜杠转义:print('Hello!yelcone to the python\'s worldi')
  2) 使用双引号：print("Hello!yelcone to the python's worldi")
*<font color="red">在Python中，单引号（'）、双引号（"）和三引号（'''或"""）都可以用来表示字符串。</font>*
    - 单引号和双引号之间没有实质性的区别，你可以根据个人偏好选择使用其中之一。以下是单引号和双引号的示例：
    ```python
    single_quoted_string = '这是一个单引号字符串'
    double_quoted_string = "这是一个双引号字符串"

    print(single_quoted_string)
    print(double_quoted_string)
    ```
    ```python
    # 输出结果为：
    这是一个单引号字符串
    这是一个双引号字符串
    ```

    - 当字符串中有单引号时，该字符串必须用双引号或三引号表示 
    ```python
    string_with_single_quote = "这是一个包含 ' 单引号的字符串"
    triple_single_quoted_string = '''这是一个包含 ' 单引号的字符串'''
    print(string_with_single_quote)
    print(triple_single_quoted_string)
    ```
    ```python
    # 输出结果为：
    这是一个包含 ' 单引号的字符串
    这是一个包含 ' 单引号的字符串
    ```
    - 而三引号可以用来创建多行字符串，其中可以包含换行符等特殊字符。三引号可以使用单引号或双引号。以下是三引号的示例：
    ```python
    triple_single_quoted_string = '''这是一个
    多行单引号字符串'''
    triple_double_quoted_string = """这是一个
    多行双引号字符串"""

    print(triple_single_quoted_string)
    print(triple_double_quoted_string)
    ```
    ```python
    # 输出结果为：
    这是一个
    多行单引号字符串
    这是一个
    多行双引号字符串
    ```

- 打印数字：
    ```python
    number = 8900
    print(number)
    ```
    输出结果为:
    ```python
    8900
    ```
    *给数字加上引号：*
    ```python
    number = '8900'
    print(number)
    ```
    输出结果为:
    ```python
    8900
    ```

    <span style="color:red">8900表示的是数字，是可以进行加减乘除的数字<br>8900'表示的一串由"8"、"9"、"0"、"0"4个字符组成的字符串</span>

 - 打印数学表达式：
    ```python
    # 打印加法表达式
    print("加法表达式: 5 + 3")

    # 打印减法表达式
    print("减法表达式: 5 - 3")

    # 打印乘法表达式
    print("乘法表达式: 5 * 3")

    # 打印除法表达式
    print("除法表达式: 5 / 3")

    # 打印指数表达式
    print("指数表达式: 5 ** 3")

    ```
    ```python
    # 输出结果为：
    加法表达式: 5 + 3
    减法表达式: 5 - 3
    乘法表达式: 5 * 3
    除法表达式: 5 / 3
    指数表达式: 5 ** 3
    ```
- 打印数学表达式运算结果：
    ```python
    print("加法表达式:", 5 + 3)
    print("减法表达式:", 5 - 3)
    print("乘法表达式:", 5 * 3)
    print("除法表达式:", 5 / 3)
    print("指数表达式:", 5 ** 3)
    ```
    ```python
    # 输出结果为：
    加法表达式: 8
    减法表达式: 2
    乘法表达式: 15
    除法表达式: 1.6666666666666667
    指数表达式: 125
    ```
- 行尾结束符end
*默认情况下，end 参数的值是 '\n'，即换行符。你可以将其更改为其他字符串来指定行尾结束符。*
    ```python
    # 使用感叹号作为行尾结束符
    print("Hello, world!", end='!')

    # 使用问号作为行尾结束符
    print("How are you?", end='?')

    # 使用冒号作为行尾结束符
    print("This is a sentence.", end=':')

    # 使用换行符作为行尾结束符
    print("This is another sentence.")

    # 使用换行符作为行尾结束符
    print("第一行\n第二行\n第三行")

    ```
    ```python
    # 输出结果为：
    Hello, world!!How are you?This is a sentence.:This is another sentence.
    第一行
    第二行
    第三行
    ```
- 分隔符
*如果你想要自定义 print() 函数的分隔符，可以使用 sep 参数。默认情况下，sep 参数的值是一个空格字符 ' '。你可以将其更改为其他字符串来指定不同的分隔符。*
    ```python
    # 使用逗号作为分隔符
    print("苹果", "橙子", "香蕉", sep=',')

    # 使用制表符作为分隔符
    print("狗", "猫", "鸟", sep='\t')

    # 使用冒号和空格作为分隔符
    print("红色", "蓝色", "绿色", sep=': ')

    # 使用自定义字符串作为分隔符
    print("One", "Two", "Three", sep='---')

    # 设置分隔符为逗号，行尾结束符为感叹号
    print("苹果", "橙子", "香蕉", sep=',', end=' ')

    ```
    ```python
    # 输出结果为：
    苹果,橙子,香蕉
    狗	猫	鸟
    红色: 蓝色: 绿色
    One---Two---Three
    苹果,橙子,香蕉!
    ```

### 1.2 变量与运算
Python 中的变量是用来存储数据的标识符。它们可以存储不同类型的值，并且可以在程序中进行引用和操作。
<font color="red">引用变量时，确保该变量已经被定义！</font>
- 变量的命名规则：
1) 变量名只能包含字母、数字和下划线。
2) 变量名不能以数字开头。
3) 变量名区分大小写，例如 count 和 Count 是不同的变量。
4) 避免使用 Python 的关键字（if、while、for）作为变量名。
```python
    # 以下是Python的一些关键字列表：
    False      class      finally    is         return
    None       continue   for        lambda     try
    True       def        from       nonlocal   while
    and        del        global     not        with
    as         elif       if         or         yield
    assert     else       import     pass
    break      except     in         raise
```

- 变量的赋值：
使用赋值运算符 = 可以将值赋给变量。
    ```python
    # 变量赋值
    text = "小张的薪资"
    salary = 8900
    print(text)
    print(salary)
    print("员工：",text,salary)
    ```
    ```python
    # 输出结果为：
    小张的薪资
    8900
    员工： 小张的薪资 8900
    ```
    ```python
    # 变量之间相互赋值
    salary = 8900
    salary_copy=salary
    print(salary_copy)
    ```
    ```python
    # 输出结果为：
    8900
    ```
    ```python
    # 给变量加上引号
    salary_copy= salary
    print('salary_copy')
    ```
    ```python
    # 输出结果为：
    salary_copy
    ```
- 变量的特性
变量每次只能赋值一个值，要赋值另一个值时，当前这个值就会被替换掉。
    ```python
    text=“小张的薪资”
    text=8900
    print(text)
    ```
    ```python
    # 输出结果为：
    8900
    ```
- 巧用变量
    ```python
    # 原message_1和message_2的值
    message_1 ="25岁 男 数据分析师"
    message_2 ="29岁 男 课程设计师"
    print('小张:',message_1)
    print('小李:',message_2)
    ```
    ```python
    # 输出结果为：
    小张: 25岁 男 数据分析师
    小李: 29岁 男 课程设计师
    ```
    ```python
    # 将message_1和message_2中的值互换
    message_1 ="25岁 男 数据分析师"
    message_2 ="29岁 男 课程设计师"
    message_1,message_2 = message_2,message_1
    print('小张:',message_1)
    print('小李:',message_2)
    ```
    ```python
    # 输出结果为：
    小张: 29岁 男 课程设计师
    小李: 25岁 男 数据分析师
    ```
- 数据类型
    - *整数（int）：* 表示整数值，例如 1、2、-3 等。
    - *浮点数（float）* ：表示带有小数部分的数值，例如 3.14、2.71828 等。
    - *字符串（str）：* 表示文本数据，由字符序列组成，使用单引号或双引号括起来，例如 'hello'、"world" 等。
    - *布尔值（bool）：* 表示逻辑值，可以是 True（真）或 False（假），用于条件判断和控制流程。
     - *列表（list）：* 表示一组有序的元素，可以包含不同类型的对象，使用方括号括起来，例如 [1, 2, 3]、['apple', 'banana', 'orange'] 等。
    - *元组（tuple）：* 类似于列表，但是元组是不可变的，即不能修改其元素的值。使用圆括号括起来，例如 (1, 2, 3)、('a', 'b', 'c') 等。
    - *集合（set）：* 表示一组唯一且无序的元素，用于去重和数学运算，使用大括号或 set() 函数创建，例如 {1, 2, 3}、set([4, 5, 6]) 等。
    - *字典（dict）：* 表示键值对的集合，每个元素由一个键和对应的值组成，键是唯一的且不可变，使用大括号或 dict() 函数创建，例如 {'name': 'Alice', 'age': 25}、dict(zip(['a', 'b', 'c'], [1, 2, 3])) 等。
    - *字节串（bytes）：* 表示二进制数据。
    - *字节数组（bytearray）：* 类似于字节串，但是是可变的。
    - *空值（None）：* 表示空对象或缺失值。

- 算术运算符
    - *加减乘除*
        **加法**
        ```python
        # 加法运算：使用加法运算符（+）可以将两个数相加，并返回它们的和。
        a = 5
        b = 3
        c = a + b
        print(c)  # 输出结果 c，即 8

        # 自加运算：自加运算符（+=）结合了加法运算和赋值运算。它将一个变量与另一个值相加，并将结果赋给变量本身。
        a = 5
        b = 3
        a += b  # 等同于 a = a + b
        print(a)  # 输出结果 a，即 8
        ```
        **减法**
        ```python
        # 减法运算：使用减法运算符可以将一个数减去另一个数，并返回它们的差。
        a = 5
        b = 3
        c = a - b
        print(c)  # 输出结果 c，即 2

        # 自减运算：自减运算符（-=）结合了减法运算和赋值运算。它可以将一个变量减去另一个值，并将结果赋给该变量本身。
        a = 5
        b = 3
        a -= b  # 等同于 a = a - b
        print(a)  # 输出结果 a，即 2
        ```

        **乘法**
        ```python
        # a * b 表示将变量 a 的值乘以变量 b 的值，并将结果赋值给变量 c
        a = 5
        b = 3
        c = a * b
        print(c)  # 输出结果 c，即 15
        ```

        **除法**
        ```python
        # 计算小张的日平均新资，8900加100加上2乘1000的总工资，再除以22天
        sa1ary=(8900+100+2*1000)/22
        print(sa1ary) # salary的值为500.0

        a = 10
        b = 3
        # 使用普通除法运算符（/），结果为浮点数
        c = a / b  # c 的值为 3.3333333333333335
        
        # 使用整除运算符（//），结果为整数
        d = a // b  # d 的值为 3

        # 使用取余运算符（%），得到除法的余数
        e = a % b  # e 的值为 1
        ```
        **幂运算**
        ```python
        # 幂运算使用双星号（**）符号执行一个数的指数操作
        a = 2
        b = 3
        c = a ** b
        print(c)  # 输出结果 c，即 8
        ```

### 1.3 输入数据与数据类型
- 输入函数
input()函数是Python中用于从用户获取输入的内置函数。它会显示一个提示信息，并等待用户在控制台输入内容，然后将输入内容作为字符串返回给程序。
```python
# 使用 input() 函数的一般语法如下：
variable = input(prompt)
# 其中，prompt 是一个可选的参数，用于显示给用户的提示信息。用户在控制台输入的内容会被存储在变量 variable 中。

# 用input()函数接收从键盘输入的小张的基本新资
salary = input()
# 运行程序时，弹出一个输入框，输入8900，按下回车
```
```python
# 输出结果为：
8900
```
*jupyter编辑器：input()函数默认输出接收的内容*
*其他编辑器：input()接收的内容须通过print()输出*
```python
name = input("请输入您的名字：")
print("您好，" + name)
# 当运行这段代码时，控制台会显示 "请输入您的名字：" 提示信息，然后等待用户输入名字。用户输入名字后按下回车键，
# 输入内容就会存储在 name 变量中，并打印出类似于 "您好，[用户输入的名字]" 的消息。
```
<span style="color:red;">请注意，在使用 input() 函数时，返回的始终是字符串类型的数据。如果需要将输入的内容转换为其他类型（如整数或浮点数），可以使用相应的类型转换函数，例如 int() 或 float()。</span>

- type()函数
type() 函数是Python中用于获取变量或值的类型信息的内置函数。它返回一个表示对象类型的值，通常是一个内置类型或自定义类的名称。
```python
# 使用 type() 函数的一般语法如下：
type(object)
# 其中，object 是要获取类型的对象或值。
```
```python
x = 10
y = 3.14
z = "Hello"

print(type(x))   # 输出：<class 'int'>
print(type(y))   # 输出：<class 'float'>
print(type(z))   # 输出：<class 'str'>

```
- 类型转换函数
1. int()：用于将一个数值或字符串转换为整数类型。
```python
x = int(3.14)  # x 的值为 3
y = int("5")   # y 的值为 5
```

2. float()：用于将一个数值或字符串转换为浮点数类型。
```python
x = float(3)    # x 的值为 3.0
y = float("5.8")  # y 的值为 5.8
```

3. str()：用于将其他数据类型转换为字符串类型。
```python
x = str(10)       # x 的值为 "10"
y = str(3.14)     # y 的值为 "3.14"
z = str(True)     # z 的值为 "True"
```

- eval() 
函数是Python的内置函数之一，用于将字符串作为表达式进行求值，并返回计算结果。
```python
# eval() 函数的一般语法如下：
eval(expression, globals=None, locals=None)

# 其中，expression 是一个字符串，表示要求值的表达式。
# globals 和 locals 是可选参数，用于指定全局和局部变量的命名空间。
# 如果没有提供这两个参数，则使用当前调用 eval() 函数的命名空间。
```
1. 求值简单的数学表达式：
```python
result = eval("2 + 3 * 4")   # result 的值为 14
```
2. 给定变量，计算表达式的值：
```python
x = 10
y = 5
result = eval("x + y")       # result 的值为 15
```
3. 使用 eval() 处理更复杂的表达式：
```python
expression = "(x + y) * 2"
result = eval(expression)    # result 的值为 30
```
### 1.4 字符串的提取与运算
**索引和切片**
1. 索引
- 字符串的索引从 0 开始，表示第一个字符。负数索引从字符串的末尾开始，表示倒数第一个字符。
- 使用方括号 [ ] 加上索引来访问特定位置的字符。
- 如果索引超出字符串的范围，将引发 IndexError 错误。

```python
# 提取学符串“李玲 女 班主任”中的性别“女“这个学符
string = "李玲 女 班主任"

print(string[3])     # Output: 女
```
|  访问字符 |  李 | 玲  | ' '  | 女  | ' '  | 班  | 主  | 任  |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
| 正向索引  |  0 |  1 |  2 |  3 | 4  |  5 |  6 | 7  |
| 反向索引  |  -8 |  -7 | -6  |  -5 | -4  | -3  |  -2 | -1  |
2. 切片
- 切片允许您提取字符串的一部分。它使用冒号 : 分隔起始索引和结束索引。
- 切片时包含起始索引对应的字符，但不包含结束索引对应的字符。
- 如果不指定起始索引，默认为字符串的开头；如果不指定结束索引，默认为字符串的末尾。
- 可以使用负数索引进行切片。
切片的基本格式是在方括号中使用起始索引、结束索引和可选的步长来提取字符串的子串。下面是切片操作的基本格式：
`string[start:end:step]`
start：起始索引，表示切片的开始位置。
end：结束索引，表示切片的结束位置（不包含在切片结果中）。
step：可选参数，表示切片的步长，默认为 1。
<span style="color:red;"> 需要注意的是，切片时包含起始索引对应的字符，但不包含结束索引对应的字符。</span>

```python
# 同时指定多个连续的索引值，来访问多个连续的字符
string = "李玲 女 班主任"

print(string[0:4])     # Output: 李玲 女
```

```python
# 使用反向索引
string = "李玲 女 班主任"

print(string[-8:-6])     # Output: 李玲
```
<span style="color:red;">需要注意的是，索引和切片操作返回的结果仍然是字符串</span>

- 在切片操作中，如果省略了起始索引或者结束索引，Python 会自动使用默认值：
如果省略了起始索引，则默认起始索引为字符串的开头（索引0）。
如果省略了结束索引，则默认结束索引为字符串的末尾（最后一个字符的后面）。
```python 
string = "李玲 女 班主任"

print(string[:4])     # Output: 李玲 女
print(string[5:])     # Output: 班主任
```
**len()函数**
len() 函数是Python内置函数之一，用于返回一个对象（如字符串、列表、元组等）的长度或元素个数。
```python
string = "Hello, World!"
length = len(string)
print(length)   # Output: 13
```

**字符串运算**
1. 字符串连接：可以使用 + 运算符将两个字符串连接起来。
```python
str1 = "Hello"
str2 = "World"
result = str1 + ", " + str2
print(result)   # Output: Hello, World
```

2. 重复字符串：可以使用 * 运算符将一个字符串重复多次。
```python
str1 = "Hello"
result = str1 * 3
print(result)   # Output: HelloHelloHello
```

3. 获取字符串长度：可以使用 len() 函数获取字符串的长度。
```python
string = "Hello, World!"
length = len(string)
print(length)   # Output: 13
```

4. 切片操作：可以使用切片操作提取字符串的子串。
```python
string = "Hello, World!"
sub_string = string[7:12]
print(sub_string)   # Output: World
```

5. 字符串格式化：可以使用字符串的 format() 方法或者f-string来进行字符串的格式化。
```python
name = "Alice"
age = 25
result = "My name is {} and I am {} years old.".format(name, age)
print(result)   # Output: My name is Alice and I am 25 years old.

# 或者使用 f-string 格式化字符串
result = f"My name is {name} and I am {age} years old."
print(result)   # Output: My name is Alice and I am 25 years old.
```

**in 成员运算符**
in 是一个成员运算符，用于检查一个值是否存在于某个集合（如字符串、列表、元组、集合或字典）中。它返回一个布尔值，如果值存在于集合中，则返回 True，否则返回 False。
*检查字符串中的字符是否存在：*
```python
string = "Hello, World!"
print("H" in string)    # Output: True
print("x" in string)    # Output: False
```
**not in** 是成员运算符的一个变种，与 in 相反。它用于检查一个值是否不存在于某个集合（如字符串、列表、元组、集合或字典）中。它返回一个布尔值，如果值不存在于集合中，则返回 True，否则返回 False。
*检查字符串中的字符是否不存在：*
```python
string = "Hello, World!"
print("H" not in string)     # Output: False
print("x" not in string)     # Output: True
```
### 1.5 字符串常用方法
- 字符串格式化
字符串格式化是指在输出或拼接字符串时，根据一定的格式规则将变量或表达式的值插入到字符串中的特定位置。
在Python中，字符串格式化有多种方式，以下是其中几种常用的方法：
1. 使用占位符：可以使用占位符（例如%s、%d等）来表示要插入的值的类型，并将变量或表达式作为参数传递给字符串的%操作符。
```python 
name = "Alice"
age = 25
message = "My name is %s and I'm %d years old." % (name, age)
print(message)
```
```python 
# 输出结果：
My name is Alice and I'm 25 years old.
```
2. 使用format方法：可以使用字符串的format方法，通过花括号{}和位置索引或关键字来指定插入的值。
```python 
name = "Bob"
age = 30
message = "My name is {} and I'm {} years old.".format(name, age)
print(message)
```
```python 
# 输出结果：
My name is Bob and I'm 30 years old.
```
```python
# 通过在花括号 {} 内添加索引号来指定要插入的变量的顺序
name = "Alice"
age = 25
country = "China"

print("My name is {1}, I am {0} years old, and I am from {2}.".format(age, name, country))
# Output: My name is Alice, I am 25 years old, and I am from China.
```
```python
# 通过在花括号 {} 内添加格式说明符来指定值的格式
# 以下是一些常用的格式说明符示例：
# {:d}：整数类型
# {:f}：浮点数类型
# {:s}：字符串类型
# {:x}：十六进制整数类型
# {:b}：二进制整数类型
num = 42
pi = 3.1415926
name = "Alice"

print("My number is {:d}".format(num))
# Output: My number is 42

print("The value of pi is {:.2f}".format(pi))
# Output: The value of pi is 3.14

print("Hello, {}!".format(name))
# Output: Hello, Alice!

# {:d} 表示整数类型，{:.2f} 表示浮点数类型并保留两位小数，{:s} 表示字符串类型。
```
```python
num = 42

print("My number is {:>5}".format(num))
# Output: My number is    42

print("My number is {:0>5}".format(num))
# Output: My number is 00042

# {:>5} 表示向右对齐，并使用空格填充到宽度为 5，{:0>5} 表示向右对齐，并使用零填充到宽度为 5。
```
3. 使用f-string（格式化字符串字面值）：在Python 3.6及以上版本中，可以使用以f开头的字符串，在其中直接嵌入变量或表达式，并使用花括号{}来表示插入点。
```python
name = "Charlie"
age = 35
message = f"My name is {name} and I'm {age} years old."
print(message)
```
```python
# 输出结果：
My name is Charlie and I'm 35 years old.
```
- replace() 函数
replace() 函数是字符串的内置方法，用于替换字符串中的子字符串。它接受两个参数：旧子字符串和新子字符串，并返回一个替换后的新字符串。
以下是 replace() 函数的语法：
*original_string：原始的字符串，需要被替换的字符串。*
*old_str：需要被替换的子字符串。*
*new_str：用于替换的新子字符串。*
*new_string：替换后的新字符串。*
`new_string = original_string.replace(old_str, new_str)`
```python
# 将原始字符串 text 中的所有 "Hello" 替换为 "Hi"，并将结果存储在 new_text 中。
text = "Hello, World! Hello, Python!"
new_text = text.replace("Hello", "Hi")

print(new_text)
# Output: Hi, World! Hi, Python!
```
<span style="color:red;">需要注意的是，replace() 方法返回的是一个新的字符串，原始字符串不会受到影响。另外，replace() 方法是区分大小写的，如果要进行大小写不敏感的替换，可以先使用 .lower() 或 .upper() 方法转换大小写。</span>

```python
# 先将字符串转换为小写，然后再进行替换。
text = "Hello, World! hello, python!"
new_text = text.lower().replace("hello", "Hi")

print(new_text)
# Output: hi, world! hi, python!
```
- split() 函数
split() 函数是字符串的内置方法，用于将一个字符串拆分成多个子字符串，并以列表的形式返回这些子字符串。
以下是 split() 函数的语法：
*original_string：原始的字符串，需要被拆分的字符串。*
*separator：可选参数，用于指定拆分字符串的分隔符，默认为空白字符（空格、制表符、换行符等）。*
`string_list = original_string.split(separator)`
```python
# 使用 split() 方法将字符串 text 拆分成多个子字符串，并将结果存储在列表中
text = "Hello, World! This is Python."

# 使用空格作为分隔符拆分字符串
words = text.split()

print(words)
# Output: ['Hello,', 'World!', 'This', 'is', 'Python.']


# 使用逗号作为分隔符拆分字符串
phrases = text.split(',')

print(phrases)
# Output: ['Hello', ' World! This is Python.']
```
```python
# 通过指定 maxsplit 参数来限制拆分的次数
text = "one two three four five"

# 拆分字符串，最多拆分两次
words = text.split(maxsplit=2)

print(words)
# Output: ['one', 'two', 'three four five']
```
### 1.6 分岔路口
- if分支结构
    - if单分支结构
    if 单分支结构是 if 条件语句的一种形式，它只包含一个 if 语句，用于在给定条件为真时执行相应的代码块。
    以下是 if 单分支结构的基本语法：
    ```python
    if condition:
        # 如果条件为真，则执行这里的代码
    ```
    在单分支结构中，condition 是一个表达式或值，用于判断条件是否成立。如果条件成立（即为真），则执行代码块；如果条件不成立（即为假），则跳过代码块。
    ```python
    # 根据条件判断年龄是否大于等于 18 岁。如果年龄大于等于 18 岁，则打印一条消息。
    age = 25

    if age >= 18:
        print("您已经成年，可以参加选举。")

    ```
    
    ```mermaid
    graph LR
    st((开始))
    input[输入变量X]
    cond{X > 0?}
    op[执行操作]
    out[输出结果]
    e((结束))

    st --> input
    input --> cond
    cond -- 是 --> op
    op --> out
    out --> e
    cond -- 否 --> e
    ```
    *比较运算符*
    <style>
    table {
        border-collapse: collapse;
        width: 100%;
    }
    th {
        background-color: lightblue;
        color: white;
        font-weight: bold;
        padding: 8px;
        text-align: left;
    }
    td {
        padding: 8px;
        border: 1px solid #ddd;
    }
    </style>

    <table>
    <tr>
        <th>运算符</th>
        <th>描述</th>
        <th>示例</th>
        <th>结果</th>
    </tr>
    <tr>
        <td>==</td>
        <td>等于</td>
        <td>5 == 5</td>
        <td>True</td>
    </tr>
    <tr>
        <td>!=</td>
        <td>不等于</td>
        <td>5 != 3</td>
        <td>True</td>
    </tr>
    <tr>
        <td>&gt;</td>
        <td>大于</td>
        <td>7 &gt; 3</td>
        <td>True</td>
    </tr>
    <tr>
        <td>&lt;</td>
        <td>小于</td>
        <td>2 &lt; 4</td>
        <td>True</td>
    </tr>
    <tr>
        <td>&gt;=</td>
        <td>大于等于</td>
        <td>6 &gt;= 6</td>
        <td>True</td>
    </tr>
    <tr>
        <td>&lt;=</td>
        <td>小于等于</td>
        <td>4 &lt;= 3</td>
        <td>False</td>
    </tr>
    </table>

    <span style="color:red;">注：=表示赋值符号，==表示等于符号</span>
    
    - if双分支结构
    if双分支结构是一种常见的编程控制结构，用于在程序中根据条件执行不同的操作。它基于一个条件表达式，如果条件为真，则执行一个代码块（通常称为"if块"或"if分支"），如果条件为假，则执行另一个代码块（通常称为"else块"或"else分支"）。
    以下是描述if双分支结构的一般形式：
    ```python
    if 条件:
        # 如果条件为真，则执行这个代码块
        执行操作1
    else:
        # 如果条件为假，则执行这个代码块
        执行操作2
    ```
    在 if 双分支结构中，首先判断条件的真假。如果条件为真，则执行代码块中的操作1；如果条件为假，则跳过代码块中的操作1，执行 else 块中的操作2。
    ```python
    # 如果成绩大于等于90，条件score >= 90为真，那么程序将执行if块中的操作，即打印出"优秀"。
    # 如果条件为假，即成绩小于90，那么程序将跳过if块，执行else块中的操作，即打印出"良好"。
    score = float(input("请输入您的成绩: "))

    if score >= 90:
        print("优秀")
    else:
        print("良好")
    ```
    ```mermaid
    graph LR
        st((开始))
        input[输入变量X]
        cond{X > 0?}
        op1[执行操作1]
        op2[执行操作2]
        out[输出结果]
        e((结束))

        st --> input
        input --> cond
        cond -- 是 --> op1
        op1 --> out
        out --> e
        cond -- 否 --> op2
        op2 --> out
        out --> e
    ```
    - if elif..多分支结构
    if-elif-else结构可以处理多个条件，并根据条件的判断结果选择相应的代码块执行。
    以下是描述if-elif-else多分支结构的一般形式：
    ```python
    if 条件1:
        # 如果条件1为真，则执行这个代码块
        执行操作1
    elif 条件2:
        # 如果条件1为假而条件2为真，则执行这个代码块
        执行操作2
    elif 条件3:
        # 如果条件1和条件2都为假而条件3为真，则执行这个代码块
        执行操作3
    ...
    else:
        # 如果所有条件都为假，则执行这个代码块
        执行默认操作
    ```
    在if-elif-else结构中，首先根据条件1的判断结果来确定是否执行操作1。如果条件1为真，则执行操作1，并跳过后续的elif和else块；如果条件1为假，则继续检查条件2，如果条件2为真，则执行操作2，并跳过后续的elif和else块；以此类推，直到找到第一个为真的条件，并执行相应的操作；如果所有条件都为假，则执行else块中的操作，作为默认操作。
    ```python
    score = float(input("请输入您的成绩: "))

    if score >= 90:
        print("优秀")
    elif score >= 80:
        print("良好")
    elif score >= 60:
        print("及格")
    else:
        print("不及格")
    ```
    ```mermaid
    graph LR
    st((开始))
    cond1{判断条件1是否为真?}
    cond2{判断条件2是否为真?}
    cond3{判断条件3是否为真?}
    op1[执行操作1]
    op2[执行操作2]
    op3[执行操作3]
    default[执行默认操作]
    e((结束))

    st --> cond1
    cond1 -- 是 --> op1 --> e
    cond1 -- 否 --> cond2
    cond2 -- 是 --> op2 --> e
    cond2 -- 否 --> cond3
    cond3 -- 是 --> op3 --> e
    cond3 -- 否 --> default --> e
    ```
- 分支结构嵌套
分支嵌套是指在一个分支结构中嵌套另一个分支结构，以实现更复杂的条件判断和操作执行。以下是一个展示分支嵌套结果的示例：
```python
score = float(input("请输入您的成绩: "))

if score >= 60:
    if score >= 90:
        print("优秀")
    elif score >= 80:
        print("良好")
    else:
        print("及格")
else:
    print("不及格")
```
在这个示例中，首先程序会要求用户输入一个成绩，并将其保存在变量 score 中。

接下来，程序使用外部的 if 结构进行整体判断，即判断是否达到及格分数线（60 分）。如果满足外部的条件，程序将进入外部的 if 块。

在外部的 if 块中，又嵌套了一个内部的 if-elif-else 结构。在内部结构中，首先判断是否达到优秀分数线（90 分），如果是，则打印出"优秀"；如果不是，则继续判断是否达到良好分数线（80 分），如果是，则打印出"良好"；如果也不是，则执行内部结构的 else 块，打印出"及格"。

如果外部的 if 结构中的条件判断为假，即成绩低于及格分数线，那么程序将跳过外部的 if 块，直接执行外部结构的 else 块，打印出"不及格"。

- 逻辑运算符
逻辑运算符用于在条件判断中组合多个条件，并根据这些条件的逻辑关系得出最终的判断结果。在Python中，常用的逻辑运算符包括以下三个：
1. 与运算符（and）：如果两个条件都为真，则返回真；否则返回假。
2. 或运算符（or）：如果两个条件中至少有一个为真，则返回真；否则返回假。
3. 非运算符（not）：如果条件为真，则返回假；如果条件为假，则返回真。
以下是逻辑运算符的使用示例：
```python
x = 5
y = 10

# 与运算符示例
if x > 0 and y > 0:
    print("x和y都大于0")

# 或运算符示例
if x > 0 or y > 0:
    print("x或者y大于0")

# 非运算符示例
if not x > 0:
    print("x不大于0")
```

### 1.7 有限次的for循环


### 1.8 不限次的while循环
### 1.9 数据结构-列表
### 1.10 数据结构-字典
### 1.11 数据结构-元组和集合
### 1.12 精简代码利器-函数
### 1.13 玩转文件
### 1.14 精简代码神器-模块
### 1.15 项目实战

## 2. Python自动化办公
*主要解决Excel和word处理数据效率低以及步骤繁杂的问题。*
### 2.1 用Python高效处理Excel
### 2.2 快速拆分工作表
### 2.3 Excel案例课
### 2.4 会议照片汇总与批量制作报销单
### 2.5 制作通知单
### 2.6 生成算术试题
### 2.7 批量生成邀请函和合同
### 2.8 整合报销单

## 3. Python数据处理
*主要解决数据杂乱、缺失、重复的问题。*
### 3.1 数据处理
### 3.2 数据筛选
### 3.3 数据清洗
### 3.4 数据填充
### 3.5 数据汇总
### 3.6 统计分析
### 3.7 综合应用(一)
### 3.8 综合应用(二)

## 4. Python可视化
*主要解决制作动态、具有交互能力的图表。*
### 4.1 走进数据可视化的世界
### 4.2 简单图形展示复杂数据
### 4.3 数据的美化工作
### 4.4 用文字说明核心问题
### 4.5 专业问题专业图形
### 4.6 组合图形展示多方面观点
### 4.7 数据可视化的高阶殿堂
### 4.8 简洁专业的基本图形
### 4.9 展示出数据的风格
### 4.10 复杂问题分解展示

## 5. Python爬虫
*主要解决数据来源不足的问题。*
### 5.1 爬虫知识准备
### 5.2 利用urllib爬取古诗文网
### 5.3 利用requests快捷爬取京东商品
### 5.4 利用好看视频网站学习isonpath
### 5.5 利用xpath提取百度贴吧网页信息
### 5.6 爬取动态小说网站
