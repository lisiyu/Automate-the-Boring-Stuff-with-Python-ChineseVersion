#Chapter 1 – Python Basics
#第一章—— Python基础

##Python Basics
##Python基础
The Python programming language has a wide range of syntactical constructions, standard library functions, and interactive development environment features. Fortunately, you can ignore most of that; you just need to learn enough to write some handy little programs.
You will, however, have to learn some basic programming concepts before you can do anything. Like a wizard-in-training, you might think these concepts seem arcane and tedious, but with some knowledge and practice, you’ll be able to command your computer like a magic wand to perform incredible feats.
Python这门编程语言有很多句法结构，标准库函数，和交互式开发环境特性。幸运的事，其中大部分你都可以忽略；你只需要学习一些知识，让你能够随手编写小程序即可。然而，你需要在开始前学习一些编程的基本概念。像见习巫师一样，你可能会认为这些概念看上去晦涩又乏味，但是具备了一定的知识，加上一些练习，你就可以像使用魔杖那样，让你的电脑完成了不起的工作

This chapter has a few examples that encourage you to type into the interactive shell, which lets you execute Python instructions one at a time and shows you the results instantly. Using the interactive shell is great for learning what basic Python instructions do, so give it a try as you follow along. You’ll remember the things you do much better than the things you only read.

本章有几个例子，鼓励你在交互式shell中输入它们，你可以在此一次执行一条Python指令，并马上将结果显示给你。使用交互式shell对于学习Python基本指令非常有帮助，所以请在接下来尝试一下。与那些你读到的东西相比，那些你做了的事情你会记得更牢。



##Entering Expressions into the Interactive Shell
##在交互式shell中输入表达式


You run the interactive shell by launching IDLE, which you installed with Python in the introduction. On Windows, open the Start menu, select All Programs ▸ Python 3.3, and then select IDLE (Python GUI). On OS X, select Applications ▸ MacPython 3.3 ▸ IDLE. On Ubuntu, open a new Terminal window and enter idle3.
A window with the >>> prompt should appear; that’s the interactive shell. Enter 2 + 2 at the prompt to have Python do some simple math.

你可以通过启动IDLE来运行交互式shell，IDLE在引言一章已经随Python一起安装了。在Windos上，点击开始菜单，选择全部程序 ▸Python 3.3，然后选择IDLE (Python GUI)。在OS X系统上，选择应用程序MacPython 3.3 ▸ IDLE。在Ubuntu上，打开终端窗口，输入**idle3**。

A window with the >>> prompt should appear; that’s the interactive shell. Enter 2 + 2 at the prompt to have Python do some simple math.

一个带有>>>提示符的窗口应该会出现；这就是交互式shell。
输入2 + 2可以让Python进行一次简单的数学计算。

```
>>> 2 + 2
4
```

The IDLE window should now show some text like this:
IDLE窗口现在应该显示如下的文本：

```
Python 3.3.2 (v3.3.2:d047928ae3f6, May 16 2013, 00:06:53) [MSC v.1600 64 bit
(AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
>>> 2 + 2
4
>>>
```

In Python, 2 + 2 is called an expression, which is the most basic kind of programming instruction in the language. Expressions consist of values (such as 2) and operators (such as +), and they can always evaluate (that is, reduce) down to a single value. That means you can use expressions anywhere in Python code that you could also use a value.
In the previous example, 2 + 2 is evaluated down to a single value, 4. A single value with no operators is also considered an expression, though it evaluates only to itself, as shown here:

在Python中，2 + 2称之为表达式，是这个语言中最基本的一种程序指令。表达式包括值（比如2）以及操作符（比如＋），它总是会进行求值（减少变量），变为一个值。这就意味着在Python中，任何你可以使用表达式的地方你都可以使用一个值。在前面的例子中，2 + 2会求值得到一个单一的值4。一个不带有操作符的单一的值也被看做是表达式，尽管它只会求其本身的值，就像下面这样：

```
>>> 2
2
```


###ERRORS ARE OKAY!
###有错误，没关系！
Programs will crash if they contain code the computer can’t understand, which will cause Python to show an error message. An error message won’t break your computer, though, so don’t be afraid to make mistakes. A crash just means the program stopped running unexpectedly.
If you want to know more about an error message, you can search for the exact message text online to find out more about that specific error. You can also check out the resources at http://nostarch.com/automatestuff/ to see a list of common Python error messages and their meanings.

如果包含了电脑无法理解的指令，程序就会崩溃，也就会让Python显示错误信息。一条错误信息并不会弄坏你的电脑。所以并不要害怕犯错误。崩溃意味着程序突然停止工作。如果你想要了解更多关于错误信息的知识，你可以在网上搜索这条信息来找到更多关于这条特定信息的内容。你也可以查看这个网站的资源[http://nostarch.com/automatestuff/]( http://nostarch.com/automatestuff/)来看一下常见的Python错误信息以及它们代表的意思。



There are plenty of other operators you can use in Python expressions, too. For example, Table 1-1 lists all the math operators in Python.

还有很多你可以在Python表达式中使用的操作符。例如，表1-1列出了Python中所有的数学操作符

|Operator|Operation|Example|Evaluates to...|
|:----:|:----:|:-----:|:-----:|
|`**`|Exponent|2 ** 3|8|
|`%`|Modulus/remainder|22 % 8|6|
|`//`|Integer division/floored quotient|28//8|2|
|`/`|Division|22 / 8|2.75|
|`*`|Multiplication|3 * 5|15|
|`-`|Subtraction|5-2|3|
|`+`|Addition|2+2|4|

|操作符|操作|实例|求值|
|:----:|:----:|:-----:|:-----:|
|`**`|指数|2 ** 3|8|
|`%`|取模/求余|22 % 8|6|
|`//`|整除/商向下取整|28//8|2|
|`/`|除法|22 / 8|2.75|
|`*`|乘法|3 * 5|15|
|`-`|减法|5-2|3|
|`+`|加法|2+2|4|


The order of operations (also called precedence) of Python math operators is similar to that of mathematics. The ** operator is evaluated first; the *, /, //, and % operators are evaluated next, from left to right; and the + and - operators are evaluated last (also from left to right). You can use parentheses to override the usual precedence if you need to. Enter the following expressions into the interactive shell:

Python算术运算符的顺序（也叫做优先级）和数学里面是一样的。`**`首先被计算；`*`, `/`, `//`, 和 `%`次之，从左向右依次进行；`+`和`-`最后进行（同样也是从左到右）。如果需要的话你可以使用括号来手动控制优先级。在交互式shell中输入下面的表达式：

```
>>> 2 + 3 * 6
20
>>> (2 + 3) * 6
30
>>> 48565878 * 578453
28093077826734
>>> 2 ** 8
256
>>> 23 / 7
3.2857142857142856
>>> 23 // 7
3
>>> 23 % 7
2
>>> 2     +            2
4
>>> (5 - 1) * ((7 + 1) / (3 - 1))
16.0
```

In each case, you as the programmer must enter the expression, but Python does the hard part of evaluating it down to a single value. Python will keep evaluating parts of the expression until it becomes a single value, as shown in Figure 1-1.

在每一个例子中，你作为程序员，需要输入指令，然而Python做了最复杂的工作，把表达式求解为一个值。Python会不断求解表达式的各个部分知道它变为一个值，如图1-1所示。

These rules for putting operators and values together to form expressions are a fundamental part of Python as a programming language, just like the grammar rules that help us communicate. Here’s an example:

这些把操作符和变量放在一起构成表达式的规则，是Python这门编程语言的基础，就像帮助我们交流的语法一样。这里有一个例子：

- This is a grammatically correct English sentence.
- This grammatically is sentence not English correct a.

- 这是一个语法正确的中文句子
- 这是语法是句子不是中文正确的一个


The second line is difficult to parse because it doesn’t follow the rules of English. Similarly, if you type in a bad Python instruction, Python won’t be able to understand it and will display a SyntaxError error message, as shown here:

第二行难以解析因为它没有遵循中文的语法。同样的，如果你输入了一个错误的Python指令，Python不能够理解它并且会输出一个SyntaxError（语法错误）的错误信息，如下所示：

```
>>> 5 +
  File "<stdin>", line 1
    5 +
      ^
SyntaxError: invalid syntax
>>> 42 + 5 + * 2
  File "<stdin>", line 1
    42 + 5 + * 2
             ^
SyntaxError: invalid syntax
```


You can always test to see whether an instruction works by typing it into the interactive shell. Don’t worry about breaking the computer: The worst thing that could happen is that Python responds with an error message. Professional software developers get error messages while writing code all the time.
你总是可以通过在交互式shell中进行输入来判断一条指令是否可以工作。不要担心弄坏电脑：能够发生的最坏的事情无非是Python反馈给你一条错误信息。专业的软件开发者在写代码的时候也总是会得到错误提示。

##The Integer, Floating-Point, and String Data Types
##整型，浮点型和字符串类型
Remember that expressions are just values combined with operators, and they always evaluate down to a single value. A data type is a category for values, and every value belongs to exactly one data type. The most common data types in Python are listed in Table 1-2. The values -2 and 30, for example, are said to be integer values. The integer (or int) data type indicates values that are whole numbers. Numbers with a decimal point, such as 3.14, are called floating-point numbers (or floats). Note that even though the value 42 is an integer, the value 42.0 would be a floating-point number.

记住，表达式仅仅是值和操作符的组合，而且它们总是会求出一个单一的值。数据类型说一个值的种类，所有的值都属于某一个特定的类型。Python中最常见的数据类型已经列在表1-2中。比如说，-2和30是整型。整型（或者int）类型表示一个值是整数。
带有小数点的值，比如3.14，被称之为浮点型（或float）。注意，即使42是一个整数，42.0会被看作是一个浮点值。

|Data type|Examples|
|:--:|:--:|
|Integers|-2, -1, 0, 1, 2, 3, 4, 5|
|Floating-point numbers|-1.25, -1.0, --0.5, 0.0, 0.5, 1.0, 1.25|
|Strings|'a', 'aa', 'aaa', 'Hello!', '11 cats'|

|数据类型|示例|
|:--:|:--:|
|整型|-2, -1, 0, 1, 2, 3, 4, 5|
|浮点型|-1.25, -1.0, --0.5, 0.0, 0.5, 1.0, 1.25|
|字符串型|'a', 'aa', 'aaa', 'Hello!', '11 cats'|


Python programs can also have text values called strings, or strs (pronounced “stirs”). Always surround your string in single quote (') characters (as in '**Hello**' or '**Goodbye cruel world!**') so Python knows where the string begins and ends. You can even have a string with no characters in it, '', called a blank string. Strings are explained in greater detail in Chapter 4.
If you ever see the error message **SyntaxError: EOL while scanning string literal**, you probably forgot the final single quote character at the end of the string, such as in this example:

Python程序也可以有一些文本值，叫做字符串，或者strs（读作“stirs”）。始终要用单引号（‘）来包裹你的字符串（就像'**Hello**' 或 '**Goodbye cruel world!**'），这样Python就知道了字符串的起始和结尾。你也可以创建没有字符的字符串，`''`，叫做空字符串。字符串将在第四章做详细介绍。
如果你曾经见过这样的错误信息：**SyntaxError: EOL while scanning string literal**，你可能是忘记了字符串的结束引号，比如例子中这样。


```
>>> 'Hello world!
SyntaxError: EOL while scanning string literal
```

##String Concatenation and Replication
##字符串连接与复制
The meaning of an operator may change based on the data types of the values next to it. For example, + is the addition operator when it operates on two integers or floating-point values. However, when + is used on two string values, it joins the strings as the string concatenation operator. Enter the following into the interactive shell:

操作符的意义可能会随着它后面的变量的类型而变化。比如说，`+`对于两个整数或是浮点数的意思是加号。然而，如果把它应用于两个字符串，它会把两个字符串链接起来，作为连接操作符。在交互式命令行里输入下面的代码：


```
>>> 'Alice' + 'Bob'
'AliceBob'
```

The expression evaluates down to a single, new string value that combines the text of the two strings. However, if you try to use the + operator on a string and an integer value, Python will not know how to handle this, and it will display an error message.

表达式求值得到单一的值，新的字符串把两个字符串的文本合并起来。然而，如果你尝试对一个字符串和一个整数使用＋号，Python就不知道如何应对了，它就会显示一条错误信息。

```
>>> 'Alice' + 42
Traceback (most recent call last):
  File "<pyshell#26>", line 1, in <module>
    'Alice' + 42
TypeError: Can't convert 'int' object to str implicitly
```


The error message **Can't convert 'int' object to str implicitly** means that Python thought you were trying to concatenate an integer to the string '**Alice**'. Your code will have to explicitly convert the integer to a string, because Python cannot do this automatically. (Converting data types will be explained in [Dissecting Your Program]() when talking about the `str()`, `int()`, and `float()` functions.)

错误信息 **Can't convert 'int' object to str implicitly** 的意思是，Python认为你尝试把一个整数连接到字符串'**Alice**'。你的代码需要显式把整数转换为字符串，因为Python不能自动完成这一步。(数据类型转换将在[Dissecting Your Program]() 中解释，当我们谈到`str()`, `int()`, 和 `float()` 函数的时。)


```
>>> 'Alice' * 5
'AliceAliceAliceAliceAlice'
```

The expression evaluates down to a single string value that repeats the original a number of times equal to the integer value. String replication is a useful trick, but it’s not used as often as string concatenation.
The * operator can be used with only two numeric values (for multiplication) or one string value and one integer value (for string replication). Otherwise, Python will just display an error message.
表达式求值得到一个值，这个值把原始的字符串重复某个整数次。字符串复制是一个有用的技巧，但是它使用的次数并不如字符串连接那么多。＊操作符可以被用于两个数字值（做乘法）或者是一个字符串值和一个整数值（做字符串复制）。否则，Python会显示一条错误信息。


```
>>> 'Alice' * 'Bob'
Traceback (most recent call last):
  File "<pyshell#32>", line 1, in <module>
    'Alice' * 'Bob'
TypeError: can't multiply sequence by non-int of type 'str'
>>> 'Alice' * 5.0
Traceback (most recent call last):
  File "<pyshell#33>", line 1, in <module>
    'Alice' * 5.0
TypeError: can't multiply sequence by non-int of type 'float'
```

It makes sense that Python wouldn’t understand these expressions: You can’t multiply two words, and it’s hard to replicate an arbitrary string a fractional number of times.

Python不能理解这些表达式是有道理的：你不能把两个单词相乘，而且也不能把一个任意的字符串复制非整数次。

##Storing Values in Variables
##把值存放在变量中
A variable is like a box in the computer’s memory where you can store a single value. If you want to use the result of an evaluated expression later in your program, you can save it inside a variable.

变量就像是计算机内存中的一个盒子，你可以把一个值放在里面。如果你想在之后的程序中，使用一个表达式的结果，你可以把它存放在内部变量里。


##Assignment Statements
##赋值语句
You’ll store values in variables with an assignment statement. An assignment statement consists of a variable name, an equal sign (called the assignment operator), and the value to be stored. If you enter the assignment statement spam = 42, then a variable named spam will have the integer value 42 stored in it.

你会通过复制语句来把值存入变量。一条复制语句包含一个变量名，一个等于号（被称作赋值号），和一个被储存的值。如果你输入赋值语句 spam=42,然后一个叫做spam的变量中就好存放一个整数值42。

Think of a variable as a labeled box that a value is placed in, as in Figure 1-2.
把一个变量想象为一个带标签的盒子，里面放有一个值，如图1-2所示。

For example, enter the following into the interactive shell:

比如，在交互式shell中输入下面命令：

```
➊ >>> spam = 40
   >>> spam
   40
   >>> eggs = 2
➋ >>> spam + eggs
   42
   >>> spam + eggs + spam
   82
➌ >>> spam = spam + 2
   >>> spam
   42
```

A variable is initialized (or created) the first time a value is stored in it ➊. After that, you can use it in expressions with other variables and values ➋. When a variable is assigned a new value ➌, the old value is forgotten, which is why spam evaluated to 42 instead of 40 at the end of the example. This is called overwriting the variable. Enter the following code into the interactive shell to try overwriting a string:

变量在第一次有值存入时被初始化（或创建）➊。这之后你就可以在表达式中使用它喝其他变量和值➋. 当一个变量被赋予新值时➌,旧的值就被忘记，这也是为什么在例子的最后，spam值为人42而不是40。这被称之为变量的覆盖。在交互式shell中输入下面的代码来尝试覆盖一个字符串:

```
>>> spam = 'Hello'
>>> spam
'Hello'
>>> spam = 'Goodbye'
>>> spam
'Goodbye'  
```

Just like the box in Figure 1-3, the spam variable in this example stores 'Hello' until you replace it with 'Goodbye'.

就像图1-3中点盒子一样，本例中的spam变量存放了‘Hello',知道你用'Goodbye'覆盖了它。


##Variable Names
##变量名
Table 1-3 has examples of legal variable names. You can name a variable anything as long as it obeys the following three rules:
表1-3列举了一些合法的变量名。只要符合以下三条规则，你可以任意命名你的变量：

1. It can be only one word.
2. It can use only letters, numbers, and the underscore (_) character.
3. It can’t begin with a number. 

1. 它只能是一个单词。
2. 它只能使用字母，数字合下划线（`_`）。
3. 它不能以数字开头。


|Valid variable names|Invalid variable names|
|:---:|:---:|
|balance|current-balance (hyphens are not allowed)|
|currentBalance||current balance (spaces are not allowed)|
|current_balance|4account (can’t begin with a number)|
|_spam|42 (can’t begin with a number)|
|SPAM|total_$um (special characters like $ are not allowed)|
|account4|'hello' (special characters like ' are not allowed)|

|有效变量名|无效变量名|
|:---:|:---:|
|balance|current-balance (`-`不允许使用)|
|currentBalance||current balance (空格不允许使用)|
|current_balance|4account (不能以数字开头)|
|_spam|42 (不能以数字开头)|
|SPAM|total_$um (像`$`这样的特殊字符不允许)|
|account4|'hello' (像`'`这样的特殊字符不允许)|


Variable names are case-sensitive, meaning that **spam**, **SPAM**, **Spam**, and **sPaM** are four different variables. It is a Python convention to start your variables with a lowercase letter.
This book uses camelcase for variable names instead of underscores; that is, variables **lookLikeThis** instead of **looking_like_this**. Some experienced programmers may point out that the official Python code style, PEP 8, says that underscores should be used. I unapologetically prefer camelcase and point to “A Foolish Consistency Is the Hobgoblin of Little Minds” in PEP 8 itself:

变量名区分大小写，这意味着**spam**, **SPAM**, **Spam**, 和**sPaM** 是四个不同的变量名。变量名以小写字母开头是Python的惯例。

本书使用驼峰命名法，而不是下划线；也就是说，使用**lookLikeThis** 而不是**looking_like_this**。一些有经验的程序员也许会指出，官方Python代码风格PEP8认为应当使用下划线。我仍不知错的要，使用驼峰命名法，并指出PEP8中“愚蠢的一致性就像没有脑子的妖怪”一节所说：

>“Consistency with the style guide is important. But most importantly: know when to be inconsistent—sometimes the style guide just doesn’t apply. When in doubt, use your best judgment.”

>“与风格指南保持一致是很重要的。但是更重要的是：知道何时变的不一致——有些时候风格指南就是不适用。当你有所怀疑的时候，相信自己最好的判断”

A good variable name describes the data it contains. Imagine that you moved to a new house and labeled all of your moving boxes as Stuff. You’d never find anything! The variable names spam, eggs, and bacon are used as generic names for the examples in this book and in much of Python’s documentation (inspired by the Monty Python “Spam” sketch), but in your programs, a descriptive name will help make your code more readable.

一个好的变量名描述了它所存放的变量。想象着你搬进了一个新家，然后把你所有搬来的包裹都贴上了“东西”这个标签。那你就永远无法找到任何东西了！变量名spam, eggs, 还有 bacon，在本书的例子中以及Python文档中作为几个通用变量名。（受到Monty Python短剧“spam”短剧的启发），但是在你的程序中，一个描述性的名字会让你的程序更加易读。


##Your First Program
##你的第一个程序
While the interactive shell is good for running Python instructions one at a time, to write entire Python programs, you’ll type the instructions into the file editor. The file editor is similar to text editors such as Notepad or TextMate, but it has some specific features for typing in source code. To open the file editor in IDLE, select File▸New Window.
The window that appears should contain a cursor awaiting your input, but it’s different from the interactive shell, which runs Python instructions as soon as you press ENTER. The file editor lets you type in many instructions, save the file, and run the program. Here’s how you can tell the difference between the two:

尽管交互式shell很适合一次运行一条Python指令，为了写一个完整的程序，你还是会把程序输入到文件编辑器中。文件编辑器和文本编辑器类似，比如Notepad或是TextMate，但是它对于输入源代码具有一些特殊的功能。在IDLE中打开文件编辑器，选择File▸New Window。新打开的窗口中应该有一个等待你输入的光标,但是和交互式命令行有一些不同，交互式命令行在你按下回车后立即执行。文件编辑器允许你输入多项命令，保存文件，然后运行程序。以下是你如何分辨二者：


- The interactive shell window will always be the one with the `>>>`prompt.
- The file editor window will not have the `>>> `prompt.

- 交互式shell窗口总是有`>>>`的那一个。
- 文件编辑器是没有`>>>`的那一个。

Now it’s time to create your first program! When the file editor window opens, type the following into it:

现在，是时候创建你的第一个程序了！当文件编辑器开启后，输入如下命令：

```
➊ # This program says hello and asks for my name.
➋ print('Hello world!')
   print('What is your name?')    # ask for their name
➌ myName = input()
➍ print('It is good to meet you, ' + myName)
➎ print('The length of your name is:')
   print(len(myName))
➏ print('What is your age?')    # ask for their age
   myAge = input()
   print('You will be ' + str(int(myAge) + 1) + ' in a year.')
```

Once you’ve entered your source code, save it so that you won’t have to retype it each time you start IDLE. From the menu at the top of the file editor window, select File▸Save As. In the Save As window, enter **hello.py** in the File Name field and then click Save.
一旦你输入完成源代码，把它保存下来这样你就不需要在每一次启动IDLE时重复输入了。在文件编辑器顶端的菜单里面选择 File▸Save As。在保存窗口中文件名一栏输入 **hello.py** 然后点击保存。

You should save your programs every once in a while as you type them. That way, if the computer crashes or you accidentally exit from IDLE, you won’t lose the code. As a shortcut, you can press CTRL-S on Windows and Linux or ⌘-S on OS X to save your file.
当你输入一段时间后，就应该保存你的程序。这样的话，如果电脑死机了或是你不小心退出了IDLE，你不会丢失代码。说到快捷键，你可以在Windows 和 Linux上用CTRL-S或者在OS X上使用⌘-S来保存文件。 

Once you’ve saved, let’s run our program. Select Run▸Run Module or just press the F5 key. Your program should run in the interactive shell window that appeared when you first started IDLE. Remember, you have to press F5 from the file editor window, not the interactive shell window. Enter your name when your program asks for it. The program’s output in the interactive shell should look something like this:

一旦你完成保存，让我们运行我们的程序。选择 Run▸Run Module或按F5键。你的程序会在你第一次打开的交互式shell窗口中运行。记住，你需要在文件编辑器中按下F5，而不是交互式shell中。当程序像你询问时，输入你的名字。交互式命令行中会显示下面的内容：

```
Python 3.3.2 (v3.3.2:d047928ae3f6, May 16 2013, 00:06:53) [MSC v.1600 64 bit
(AMD64)] on win32
Type "copyright", "credits" or "license()" for more information.
>>> ================================ RESTART ================================
>>>
Hello world!
What is your name?
Al
It is good to meet you, Al
The length of your name is:
2
What is your age?
4
You will be 5 in a year.
>>>
```
When there are no more lines of code to execute, the Python program terminates; that is, it stops running. (You can also say that the Python program *exits*.)
You can close the file editor by clicking the X at the top of the window. To reload a saved program, select File▸Open from the menu. Do that now, and in the window that appears, choose hello.py, and click the Open button. Your previously saved hello.py program should open in the file editor window.

##Dissecting Your Program
With your new program open in the file editor, let’s take a quick tour of the Python instructions it uses by looking at what each line of code does.

###Comments
The following line is called a comment.

```
➊ # This program says hello and asks for my name.
```

Python ignores comments, and you can use them to write notes or remind yourself what the code is trying to do. Any text for the rest of the line following a hash mark (#) is part of a comment.
Sometimes, programmers will put a # in front of a line of code to temporarily remove it while testing a program. This is called commenting out code, and it can be useful when you’re trying to figure out why a program doesn’t work. You can remove the # later when you are ready to put the line back in.
Python also ignores the blank line after the comment. You can add as many blank lines to your program as you want. This can make your code easier to read, like paragraphs in a book.

###The print() Function

The print() function displays the string value inside the parentheses on the screen.

```
➋ print('Hello world!')
   print('What is your name?') # ask for their name
```

The line **print('Hello world!')** means “Print out the text in the string '**Hello world!**'.” When Python executes this line, you say that Python is calling the **print()** function and the string value is being passed to the function. A value that is passed to a function call is an argument. Notice that the quotes are not printed to the screen. They just mark where the string begins and ends; they are not part of the string value.

**NOTE**
*You can also use this function to put a blank line on the screen; just call print() with nothing in between the parentheses.*

When writing a function name, the opening and closing parentheses at the end identify it as the name of a function. This is why in this book you’ll see print() rather than print. Chapter 2 describes functions in more detail.

###The input() Function
The input() function waits for the user to type some text on the keyboard and press ENTER.

```
➌ myName = input()
```
This function call evaluates to a string equal to the user’s text, and the previous line of code assigns the myName variable to this string value.
You can think of the **input()** function call as an expression that evaluates to whatever string the user typed in. If the user entered 'Al', then the expression would evaluate to **myName = 'Al'**.

###Printing the User’s Name
The following call to print() actually contains the expression '**It is good to meet you, ' + myName** between the parentheses.

```
➍ print('It is good to meet you, ' + myName)
```
Remember that expressions can always evaluate to a single value. If 'Al' is the value stored in myName on the previous line, then this expression evaluates to '**It is good to meet you, Al**'. This single string value is then passed to print(), which prints it on the screen.


###The len() Function
You can pass the len() function a string value (or a variable containing a string), and the function evaluates to the integer value of the number of characters in that string.
```
➎ print('The length of your name is:')
  print(len(myName))
```
Enter the following into the interactive shell to try this:

```
>>> len('hello')
5
>>> len('My very energetic monster just scarfed nachos.')
46
>>> len('')
0
```
Just like those examples, len(myName) evaluates to an integer. It is then passed to print() to be displayed on the screen. Notice that print() allows you to pass it either integer values or string values. But notice the error that shows up when you type the following into the interactive shell:

```
>>> print('I am ' + 29 + ' years old.')
Traceback (most recent call last):
  File "<pyshell#6>", line 1, in <module>
    print('I am ' + 29 + ' years old.')
TypeError: Can't convert 'int' object to str implicitly
```

The **print()** function isn’t causing that error, but rather it’s the expression you tried to pass to print(). You get the same error message if you type the expression into the interactive shell on its own.

```
>>> 'I am ' + 29 + ' years old.'
Traceback (most recent call last):
  File "<pyshell#7>", line 1, in <module>
    'I am ' + 29 + ' years old.'
TypeError: Can't convert 'int' object to str implicitly
```

Python gives an error because you can use the + operator only to add two integers together or concatenate two strings. You can’t add an integer to a string because this is ungrammatical in Python. You can fix this by using a string version of the integer instead, as explained in the next section.

###The str(), int(), and float() Functions
If you want to concatenate an integer such as 29 with a string to pass to print(), you’ll need to get the value '29', which is the string form of 29. The str() function can be passed an integer value and will evaluate to a string value version of it, as follows:

```
>>> str(29)
'29'
>>> print('I am ' + str(29) + ' years old.')
I am 29 years old.
```

Because str(29) evaluates to '29', the expression 'I am ' + str(29) + ' years old.' evaluates to 'I am ' + '29' + ' years old.', which in turn evaluates to 'I am 29 years old.'. This is the value that is passed to the print() function.
The str(), int(), and float() functions will evaluate to the string, integer, and floating-point forms of the value you pass, respectively. Try converting some values in the interactive shell with these functions, and watch what happens.

```
>>> str(0)
'0'
>>> str(-3.14)
'-3.14'
>>> int('42')
42
>>> int('-99')
-99
>>> int(1.25)
1
>>> int(1.99)
1
>>> float('3.14')
3.14
>>> float(10)
10.0
```

The previous examples call the str(), int(), and float() functions and pass them values of the other data types to obtain a string, integer, or floating-point form of those values.
The str() function is handy when you have an integer or float that you want to concatenate to a string. The int() function is also helpful if you have a number as a string value that you want to use in some mathematics. For example, the input() function always returns a string, even if the user enters a number. Enter **spam = input()** into the interactive shell and enter **101** when it waits for your text.

```
>>> spam = input()
101
>>> spam
'101'
```

The value stored inside spam isn’t the integer 101 but the string '101'. If you want to do math using the value in spam, use the int() function to get the integer form of spam and then store this as the new value in spam.

```
>>> spam = int(spam)
>>> spam
101
```

Now you should be able to treat the spam variable as an integer instead of a string.

```
>>> spam * 10 / 5
202.0
```

Note that if you pass a value to int() that it cannot evaluate as an integer, Python will display an error message.

```
>>> int('99.99')
Traceback (most recent call last):
  File "<pyshell#18>", line 1, in <module>
    int('99.99')
ValueError: invalid literal for int() with base 10: '99.99'
>>> int('twelve')
Traceback (most recent call last):
  File "<pyshell#19>", line 1, in <module>
    int('twelve')
ValueError: invalid literal for int() with base 10: 'twelve'
```

The int() function is also useful if you need to round a floating-point number down. If you want to round a floating-point number up, just add 1 to it afterward.

```
>>> int(7.7)
7
>>> int(7.7) + 1
8
```

In your program, you used the int() and str() functions in the last three lines to get a value of the appropriate data type for the code.

```
➏ print('What is your age?') # ask for their age
   myAge = input()
   print('You will be ' + str(int(myAge) + 1) + ' in a year.')
```

The myAge variable contains the value returned from input(). Because the input() function always returns a string (even if the user typed in a number), you can use the int(myAge) code to return an integer value of the string in myAge. This integer value is then added to 1 in the expression int(myAge) + 1.

The result of this addition is passed to the str() function: str(int(myAge) + 1). The string value returned is then concatenated with the strings 'You will be ' and ' in a year.' to evaluate to one large string value. This large string is finally passed to print() to be displayed on the screen.

Let’s say the user enters the string '4' for myAge. The string '4' is converted to an integer, so you can add one to it. The result is 5. The str() function converts the result back to a string, so you can concatenate it with the second string, 'in a year.', to create the final message. These evaluation steps would look something like Figure 1-4.


##Summary
You can compute expressions with a calculator or type string concatenations with a word processor. You can even do string replication easily by copying and pasting text. But expressions, and their component values—operators, variables, and function calls—are the basic building blocks that make programs. Once you know how to handle these elements, you will be able to instruct Python to operate on large amounts of data for you.

It is good to remember the different types of operators (+, -, *, /, //, %, and ** for math operations, and + and * for string operations) and the three data types (integers, floating-point numbers, and strings) introduced in this chapter.

A few different functions were introduced as well. The print() and input() functions handle simple text output (to the screen) and input (from the keyboard). The len() function takes a string and evaluates to an int of the number of characters in the string. The str(), int(), and float() functions will evaluate to the string, integer, or floating-point number form of the value they are passed.

In the next chapter, you will learn how to tell Python to make intelligent decisions about what code to run, what code to skip, and what code to repeat based on the values it has. This is known as flow control, and it allows you to write programs that make intelligent decisions.




##Practice Questions

Q:
1. Which of the following are operators, and which are values?

```
*
'hello'
-88.8
-
/
+
5
```
Q:
2. Which of the following is a variable, and which is a string?

```
spam
'spam'
```
Q:
3. Name three data types.


Q:
4. What is an expression made up of? What do all expressions do?


Q:
5. This chapter introduced assignment statements, like spam = 10. What is the difference between an expression and a statement?


Q:
6. What does the variable bacon contain after the following code runs?
```
bacon = 20
bacon + 1
```

Q:
7. What should the following two expressions evaluate to?
```
'spam' + 'spamspam'
'spam' * 3
```

Q:
8. Why is eggs a valid variable name while 100 is invalid?


Q:
9. What three functions can be used to get the integer, floating-point number, or string version of a value?

Q:
10. Why does this expression cause an error? How can you fix it?
```
'I have eaten ' + 99 + ' burritos.'
```

Extra credit: Search online for the Python documentation for the len() function. It will be on a web page titled “Built-in Functions.” Skim the list of other functions Python has, look up what the round() function does, and experiment with it in the interactive shell.