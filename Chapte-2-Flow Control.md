# Flow Control 流程控制
## [相关教学视频](https://youtu.be/4XA9CKJJbr4)

So you know the basics of individual instructions and that a program is just a series of instructions. But the real strength of programming isn’t just running (or executing) one instruction after another like a weekend errand list. Based on how the expressions evaluate, the program can decide to skip instructions, repeat them, or choose one of several instructions to run. In fact, you almost never want your programs to start from the first line of code and simply execute every line, straight to the end. Flow control statements can decide which Python instructions to execute under which conditions.  
就你目前你所知的程序基本上是由各种基本语句和一系列指令组成的集合。但是真正的程序并不是像周末任务列表一样一个接一个运行。基于表达式的值，该程序可以决定跳过指令，重复运行某些指令，或选择几个指令来运行的。事实上，你几乎不会希望你的程序从第一行代码开始，顺序执行每一行，直奔终点。流程控制语句可以决定Python根据指示在不同条件下执行不同的逻辑。  

These flow control statements directly correspond to the symbols in a flowchart, so I’ll provide flowchart versions of the code discussed in this chapter. Figure 2-1 shows a flowchart for what to do if it’s raining. Follow the path made by the arrows from Start to End.  
这些流程控制语句直接对应流程图中的符号，我们将在本章讨论不同的代码流程图。
下图显示了如果下雨怎么办的流程图。按照从开始到结束的路径。  
![Figure](https://automatetheboringstuff.com/images/000105.jpg)  

In a flowchart, there is usually more than one way to go from the start to the end. The same is true for lines of code in a computer program. Flowcharts represent these branching points with diamonds, while the other steps are represented with rectangles. The starting and ending steps are represented with rounded rectangles.  
在一个流程中，通常从开始到结果有不止一种到达方式。在程序代码中也是这样。流程图中用菱形表示分支节点，而其他步骤用矩形表示。开始和结束的步骤被表示成具有圆角的矩形。  

But before you learn about flow control statements, you first need to learn how to represent those yes and no options, and you need to understand how to write those branching points as Python code. To that end, let’s explore Boolean values, comparison operators, and Boolean operators.  
但是在你学习流程控制语句之前，你首先需要学习如何表达yes和no选项，并且你需要了解在python代码中如何写那些分支点。为此，让我们来看看布尔值，比较运算符和布尔运算。  

## Boolean Values
## 布尔值

While the integer, floating-point, and string data types have an unlimited number of possible values, the Boolean data type has only two values: True and False. (Boolean is capitalized because the data type is named after mathematician George Boole.) When typed as Python code, the Boolean values True and False lack the quotes you place around strings, and they always start with a capital T or F, with the rest of the word in lowercase. Enter the following into the interactive shell. (Some of these instructions are intentionally incorrect, and they’ll cause error messages to appear.)  
整数，浮点和字符串数据类型具有数量不限的可能值,但是布尔类型的数据只有真和假两种值。(布尔是大写的，因为布尔数据类型是根据数学家乔治·布尔名字命名的。）在python代码中布尔变量的值都是以大写字母的T和F开头后面字母小写的Ture和
False来代表布尔值的真和假。在python交互窗体输入以下内容（其中的一些指令是故意写错的，他们会导致出现错误消息。）  

	>>> spam = True     # (1)
	>>> spam
	True
	>>> true            # (2)
	Traceback (most recent call last):
	  File "<stdin>", line 1, in <module>
	NameError: name 'true' is not defined
	>>> True = 2 + 2    # (3)
	  File "<stdin>", line 1
	SyntaxError: can't assign to keyword
	>>> 
	Connection to server timed out. Click run to reconne  

Like any other value, Boolean values are used in expressions and can be stored in variables ➊. If you don’t use the proper case ➋ or you try to use True and False for variable names ➌, Python will give you an error message.  
像任何其他值一样，布尔值可以在表达式中使用，并且可以存储在变量中（1）。如果你使用不正确（2）或试图使用True和False变量名（3），Python将会给你一个错误信息。  

## Comparison Operators
## 比较运算符

Comparison operators compare two values and evaluate down to a single Boolean value. Table 2-1 lists the comparison operators.    比较运算符比较两个值并最终获得一个单一的布尔值。下表2-1列出了比较操作符。    Table 2-1. Comparison Operators  

|Operator |Meaning|
|---------|-------|
|== |Equal to|
|!= |Not equal to|
|< |Less than|
|> |Greater than|
|<= |Less than or equal to|
|>= |Greater than or equal to|

These operators evaluate to True or False depending on the values you give them. Let’s try some operators now, starting with == and !=.  
这些表达式的结果为真或假取决于你给他们的值。让我们从==和!=开始尝试一些运算表达式。  

	>>> 42 == 42
	True
	>>> 42 == 99
	False
	>>> 2 != 3
	True
	>>> 2 != 2
	False
	>>> 

As you might expect, == (equal to) evaluates to True when the values on both sides are the same, and != (not equal to) evaluates to True when the two values are different. The == and != operators can actually work with values of any data type.  
正如你所预料的，==（等于）计算结果为真时，两边的值是相同的，！=（不等于）时，这两个值是不同的。==和！=操作实际上可以在任何数据类型之间。  

	>>> 'hello' == 'hello'
	True
	>>> 'hello' == 'Hello'
	False
	>>> 'dog' != 'cat'
	True
	>>> True == True
	True
	>>> True != False
	True
	>>> 42 == 42.0
	True
	>>> 42 == '42'
	False
	>>> 
	
Note that an integer or floating-point value will always be unequal to a string value. The expression 42 == '42' ➊ evaluates to False because Python considers the integer 42 to be different from the string '42'.  
注意，整数或浮点值将始终不等于一个字符串值。表达式42=='42'➊计算为假，因为Python认定整数42和字符串'42'不同。  