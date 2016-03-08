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
![Figure 2-2](https://automatetheboringstuff.com/images/000023.jpg)

##Elements of Flow Control
## 流程控制的元素

