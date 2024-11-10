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


## #24 Different types of bytes

Basics: What is MB and GB?

	1.	MB (Megabyte):
	•	A Megabyte (MB) is like a medium-sized box that can hold a good amount of data.
	•	It’s usually big enough for things like a short song or a picture.
	2.	GB (Gigabyte):
	•	A Gigabyte (GB) is like a much bigger box. It can hold more than 1,000 MB boxes!
	•	With 1 GB, you could store hundreds of songs or several hundred pictures. For example, a small movie might be around 1 GB.

How Do They Work?

	•	Computers have storage to keep information (like games, music, and videos), and they use MB and GB to measure how much they can store.
	•	The more MB or GB a device has, the more data it can hold.

Are There More Types?

Yes! Computers use even bigger boxes when they need to store a lot more data. Here are some other sizes:
	1.	KB (Kilobyte):
	•	A Kilobyte (KB) is smaller than an MB. Think of it as a tiny box.
	•	It might only hold a few words of text, like a sentence or two.
	2.	TB (Terabyte):
	•	A Terabyte (TB) is a giant box! It can hold 1,000 GB.
	•	You’d use this if you wanted to store a huge collection of games, videos, or pictures.
	3.	PB (Petabyte):
	•	A Petabyte (PB) is like an enormous storage warehouse that holds 1,000 TB!
	•	Companies or data centers use petabytes to store tons of information.

Quick Summary

	•	KB (Kilobyte) – tiny box, holds text or small data.
	•	MB (Megabyte) – medium box, holds a picture or a short song.
	•	GB (Gigabyte) – big box, holds many songs, pictures, or a small movie.
	•	TB (Terabyte) – very big box, holds a huge collection of videos or games.
	•	PB (Petabyte) – massive warehouse, used for companies that store tons of data.

So, think of MB, GB, and the others as different-sized boxes that help us measure how much stuff we can fit in our devices! The bigger the box (like GB or TB), the more fun things we can store.

--- 
## #25 Inside a PC

Inside a desktop PC, there are several important components that work together to make the computer run. Here’s a look at the main parts and what they do:

1. Motherboard

	•	Description: This is like the “central hub” of the computer. All other components connect to the motherboard, allowing them to communicate.
	•	Function: It holds the CPU, RAM, and other key components and connects everything with circuits (like roads) so data can travel between them.

2. CPU (Central Processing Unit)

	•	Description: Often called the “brain” of the computer.
	•	Function: The CPU processes instructions and performs calculations to run programs. It handles everything from opening a file to running games.

3. RAM (Random Access Memory)

	•	Description: This is your computer’s short-term memory.
	•	Function: RAM temporarily holds data and instructions that the CPU needs while the computer is on. For example, when you’re playing a game, it keeps important game data in RAM so the CPU can access it quickly. When you turn off your computer, everything in RAM is erased.

4. Storage Drive (HDD or SSD)

	•	HDD (Hard Disk Drive): Uses spinning disks to store data. It’s slower but can hold a lot of data.
	•	SSD (Solid State Drive): Uses memory chips to store data. It’s faster and more reliable, but usually more expensive than HDDs.
	•	Function: This is where all your files, programs, and operating system are stored. Unlike RAM, the data here isn’t erased when you turn off your computer.

5. Power Supply Unit (PSU)

	•	Description: This is the “power source” for the computer.
	•	Function: The PSU takes power from the outlet and converts it to the type and amount of power needed by each component in the computer. It ensures each part gets enough energy to run.

6. GPU (Graphics Processing Unit)

	•	Description: Also called a graphics card, this handles the display of images and video.
	•	Function: The GPU is designed to process complex graphics calculations quickly, making it essential for gaming, video editing, and other visually intensive tasks.

7. Cooling System (Fans, Heatsinks, and Sometimes Liquid Cooling)

	•	Description: Computers generate heat, especially the CPU and GPU.
	•	Function: The cooling system keeps the computer’s components from overheating. Fans and heatsinks pull heat away, and some high-performance computers use liquid cooling for even better temperature control.

8. Case

	•	Description: The case is the physical box that holds and protects all the internal components.
	•	Function: It keeps everything in place and provides space for airflow, which helps with cooling.

Summary of Main Parts

	•	Motherboard: Central hub connecting all parts.
	•	CPU: Brain of the computer, handles processing.
	•	RAM: Short-term memory for active tasks.
	•	Storage Drive: Long-term storage for files and programs.
	•	Power Supply (PSU): Provides power to all components.
	•	GPU: Handles graphics and video processing.
	•	Cooling System: Keeps parts from overheating.
	•	Case: Protects and organizes everything.

These parts all work together, allowing you to run applications, store files, and use your computer smoothly!

--- 
## #26 APP/Application

An application (or “app”) is a program you use on your computer, tablet, or phone to do specific tasks. For example, there are apps for games, drawing, sending messages, or even doing homework.

What is an Application?

	•	Think of an application like a tool or a toy. Just like a hammer is a tool to build things, and a toy is something you play with, an application is a program you use to do things on your device.
	•	For example:
	•	Game app: lets you play a game.
	•	Drawing app: lets you create pictures.
	•	Calculator app: helps you solve math problems.

Where Does the Term “Application” Come From?

The word application originally means “to apply” something, like when you apply paint to a wall or when you apply an idea in real life.

In computers, “application” means applying the computer’s power to do something useful for you, like writing, drawing, or playing games. That’s why we call these programs “applications” – because we’re “applying” the computer to do different tasks.

So, in Summary:

	•	An application is a program that lets you do a specific task on your device.
	•	The word “application” means “using something for a purpose,” and in computers, it means using the device’s power to help you with a task, like messaging, gaming, or drawing.

---
## #27 Back-end/Front-End
In the world of computers and websites, front-end and back-end are like two different parts of a team that work together to make a website or app function.

What is the Front-End?

	•	The front-end is the part of a website or app that you can see and interact with. It’s the “user-facing” side – like the graphics, buttons, text, and images you see on the screen.
	•	Think of it as the stage at a play: you see the actors, props, and scenery. Everything the audience (you) sees is like the front-end of a website.
	•	Examples:
	•	When you click a button, type in a search bar, or scroll through images, you’re using the front-end of a website.
	•	Front-end programming languages include HTML, CSS, and JavaScript – these help design and style what you see on a webpage.

What is the Back-End?

	•	The back-end is like the behind-the-scenes part of a website or app. It’s everything you don’t see but is crucial for making the website work, like servers, databases, and code that manage data.
	•	Think of it as backstage at a play: it includes the crew, directors, and scripts that make the performance happen. They’re not seen, but they make sure everything on stage runs smoothly.
	•	Examples:
	•	When you log into your account on a website, the back-end checks your username and password.
	•	Back-end programming languages include Python, Ruby, Java, and SQL – they help manage data, run logic, and communicate with the front-end.

Summary

	•	Front-End: The visible part you interact with – like the stage of a play. It’s designed with HTML, CSS, and JavaScript.
	•	Back-End: The invisible part that powers the website – like the crew backstage making sure everything runs smoothly. It’s created with languages like Python and Java.

Together, the front-end and back-end make a website work, just like the actors and crew work together to put on a successful play!

---
## #28 JavaScript vs Python

从前端和后端的角度来看，JavaScript 和 Python 的用途和特点有很大差异。下面是它们在前端和后端的不同之处：

前端

	•	JavaScript
JavaScript 是前端开发的核心语言，用于让网页更加动态和互动。几乎所有现代网页都依赖 JavaScript 来处理用户的操作，比如点击按钮、弹出窗口、显示动画等。它能让网页立即响应用户的输入，不需要重新加载整个页面。像 React、Vue 和 Angular 这样的框架让 JavaScript 开发更便捷，适合制作现代化、复杂的用户界面。
	•	Python
Python 在前端的使用非常少。虽然它的语法简单，但不适合直接在网页浏览器上运行，因为浏览器不支持直接运行 Python。Python 更适合在后台处理数据，再通过 API 传送到前端展示。实际上，Python 的前端应用主要限于数据可视化和一些简单的网页制作，不像 JavaScript 那样能实现全面的网页互动。

后端

	•	JavaScript (Node.js)
JavaScript 通过 Node.js 也可以在后端运行。Node.js 让 JavaScript 可以处理服务器上的任务，比如接收用户请求、读取数据库、处理数据等。Node.js 非常适合处理大量请求，比如聊天应用或实时数据更新的情况，因为它的异步处理可以同时进行多个任务，而不会被卡住。Express.js 是常用的 Node.js 框架，帮助快速构建服务器和 API。
	•	Python
Python 在后端非常受欢迎，适合开发服务器、处理数据、分析信息等。Python 的框架（如 Django 和 Flask）让它能够轻松创建强大的后端服务。Python 的语法简单，适合构建需要复杂逻辑的应用，比如数据分析平台或机器学习系统。它处理高计算量的任务更有效，适合需要科学计算的应用。Python 在 AI 和数据科学领域的库（如 TensorFlow、Pandas）让它在后端计算上具备强大优势。

总结

	•	前端：JavaScript 是前端的主力，负责网页的动态和互动。Python 几乎不用于前端。
	•	后端：JavaScript 和 Python 都能用于后端，但适合不同的应用场景。JavaScript 适合高并发、实时性强的应用，而 Python 则适合数据处理、分析和 AI 相关的应用。

选择 JavaScript 还是 Python，取决于你在前端还是后端工作，以及你需要的具体功能。


Micro:Bit 支持 JavaScript 和 Python 的原因在于这两种语言的特点和它们在教育中的优势。Micro:Bit 是一个面向教育的微型开发板，专为学生和编程初学者设计。支持这两种语言有以下几个主要原因：

1. JavaScript 和 Python 易于学习且流行

	•	JavaScript 和 Python 都是语法简单、学习曲线较平缓的编程语言，非常适合初学者学习编程基础。
	•	这两种语言都是广泛应用的主流语言，掌握它们对学生未来学习更复杂的编程和技术非常有帮助。让学生在 Micro:Bit 上接触 JavaScript 和 Python，可以让他们学到真实世界中使用的编程知识。

2. 两种语言有不同的优势

	•	JavaScript：适合网页和前端开发。因为许多学生未来可能会接触网页开发，JavaScript 是网页编程的核心语言之一，Micro:Bit 支持 JavaScript 让学生更容易过渡到网页开发。
	•	Python：适合数据处理、科学计算和嵌入式开发，语法简单、结构清晰，非常适合用来编写小型的嵌入式程序。Python 也广泛应用于数据科学和人工智能领域，Micro:Bit 支持 Python 可以激发学生对这些领域的兴趣。

3. 扩大教育覆盖面和选择性

	•	许多学生和老师可能对某一种语言更熟悉或更偏好。Micro:Bit 提供了这两种语言支持，能够让更多人根据自己的需求和兴趣选择合适的编程语言。
	•	通过支持 JavaScript 和 Python，Micro:Bit 平台能够覆盖不同的教育需求和编程课程。比如，某些学校的课程可能更偏向网页开发，这时可以用 JavaScript，而其他课程可能更注重数据或简单嵌入式编程，则可以选择 Python。

4. 推动创造性项目开发

	•	JavaScript 和 Python 都有丰富的资源和库。支持这两种语言可以让学生在 Micro:Bit 上编写更复杂、更有趣的应用，借助已有的 JavaScript 和 Python 社区资源，学生可以开发出更丰富的项目。

5. 跨平台应用的能力

	•	JavaScript 和 Python 的跨平台性使得学生编写的代码更容易移植到其他系统上，比如从 Micro:Bit 转移到桌面应用或其他硬件平台。Python 的代码可以直接用于其他嵌入式系统，而 JavaScript 的技能也有助于学习 Web 技术。

总结

Micro:Bit 支持 JavaScript 和 Python 是为了让编程学习变得更简单和灵活，并且让学生有机会接触到不同的编程语言、为未来的学习打下基础。这种多语言支持能够适应不同教育需求，帮助学生更好地理解编程的概念并激发他们的创造力。


## #29 


