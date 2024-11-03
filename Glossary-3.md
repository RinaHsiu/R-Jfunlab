## #21 命名规范(Sanke, Pascal)

在 Python 编程中，命名规范是指如何为变量、函数、类和其他标识符命名，使代码更具可读性和一致性。Python 通常推荐使用 PEP 8 作为其命名规范的指南。

常见的命名风格

Python 中使用的命名风格包括 Snake Case 和 Pascal Case 等，其他风格如 Camel Case 和 Kebab Case 也在其他编程语言中使用，但在 Python 中不常用。

### 1. Snake Case（蛇形命名法）

	•	格式：单词之间使用下划线连接，所有字母小写。
	•	使用场景：Python 中，变量名和函数名常用这种风格。
	•	示例：

user_name = "John"   # 变量
def calculate_sum(): # 函数
    pass



### 2. Camel Case（驼峰命名法）

	•	格式：第一个单词首字母小写，后续单词的首字母大写。
	•	使用场景：Camel Case 通常用于 JavaScript 等其他编程语言中的变量名和函数名，但在 Python 中不推荐。
	•	示例：

userName = "Alice"  # 不常用于 Python



### 3. Pascal Case（帕斯卡命名法）

	•	格式：每个单词的首字母大写，没有分隔符。
	•	使用场景：在 Python 中，类名通常使用 Pascal Case。
	•	示例：

class UserProfile:
    pass



### 4. Kebab Case（烤串命名法）

	•	格式：单词之间用连字符 - 连接，所有字母小写。
	•	使用场景：这种风格不用于 Python，因为连字符在 Python 中会被解释为减号。
	•	示例：

user-name = "Invalid in Python"  # 不用于 Python



Python 中的命名规范总结

	•	变量和函数：使用 Snake Case，例如 my_variable，calculate_sum()。
	•	类：使用 Pascal Case，例如 MyClass，UserProfile。
	•	常量：使用全大写字母和下划线，例如 MAX_VALUE，PI。

其他注意事项

	•	可读性：命名应尽量清晰明了，表达出变量、函数或类的用途。
	•	避免保留字：不要使用 Python 关键字（如 class、def、import）作为命名。
	•	缩写和拼写：尽量避免使用难懂的缩写和拼写错误，保持名称具有可读性。

示例代码
```

# 变量和函数 - Snake Case
user_age = 25
def get_user_info():
    return "User information"

# 类 - Pascal Case
class UserProfile:
    def __init__(self, name, age):
        self.name = name
        self.age = age

# 常量
MAX_USERS = 100
```

遵循 Python 的命名规范有助于提高代码的可读性和可维护性，尤其在团队合作和共享代码时更为重要。

---

## #22 Variables 变量

在编程中，变量（Variables） 就像是盒子，你可以把东西（数据）放进去，然后给盒子贴上一个名字，这样你就知道在哪里找到它。

什么是变量？

变量是用来存储信息的名字。想象你有一个盒子，里面放着你最喜欢的玩具。你给盒子贴上“我的玩具”的标签，这样你每次看到这个标签，就知道这是装玩具的盒子。在编程中，变量也是这样的——它们用来存储数字、文字、甚至图片等信息。

在 Python 中怎么使用变量？

```
在 Python 中，你可以很容易地创建一个变量并给它赋值。比如：

age = 11  # 变量叫 `age`，存储了数字 11
name = "Rina"  # 变量叫 `name`，存储了名字 "Rina"
```

变量的特点

	•	名字：每个变量都有一个名字，就像盒子上的标签。
	•	值：变量里面的内容，可以是数字、文字或其他信息。
	•	可变：你可以改变变量里面的内容，就像可以把旧玩具从盒子里拿出来，放进新玩具。

变量是如何工作的？

当你在编写程序时，你可以用变量来存储数据并用它们做事情。比如，如果你想打印出一个问候语：
```
name = "Rina"
print("Hello, " + name)  # 打印出 "Hello, Rina"

例子解释

想象一下，你有一个用来记录你今天捡到的石头数量的变量：

stones_collected = 5  # 你今天捡到了 5 颗石头

如果你下午又捡到 2 颗石头，你可以更新变量：

stones_collected = stones_collected + 2  # 现在总共是 7 颗石头
```

为什么变量有用？

变量让程序能够记住信息并使用它。比如，在游戏中，变量可以用来记分；在计算中，变量可以帮助存储计算结果。

总结

	•	变量是一个用来存储数据的“盒子”。
	•	你可以给这个“盒子”取名字，并放入不同的内容。
	•	变量让你的程序更强大，因为它能记住和使用数据。

通过使用变量，你可以编写更有趣、更复杂的程序！

---



## #23 Python Keywords 关键字
Python 关键字（Keywords） 是 Python 编程语言中已经被预先定义好的、具有特定含义的单词。它们是 Python 语法的一部分，不能用作变量、函数或类的名字。关键字用来表示特定的功能或控制结构，例如条件判断、循环和定义函数。

为什么关键字很重要？

关键字是 Python 解释器用来识别程序结构的基础部分。它们有助于告诉 Python 该如何运行代码。
```
Python 中的常见关键字及解释

	1.	if / else / elif：
	•	用于条件判断，if 表示“如果”，else 表示“否则”，elif 是“else if”的缩写，表示“否则如果”。

if age > 10:
    print("You are older than 10")
elif age == 10:
    print("You are 10 years old")
else:
    print("You are younger than 10")


	2.	for / while：
	•	用于循环，for 用来遍历一个序列，while 用来在某个条件为真时重复执行代码。

for i in range(5):
    print(i)  # 输出 0 到 4

count = 0
while count < 5:
    print(count)
    count += 1  # 输出 0 到 4


	3.	def：
	•	用来定义函数。

def greet(name):
    print("Hello, " + name)


	4.	return：
	•	用于函数返回值。

def add(a, b):
    return a + b


	5.	class：
	•	用于定义类，类是创建对象的模板。

class Dog:
    def __init__(self, name):
        self.name = name


	6.	import：
	•	用于导入模块或库，让你可以使用模块中的功能。

import math
print(math.sqrt(16))  # 输出 4.0


	7.	try / except：
	•	用于捕获和处理异常或错误。

try:
    result = 10 / 0
except ZeroDivisionError:
    print("You can't divide by zero!")


	8.	True / False：
	•	表示布尔值 真 和 假，用于逻辑判断。

is_adult = True
if is_adult:
    print("You are an adult")


	9.	None：
	•	表示空值或“什么都没有”。

value = None
if value is None:
    print("Value is None")


	10.	and / or / not：
	•	用于逻辑运算。and 表示“与”，or 表示“或”，not 表示“非”。

if age > 10 and age < 18:
    print("You are a teenager")



如何查看 Python 关键字？

你可以在 Python 中使用以下方法查看所有关键字：

import keyword
print(keyword.kwlist)

```
总结

	•	Python 关键字 是 Python 编程中保留的、不能用作变量或标识符的词。
	•	它们定义了 Python 语言的结构和行为，如控制结构、逻辑判断、函数定义等。
	•	熟悉 Python 关键字有助于编写清晰、有效的代码。
