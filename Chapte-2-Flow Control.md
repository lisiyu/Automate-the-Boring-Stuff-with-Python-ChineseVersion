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

Comparison operators compare two values and evaluate down to a single Boolean value. Table 2-1 lists the comparison operators.    比较运算符比较两个值并最终获得一个单一的布尔值。下表2-1列出了比较操作符。    
Table 2-1. Comparison Operators  

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
注意，整数或浮点值将始终不等于一个字符串值。表达式42=='42'➊计算为假，因为Python认为整数42和字符串'42'不同。 The <, >, <=, and >= operators, on the other hand, work properly only with integer and floating-point values.  
在另一方面<，>，<=，和> =运算符仅适用于整数和浮点值运算。  
	
	>>> 42 < 100
	True
	>>> 42 > 100
	False
	>>> 42 < 42
	False
	>>> eggCount = 42
	>>> eggCount <= 42
	True
	>>> myAge = 29
	>>> myAge >= 10
	True
	>>>    
		
### THE DIFFERENCE BETWEEN THE == AND = OPERATORS
You might have noticed that the == operator (equal to) has two equal signs, while the = operator (assignment) has just one equal sign. It’s easy to confuse these two operators with each other. Just remember these points:  
The == operator (equal to) asks whether two values are the same as each other.
The = operator (assignment) puts the value on the right into the variable on the left.
To help remember which is which, notice that the == operator (equal to) consists of two characters, just like the != operator (not equal to) consists of two characters.  
### ==和=运算符的区别  
你可能已经注意到了==运算符（等于）有两个等号，而=运算符（赋值）只有一个等号。这是很容易相互混淆的两个运算符。请记住以下几点：  
- ==运算符（等于）是询问两个值彼此是否相同。 
- =运算符（赋值）把右侧的值传递到左侧的变量。 
为了帮助记忆哪个是哪个，请注意==操作符（等于）由两个字符组成，就像！=运算符（不等于）一样也是两个字符。  

You’ll often use comparison operators to compare a variable’s value to some other value, like in the eggCount <= 42 ➊ and myAge >= 10 ➋ examples. (After all, instead of typing 'dog' != 'cat' in your code, you could have just typed True.) You’ll see more examples of this later when you learn about flow control statements.  
你会经常使用比较运算符比较两个变量的值，像eggCount <= 42和myAge> = 10的例子。 
（毕竟你在代码中只输入True，而比键入'狗'！='猫'方便多了。）当您了解流程控制语句后会看到更多的例子。  

## Boolean Operators
## 布尔运算符

The three Boolean operators (and, or, and not) are used to compare Boolean values. Like comparison operators, they evaluate these expressions down to a Boolean value. Let’s explore these operators in detail, starting with the and operator.  
三个布尔运算符（与，或，非）用于比较的布尔值。像比较运算符一样，他们计算表达式的值直到得到一个布尔值。让我们首先从与运算符开始来探究这些运算符。  

## Binary Boolean Operators
## 二元布尔运算符

The and and or operators always take two Boolean values (or expressions), so they’re considered binary operators. The and operator evaluates an expression to True if both Boolean values are True; otherwise, it evaluates to False. Enter some expressions using and into the interactive shell to see it in action.  
与和或运算符通常有两个布尔值或表达式，因此我们把它们成为二元运算符。如果两个布尔值是True的值进行和运算后结果为True，反之为False.在交互式窗口输入以下的表达式看看他们的运算结果。  

	>>> True and True
	True
	>>> True and False
	False

A truth table shows every possible result of a Boolean operator. Table 2-2 is the truth table for the and operator.
与运算符的真值表显示了布尔逻辑运算符的每一个可能的结果。表2-2是与运算符的真值表。  
Table 2-2. The and Operator’s Truth Table  

|Expression|Evaluates to|
|----------|------------|
|True and True|True|
|True and False|False|
|False and True|False|
|False and False|False|

On the other hand, the or operator evaluates an expression to True if either of the two Boolean values is True. If both are False, it evaluates to False
另一方面，如果两个布尔值其中一个为True则或运算符计算表达式值为True。如果两个都是假的，它的计算结果为False。 

You can see every possible outcome of the or operator in its truth table, shown in Table 2-3.   
如表2-3所示你可以看到在或运算符的每一个可能的结果。  
Table 2-3. The or Operator’s Truth Table  

|Expression|Evaluates to|
|----------|------------|
|True and True|True|
|True and False|True|
|False and True|True|
|False and False|False|

## The not Operator
## NOT运算符
Unlike and and or, the not operator operates on only one Boolean value (or expression). The not operator simply evaluates to the opposite Boolean value.  
和与和或表达式不同，非运算符运行在只有一个布尔值（或表达式）。非运算符计算结果为相反的布尔值。  

	>>> not True
	False
	>>> not not not not True    # (1)
	True
	
Much like using double negatives in speech and writing, you can nest not operators ➊, though there’s never not no reason to do this in real programs. Table 2-4 shows the truth table for not.  
（1）就像在语言和写作中使用双重否定，可以多次使用非表达式，虽然实际程序很少这样实现。表2-4显示了非运算符的真值表。  
Table 2-4. The not Operator’s Truth Table   

|Expression|Evaluates to|
|----------|------------|
|not True|False|
|not False|True|

## Mixing Boolean and Comparison Operators
##　混合布尔和比较运算符

Since the comparison operators evaluate to Boolean values, you can use them in expressions with the Boolean operators.Recall that the and, or, and not operators are called Boolean operators because they always operate on the Boolean values True and False. While expressions like 4 < 5 aren’t Boolean values, they are expressions that evaluate down to Boolean values. Try entering some Boolean expressions that use comparison operators into the interactive shell.　　　　
由于比较运算符计算结果为布尔值，你可以在表达式中使用布尔运算符。因为与，或，非的值总是布尔值的True和false，所以我们们把他们成为布尔运算符。就像表达式4<5，虽然不是布尔值，但是表达式的运算结果会获得一个布尔值。在交互窗口输入以下使用比较操作符的布尔运算式。

	>>> (4 < 5) and (5 < 6)
	True
	>>> (4 < 5) and (9 < 6)
	False
	>>> (1 == 2) or (2 == 2)
	True
	>>> 
	
The computer will evaluate the left expression first, and then it will evaluate the right expression. When it knows the Boolean value for each, it will then evaluate the whole expression down to one Boolean value. You can think of the computer’s evaluation process for (4 < 5) and (5 < 6) as shown in Figure 2-2.  
You can also use multiple Boolean operators in an expression, along with the comparison operators.  
计算机将会从左到右依次计算表达式的值。当得到每一个表达式的布尔值后，它计算评估整个表达式直到获得一个布尔值。你可以思考下计算机计算(4 < 5) and (5 < 6)的过程，如图 Figure2-2.您也可以在表达式中使用多个布尔运算符和比较运算符.

	>>> 2 + 2 == 4 and not 2 + 2 == 5 and 2 * 2 == 2 + 2
	True
	
The Boolean operators have an order of operations just like the math operators do. After any math and comparison operators evaluate, Python evaluates the not operators first, then the and operators, and then the or operators.  
布尔运算符的操作顺序就像数学运算。先经进行各种数学运算和比较运算，Python的计算结果首先是非运算符，然后是和运算符，最后是或运算符。  

####   Figure2-2  
![Figure 2-2](https://automatetheboringstuff.com/images/000023.jpg)

##Elements of Flow Control
## 流程控制的原理

Flow control statements often start with a part called the condition, and all are followed by a block of code called the clause. Before you learn about Python’s specific flow control statements, I’ll cover what a condition and a block are.  
流程控制语句开始部分我们称为条件，后面跟着一个代码块叫做子句。在你学习Python的具体流程控制语句前，我将介绍什么是条件和什么是代码块。  

### Conditions
### 条件

The Boolean expressions you’ve seen so far could all be considered conditions, which are the same thing as expressions; condition is just a more specific name in the context of flow control statements. Conditions always evaluate down to a Boolean value, True or False. A flow control statement decides what to do based on whether its condition is True or False, and almost every flow control statement uses a condition.  
到目前为止我们在布尔表达式中考虑到的各种情况都是相同的表达式。条件只是在流程控制语句中更具体的名称而已。条件运算的结果最终为一个布尔值，真或假。而这几乎是每一个流量控制语句使用的条件。  

### Blocks of Code
### 代码块

Lines of Python code can be grouped together in blocks. You can tell when a block begins and ends from the indentation of the lines of code. There are three rules for blocks.  
-Blocks begin when the indentation increases.  
-Blocks can contain other blocks.  
-Blocks end when the indentation decreases to zero or to a containing block’s indentation.
Blocks are easier to understand by looking at some indented code, so let’s find the blocks in part of a small game program, shown here:  
Python代码行可以一起组成一个块。通过代码的缩进你可以知道每一个代码块的开始和结束。这里有针对代码分块的三个规则。
-缩进增加代表代码块开始。  
-代码块可以在其他代码块中间。
-当缩进减少到零或者遇到另一个代码块的缩进时代码块结束。  
通过观察代码缩进很容易理解代码块。让我们在下面这个小游戏代码中来寻找代码块吧。  

	name = 'Mary'
	password = 'swordfish'
	if name == 'Mary':
		print('Hello Mary')
		if password == 'swordfish':
			print('Access granted.')
		else:
			print('Wrong password.')
  
The first block of code starts at the line print('Hello Mary') and contains all the lines after it. Inside this block is another block , which has only a single line in it: print('Access Granted.'). The third block is also one line long: print('Wrong password.').  
第一个代码块开始于行print('Hello Marry')并且包含后面所有的部分。在这个代码块里面有另外一个代码块，仅仅包含一行代码：print('Access Granted').第三个代码块也仅仅有一行代码长：print('Wrong password').  

### Program Execution
### 程序执行

In the previous chapter’s hello.py program, Python started executing instructions at the top of the program going down, one after another. The program execution (or simply, execution) is a term for the current instruction being executed. If you print the source code on paper and put your finger on each line as it is executed, you can think of your finger as the program execution.  
在前面的章节中的hello.py程序，python开始执行的时候是从程序的第一行开始一直往下，一行接一行。程序执行（或简单地说，执行）是用于当前指令正在执行的一个术语。如果您在纸张上打印的源代码，把你手指过程序的每一行当着执行，你可以把你的手指作为程序执行。  
Not all programs execute by simply going straight down, however. If you use your finger to trace through a program with flow control statements, you’ll likely find yourself jumping around the source code based on conditions, and you’ll probably skip entire clauses.  
但并不是所有的程序都是这样简单从头到尾按顺序执行。如果你用你的手指跟随流程控制语句执行程序，你会发现你需要根据条件跳来跳去，有时候还会跳过整个子句。  

## Flow Control Statements
## 流控制语句
## [相关视频教程](https://youtu.be/lWeCgEbk-Ro)

Now, let’s explore the most important piece of flow control: the statements themselves. The statements represent the diamonds you saw in the flowchart in Figure 2-1, and they are the actual decisions your programs will make.  
现在，让我们来探索流程控制最重要的部分：该语句本身。该声明标识你在图2-1中看到的流程图中的钻石图形部分，他们将决定你程序如何运行。  

### if Statements
### if 语句

The most common type of flow control statement is the if statement. An if statement’s clause (that is, the block following the if statement) will execute if the statement’s condition is True. The clause is skipped if the condition is False.  
if语句是流程控制语句中最常见的类型。if语句的子句（也就是指if语句下面的程序块）将被执行，如果该if语句的条件为True。如果if条件的结果为False该子句被跳过.  
In plain English, an if statement could be read as, “If this condition is true, execute the code in the clause.” In Python, an if statement consists of the following:  
用简单的英语，if语句可以理解为，“如果这个条件为真，则执行该子句中的代码。” 在python中if语句包含以下内容：  

- The if keyword
- A condition (that is, an expression that evaluates to True or False)
- A colon
- Starting on the next line, an indented block of code (called the if clause)  
- if关键字
- 条件（也就是说，计算结果为真或假的表达式)
- 冒号
- 另起一行并且包含缩进的代码块(称为if子句)  

For example, let’s say you have some code that checks to see whether someone’s name is Alice. (Pretend name was assigned some value earlier.)  
例如，我们有一段用来检测别人的名字是否为Alice的代码。（假设名字提前赋值在一个变量中）  

	if name == 'Alice':
		print('Hi, Alice.')

All flow control statements end with a colon and are followed by a new block of code (the clause). This if statement’s clause is the block with print('Hi, Alice.'). Figure 2-3 shows what a flowchart of this code would look like.  
所有的流程控制语句都以冒号结束后面跟随一个新的代码块（子句）。这if语句的子句是代码块print('Hi,Alice').图2-3显示了此代码的流程图的样子。  

![Figure 2-3](https://automatetheboringstuff.com/images/000019.jpg)
> Figure 2-3. The flowchart for an if statement  

### else Statements
### else语句

An if clause can optionally be followed by an else statement. The else clause is executed only when the if statement’s condition is False. In plain English, an else statement could be read as, “If this condition is true, execute this code. Or else, execute that code.” An else statement doesn’t have a condition, and in code, an else statement always consists of the following:  
-The else keyword  
-A colon
-Starting on the next line, an indented block of code (called the else clause)  
Returning to the Alice example, let’s look at some code that uses an else statement to offer a different greeting if the person’s name isn’t Alice.  
一个if语句后面可跟着一个else语句。当if语句的条件为假else子句被执行。用简单的英语，一个else语句可以理解为，“如果这个条件为真，执行该代码。否则，执行其他代码“。else语句没有具体条件。在代码中，else语句以下面方式表示：  
- else关键字
- 一个冒号
- 另起一行并且包含缩进的代码块(称为else子句)
让我们回到Alice的例子，让我们来看看如果这个人的名字不是Alice使用else语句来提供不同的问候语的代码。

	name = 'Bob'
	if name == 'Alice':
		print('Hi, Alice.')
	else:
		print('Hello, stranger.')
		
Figure 2-4 shows what a flowchart of this code would look like.
图2-4显示了此代码的流程图的样子。
![Figure 2-4](https://automatetheboringstuff.com/images/000106.png)
> Figure 2-4. The flowchart for an else statement

### elif Statements
### ELIF语句

While only one of the if or else clauses will execute, you may have a case where you want one of many possible clauses to execute. The elif statement is an “else if” statement that always follows an if or another elif statement. It provides another condition that is checked only if any of the previous conditions were False. In code, an elif statement always consists of the following:  

- The elif keyword  
- A condition (that is, an expression that evaluates to True or False)
- A colon
- Starting on the next line, an indented block of code (called the elif clause)
Let’s add an elif to the name checker to see this statement in action.  
虽然仅有一个if或else就能执行，但是有的情况下可能有多个不同子句需要执行。elif语句，就是一个“else is”语句,始终跟随if语句或其他elif语句。当任何前面的所有条件都是假时它提供另一个条件进行判断。在代码中，else语句以下面方式表示：  
- elif关键字
- 一个条件（也就是，计算结果为真或假的表达式）
- 一个冒号
- 另起一行并且包含缩进的代码块(称为elif子句)
让我们把elif加到名字检查例程中看看这个语句如何执行。  

	name = 'Bob'
	age = 5
	if name == 'Alice':
		print('Hi, Alice.')
	elif age < 12:
		print('You are not Alice, kiddo.')
		
This time, you check the person’s age, and the program will tell them something different if they’re younger than 12. You can see the flowchart for this in Figure 2-5.  
这次，你检查人的年龄，如果他们小于12岁程序会告诉他们不同的东西。程序执行流程图 如图2-5
![Figure](https://automatetheboringstuff.com/images/000107.png)
> Figure 2-5. The flowchart for an elif statement

The elif clause executes if age < 12 is True and name == 'Alice' is False. However, if both of the conditions are False, then both of the clauses are skipped. It is not guaranteed that at least one of the clauses will be executed. When there is a chain of elif statements, only one or none of the clauses will be executed. Once one of the statements’ conditions is found to be True, the rest of the elif clauses are automatically skipped. For example, open a new file editor window and enter the following code, saving it as vampire.py:  
如果年龄小于12是真并且名字是Alice为假elif语句将会执行。如果这两个条件的结果都是假的，则这两个子句都会跳过。它并不保证所有子句中的至少一个将被执行。存在多个elif语句的程序中，只有一个或没有子句被执行。一旦这些语句的条件之一被发现是真，其余elif子句将被自动跳过。例如，打开一个新的文件编辑器窗口输入以下代码，保存为vampire.py：

	name = 'Dracula'
	age = 4000
	if name == 'Alice':
		print('Hi, Alice.')
	elif age < 12:
		print('You are not Alice, kiddo.')
	elif age > 2000:
		print('Unlike you, Alice is not an undead, immortal vampire.')
	elif age > 100:
    print('You are not Alice, grannie.')
	
Here I’ve added two more elif statements to make the name checker greet a person with different answers based on age. Figure 2-6 shows the flowchart for this.  
在这里，我增加了两个ELIF语句，以使名称检查同时基于年龄给不同的人不同的答案。图2-6显示了该流程图。
![Figure 2-6](https://automatetheboringstuff.com/images/000088.png)
> Figure 2-6. The flowchart for multiple elif statements in the vampire.py program

The order of the elif statements does matter, however. Let’s rearrange them to introduce a bug. Remember that the rest of the elif clauses are automatically skipped once a True condition has been found, so if you swap around some of the clauses in vampire.py, you run into a problem. Change the code to look like the following, and save it as vampire2.py:  
elif语句按照顺序完成事物。让我们重新排列它们引入的错误。请记住，elif子句发现一次条件为真时其余部分自动跳过。如果你在vampire2.py中换一些子句你会运行遇到错误。把你的代码改成下面的样子并保存为vampire2.py：  

	name = 'Dracula'
	age = 4000
	if name == 'Alice':
		print('Hi, Alice.')
	elif age < 12:
		print('You are not Alice, kiddo.')
	elif age > 100:
		print('You are not Alice, grannie.')
	elif age > 2000:
		print('Unlike you, Alice is not an undead, immortal vampire.')
		
Say the age variable contains the value 3000 before this code is executed. You might expect the code to print the string 'Unlike you, Alice is not an undead, immortal vampire.'. However, because the age > 100 condition is True (after all, 3000 is greater than 100) , the string 'You are not Alice, grannie.' is printed, and the rest of the elif statements are automatically skipped. Remember, at most only one of the clauses will be executed, and for elif statements, the order matters!   
假设代码执行之前把变量age赋值为3000。你期望代码输出'Unlike you, Alice is not an undead, immortal vampire.'.。但是age >100已经为真了。（尽管3000比100大很多），'You are not Alice, grannie.'被打印出来，剩下的elif语句都被跳过了。对于elif语句来说最多只有一个子句被执行这是确信无疑的事实。  

Figure 2-7 shows the flowchart for the previous code. Notice how the diamonds for age > 100 and age > 2000 are swapped.  
图2-7显示了前面的代码的流程图。请注意age > 100和age > 2000流程图的交换。  
![Figure 2-7](https://automatetheboringstuff.com/images/000089.png)
> Figure 2-7. The flowchart for the vampire2.py program. The crossed-out path will logically never happen, because if age were greater than 2000, it would have already been greater than 100.  
> 图2-7为vampire2.py程序的流程图。打叉的路径逻辑永远不会发生，因为如果年龄超过2000人时，它早已经大于100。  

Optionally, you can have an else statement after the last elif statement. In that case, it is guaranteed that at least one (and only one) of the clauses will be executed. If the conditions in every if and elif statement are False, then the else clause is executed. For example, let’s re-create the Alice program to use if, elif, and else clauses.    
你可以有在所有elif语句后面else语句。
在这种情况下，可以保证子句中的至少一个（并且仅一个）将被执行。如果所有if和elif的语句的条件都是假的，那么else子句被执行。例如，让我们重新创建一个使用if,elif和else子句的Alice程序。  

	name = 'Bob'
	age = 30
	if name == 'Alice':
		print('Hi, Alice.')
	elif age < 12:
		print('You are not Alice, kiddo.')
	else:
		print('You are neither Alice nor a little kid.')
		
Figure 2-8 shows the flowchart for this new code, which we’ll save as littleKid.py.  
图2-8展示了这个新的代码的流程图，我们将其保存为littleKid.py。  
In plain English, this type of flow control structure would be, “If the first condition is true, do this. Else, if the second condition is true, do that. Otherwise, do something else.” When you use all three of these statements together, remember these rules about how to order them to avoid bugs like the one in Figure 2-7. First, there is always exactly one if statement. Any elif statements you need should follow the if statement. Second, if you want to be sure that at least one clause is executed, close the structure with an else statement.  
简单的说，这种类型的流程控制结构是，“如果第一个条件为真，执行它。否则，如果第二条件为真，执行这个。否则，执行其他的事情。“当您同时使用这三个语句，记住以下的规则以避免出现图2-7中的bug。首先，总共只有一个if语句。任何 elif语句都在if语句后面。第二，如果你要确保至少有一个子句被执行，需要在代码块最后以else语句结束。
![Figure 2-8](https://automatetheboringstuff.com/images/000090.png)
> Figure 2-8. Flowchart for the previous littleKid.py program

### while Loop Statements
### while循环语句
