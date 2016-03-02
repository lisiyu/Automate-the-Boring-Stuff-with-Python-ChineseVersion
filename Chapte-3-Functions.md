# Functions
## https://youtu.be/WB4hJJkfhLU相应的视频教程
### 
 You’re already familiar with the print(), input(), and len() functions from the previous chapters. 
 Python provides several builtin functions like these, but you can also write your own functions. 
 A function is like a mini-program within a program.
 在前面的章节你已经熟悉的print()，input()和len()函数。
 Python提供了一些这样的内建函数，你也可以编写自己的函数。
 函数就像一个程序中的一个小程序。
### 
 To better understand how functions work, let’s create one. Type this program into the file editor and save it as helloFunc.py:
 理解函数的工作原理的最好方法是我们创建一个试试。在文件编辑器里面输入这段代码到并保存为helloFunc.py：
### 
''def hello():  
	print('Howdy!')  
	print('Howdy!!!')  
	print('Hello there.')  
hello()  
hello()  
hello()  ''
### 
 The first line is a def statement [1], which defines a function named hello().
 The code in the block that follows the def statement[2]， is the body of the function. 
 This code is executed when the function is called, not when the function is first defined.
 第一行的def我们成为函数声明语句。def为函数声明关键词。我们将这个函数名称定义为hello.
 紧跟着函数声明语句的代码块我们成为函数体。
 当函数被调用的时候函数的代码才会执行，而不是在首次定义函数的时候执行该代码。
### 
 The hello() lines after the function are function calls. In code,  a function call is  just the  function’s name 
 followed by  parentheses, possibly with some number of arguments in between the parentheses.  When the  program execution
 reaches these  calls, it  will jump  to the  top line  in the function and begin executing the code there. When it reaches the end 
 of the function, the execution eturns to the line  that called the function  and continues moving through  the code as before. 
 Since  this program calls hello()  three times, the code  in the hello() function is executed three times. When you run this program,
 the  output looks like this:  
'Howdy!  
Howdy!!!  
Hello there.  
Howdy!  
Howdy!!!  
Hello there.  
Howdy!  
Howdy!!!  
Hello there.  '
 最后三行的hello()我们称之为函数调用。函数调用仅仅需要函数名和紧跟着的括号，括号里面包含几个这个函数所定义的参数。当程序执行到
 函数调用的时候会自动跳转到这个函数声明的位置并开始执行函数代码。当函数功能的结束时，执行返回到调用函数位置，并继续执行下面的代码.
 因为这段代码调用了三次hello()函数所以hello()函数被执行了三次。当你运行这段代码时输出结果如下：  
Howdy!    
Howdy!!!    
Hello there.  
Howdy!  
Howdy!!!  
Hello there.  
Howdy!  
Howdy!!!  
Hello there.  
### 
 A major purpose of functions is to group code that gets executed multiple times. Without a function defined, you would have to  copy and paste this code each time, and the program would look like this:
 定义函数功能的主要目的把需要多次执行的代码遍成一个组。如果没有定义一个函数，你就必须复制和粘贴此代码，刚才的程序就会变成这样：  
print('Howdy!')  
print('Howdy!!!')  
print('Hello there.')  
print('Howdy!')  
print('Howdy!!!')  
print('Hello there.')  
print('Howdy!')  
print('Howdy!!!')  
print('Hello there.')  
### 
In general, you always want to avoid duplicating code, because if you ever decide to update the code—if, for example, you find a bug you need to fix—you’ll have to remember to change the code everywhere you copied it.  
一般情况下，你总是希望避免重复的代码。举个例子，当你发现程序片段中有bug需要修复，你需要记得把你到处复的所有代码中的错误都进行修复。这是很痛苦的。  

## def Statements with Parameters
## 带参数的函数声明语句 def
### 
 When you call the print() or len() function, you pass in values, called arguments in this context, by typing them between the parentheses. You can also define your own functions that accept arguments. Type this example into the file editor and save it as helloFunc2.py:  
当你调用print（）或LEN（）函数时在括号中输入的内容我们称为函数车参数。你也可以定义自己的函数可以接受的参数。在文件编辑器输入如下示例程序并保存为helloFunc2.py  
def hello(name):  
	print('Hello ' + name)  
hello('Alice')  
hello('Bob')  
When you run this program, the output looks like this:  
当你运行这个程序时可以获得如下结果：  
Hello Alice  
Hello Bob  
### 
The definition of the hello() function in this program has a parameter called name .A parameter is a variable that an argument is stored in when a function is called. The first time the hello() function is called, it’s with the argument 'Alice'. The program execution enters the function, and the variable name is automatically set to 'Alice', which is what gets printed by the print() statement.  
我们在这段代码中定义Hello（）函数有一个参数叫name。当函数被调用时该参数被当成一个变量存储在函数中。当第一次调用Hello（）函数时它被赋值为‘Alice'.当程序执行时，变量name就被自动赋值为'Alice'并且能够传递给print()函数。  
### 
One special thing to note about parameters is that the value stored in a parameter is forgotten when the function returns. For example, if you added print(name) after hello('Bob') in the previous program, the program would give you a NameError because there is no variable named name. This variable was destroyed after the function call hello('Bob') had returned, so print(name) would refer to a name variable that does not exist.  
需要注意的是参数有一个特别之处，当函数返回时存储在一个参数的值将被清空。举例，在前面的程序中如果你在hello('Bob')后添加代码print（name)，程序会报NameError错误，因为变量name没有被赋值。name的值在函数调用hello('Bob')返回后就被清空了。所以print(name)将指向一个不存在值的变量name。  
### 
This is similar to how a program’s variables are forgotten when the program terminates. I’ll talk more about why that happens later in the chapter, when I discuss what a function’s local scope is.  
这类似于程序终止时，程序的变量被清空。在后面的章节中讲到函数的局部范围时我们在做更多地讨论。  

## Return Values and return Statements  
## 返回值和返回语句  
### 
When you call the len() function and pass it an argument such as 'Hello', the function call evaluates to the integer value 5, which is the length of the string you passed it. In general, the value that a function call evaluates to is called the return value of the function.  
When creating a function using the def statement, you can specify what the return value should be with a return statement. A return statement consists of the following:  
- The return keyword  
- The value or expression that the function should return  
当你把hello作为参数传递给函数len()时，函数调用的计算结果为整型值5，刚好这就是你传递参数hello字符串的长度。通常我们把该函数调用后的计算结果值称为被调用的函数的返回值。  
当使用def语句创建一个新函数时，我们可以用return声明语句定义函数的返回值应该是什么。return声明语句句法如下：  
- 关键字 return  
- 希望函数返回的值或者表达式  
### 
When an expression is used with a return statement, the return value is what this expression evaluates to. For example, the following program defines a function that returns a different string depending on what number it is passed as an argument. Type this code into the file editor and save it as magic8Ball.py:  
当用表达式来定义返回语句时，返回值就是表达式的运算结果。举例，下面程序不同的数字作为参数时将返回不同的字符串。在文件编辑器中编写下面的代码并保存为magic8Ball.py:  
➊ import random  
➋ def getAnswer(answerNumber):  
➌     if answerNumber == 1:  
           return 'It is certain'  
       elif answerNumber == 2:  
           return 'It is decidedly so'  
       elif answerNumber == 3:  
           return 'Yes'  
       elif answerNumber == 4:  
           return 'Reply hazy try again'  
       elif answerNumber == 5:  
           return 'Ask again later'  
       elif answerNumber == 6:  
           return 'Concentrate and ask again'  
       elif answerNumber == 7:  
           return 'My reply is no'  
       elif answerNumber == 8:  
           return 'Outlook not so good'  
       elif answerNumber == 9:  
           return 'Very doubtful'  

➍ r = random.randint(1, 9)  
➎ fortune = getAnswer(r)  
➏ print(fortune)  
### 
When this program starts, Python first imports the random module ➊. Then the getAnswer() function is defined ➋. Because the function is being defined (and not called), the execution skips over the code in it. Next, the random.randint() function is called with two arguments, 1 and 9 ➍. It evaluates to a random integer between 1 and 9 (including 1 and 9 themselves), and this value is stored in a variable named r.  
当程序执行时先导入random模块。然后定义 getAnswer()函数。因为该函数刚被定义（没调用），执行时会跳过它的代码。接下来random.randint()函数调用并使用了两个参数1和9.它的计算结果为1和9之间的随机整数（包括1和9本身）并且该值被存储在一个变量名r中。  
### 
The getAnswer() function is called with r as the argument ➎. The program execution moves to the top of the getAnswer() function ➌, and the value r is stored in a parameter named answerNumber. Then, depending on this value in answerNumber, the function returns one of many possible string values. The program execution returns to the line at the bottom of the program that originally called getAnswer() ➎. The returned string is assigned to a variable named fortune, which then gets passed to a print() call ➏ and is printed to the screen.  
getAnswer（）函数被调用并把变量r作为参数。程序执行将跳转到getAnswer()函数的第一行，并且r值存储在参数answerNumber中。然后根据 answerNumber被赋予的不同值函数返回多个字符串中的某一个值。程序执行返回到原来调用的getAnswer()函数的的底部。他返回的字符串被分配到一个名为fortune的变量，然后把它传递给打印函数print()并将结果打印到屏幕上。  
### 
Note that since you can pass return values as an argument to another function call, you could shorten these three lines:  
需要注意的是，因为可以通过返回值作为参数传递给另一个函数调用，所以您可以把三行缩短成一行：  
r = random.randint(1, 9)  
fortune = getAnswer(r)  
print(fortune)  
to this single equivalent line:  
print(getAnswer(random.randint(1, 9)))  
### 
Remember, expressions are composed of values and operators. A function call can be used in an expression because it evaluates to its return value.  
请记住，表达式是由值和运算符组成。函数调用可以在表达式中使用，因为表达式的计算结果就是它的返回值。  

## The None Value
## 空值

In Python there is a value called None, which represents the absence of a value. None is the only value of the NoneType data type. (Other programming languages might call this value null, nil, or undefined.) Just like the Boolean True and False values, None must be typed with a capital N.  
在python中有一个表示不存在的值，NoneType数据类型的唯一值，我们称其为空值。在其他编程语言中可能叫做空或者未定义值。这个值就像布尔True和False值，空值必须以大写N开头写为None.  

This value-without-a-value can be helpful when you need to store something that won’t be confused for a real value in a variable. One place where None is used is as the return value of print(). The print() function displays text on the screen, but it doesn’t need to return anything in the same way len() or input() does. But since all function calls need to evaluate to a return value, print() returns None. To see this in action, enter the following into the interactive shell:  
当你需要在变量中存储一个无法定义的数值时，空值就会变得非常有用。空值有一个常用的地方就是作为print()函数执行后的返回值。print()函数的功能是把字符打印到屏幕上，但是他又不能像len()或input()函数一样执行后返回一个真实存在的值。但所有函数执行完成后都需要一个返回值，print()函数返回为空值。想看到空值的作用请在交互窗口中输入如下代码：  
spam = print('Hello!')  
Hello!  
None == spam  
True  

Behind the scenes, Python adds return None to the end of any function definition with no return statement. This is similar to how a while or for loop implicitly ends with a continue statement. Also, if you use a return statement without a value (that is, just the return keyword by itself), then None is returned.  
在幕后，python在任何未定义返回参数的函数末尾增加了返回空值语句。这就好像for循环和whlie循环在末尾隐藏了一个continue语句。另外，如果使用return语句没有返回值（即，只返回关键字本身）这个时候就会返回空值。  

## Keyword Arguments and print()
## 关键字参数和print()函数

Most arguments are identified by their position in the function call. For example, random.randint(1, 10) is different from random.randint(10, 1). The function call random.randint(1, 10) will return a random integer between 1 and 10, because the first argument is the low end of the range and the second argument is the high end (while random.randint(10, 1) causes an error).  
大多数参数都是由它们在函数调用位置来识别。例如，random.randint（1，10和random.randint（10，1）不同。函数调用random.randint（1，10）将返回1和10之间的随机整数，因为第一个参数是random函数的最小值，第二个参数是最大值。如果写成random.randint(10, 1)就会出错。  

However, keyword arguments are identified by the keyword put before them in the function call. Keyword arguments are often used for optional parameters. For example, the print() function has the optional parameters end and sep to specify what should be printed at the end of its arguments and between its arguments (separating them), respectively.  
If you ran the following program:  
但是关键字参数是在他们函数调用之前通过关键字进行定义和区分的。关键字参数通常是可选参数。例如，print()函数具有可选参数end和spe两个可选参数.end这个参数可以指定在其结尾换行或继续打印。spe参数则可以在多个参数之间打印一些特殊字符如逗号等。当你运行下面的程序：  
print('Hello')  
print('World')  
the output would look like this:  
运行结果如下：  
Hello  
World  

The two strings appear on separate lines because the print() function automatically adds a newline character to the end of the string it is passed. However, you can set the end keyword argument to change this to a different string. For example, if the program were this:  
这两个字符串出现在不同的行上，因为print（）函数会自动添加一个换行符在字符串的结尾。但是，您可以将end关键字参数更改为不同的字符串。
例如，如果程序是这样的:  
print('Hello', end='')    
print('World')    
the output would look like this:  
程序运行结果是两个字符在同一行。  
HelloWorld  

The output is printed on a single line because there is no longer a new-line printed after 'Hello'. Instead, the blank string is printed. This is useful if you need to disable the newline that gets added to the end of every print() function call.  
输出显示在一行，因为不再有换行符在“Hello”打印之后。取而代之的是空字符串。如果你需要禁用每一个print（）函数调用结束的换行符，这是非常有用的。  

Similarly, when you pass multiple string values to print(), the function will automatically separate them with a single space. Enter the following into the interactive shell:  
同样，当你使用print（）函数打印多个字符串值，该功能会自动将这些用一个空格分开。输入以下内容：  
print('cats', 'dogs', 'mice')    
cats dogs mice  

But you could replace the default separating string by passing the sep keyword argument. Enter the following into the interactive shell:  
但是你可以通过传递sep关键字参数替换默认的分隔字符串。在交互窗体输入以下代码：  
print('cats', 'dogs', 'mice', sep=',')    
cats,dogs,mice  

You can add keyword arguments to the functions you write as well, but first you’ll have to learn about the list and dictionary data types in the next two chapters. For now, just know that some functions have optional keyword arguments that can be specified when the function is called.  
您可以添加关键字参数给你写的函数，但首先你必须在接下来的两个章节学习列表类型和字典数据类型。现在你只需要知道一些函数在被调用时可以指定可选关键字参数。  

## Local and Global Scope  
## 局部和全局范围  
## https://youtu.be/M-CoVBK_bLE对应的教学视频    

Parameters and variables that are assigned in a called function are said to exist in that function’s local scope. Variables that are assigned outside all functions are said to exist in the global scope. A variable that exists in a local scope is called a local variable, while a variable that exists in the global scope is called a global variable. A variable must be one or the other; it cannot be both local and global.  
在函数被调用时才赋值的参数和变量其作用范围为局部范围，这样的参数和变量我们称为局部参数和局部变量。在全部函数外部被赋值的变量其作用范围为全局范围，这样的变量我们称为全局变量。一个变量的作用范围必须是全局或局部的一种，一个变量不能既是全局变量又是局部变量。  
  
Think of a scope as a container for variables. When a scope is destroyed, all the values stored in the scope’s variables are forgotten. There is only one global scope, and it is created when your program begins. When your program terminates, the global scope is destroyed, and all its variables are forgotten. Otherwise, the next time you ran your program, the variables would remember their values from the last time you ran it.  
思考一下变量的作用范围。当一个作用范围被破坏，储存在范围内的变量的所有值都清空了。Python中只有一个全局范围，在你的程序开始时生成。当你的程序终止时全局范围被破坏，它的所有变量将清空。否则，你程序下一次运行时，变量就会调出它最后一次运行时被赋值它们的值。  

A local scope is created whenever a function is called. Any variables assigned in this function exist within the local scope. When the function returns, the local scope is destroyed, and these variables are forgotten. The next time you call this function, the local variables will not remember the values stored in them from the last time the function was called.  
每当函数被调用时都会创建局部作用范围。任何在函数内部被赋值的变量都是局部范围。当函数返回时，局部范围被破坏，这些变量就被清空。当你下次调用这个函数的时候局部变量不会记得上次函数调用时存储的值。  

Scopes matter for several reasons:
Code in the global scope cannot use any local variables.
However, a local scope can access global variables.
Code in a function’s local scope cannot use variables in any other local scope.
You can use the same name for different variables if they are in different scopes. That is, there can be a local variable named spam and a global variable also named spam.  
他们之间有以下关系：  
全局范围内的代码不能使用任何局部变量。    
但是，局部变量可以范围全局变量。  
一个函数内部的代码不能使用另外的局部变量。  
如果变量的作用范围是不一样的那么你可以使用相同的名字来命名不同的变量。也就是说允许一个局部变量命名为spam和一个全局变量也命名为spam。  

The reason Python has different scopes instead of just making everything a global variable is so that when variables are modified by the code in a particular call to a function, the function interacts with the rest of the program only through its parameters and the return value. This narrows down the list code lines that may be causing a bug. If your program contained nothing but global variables and had a bug because of a variable being set to a bad value, then it would be hard to track down where this bad value was set. It could have been set from anywhere in the program—and your program could be hundreds or thousands of lines long! But if the bug is because of a local variable with a bad value, you know that only the code in that one function could have set it incorrectly.    
python使用不同作用范围来代替把所有变量都定义成全局的原因是，当一个变量被特定的函数调用赋值后，这个函数与其他代码的交互和作用只能通过参数和其返回值进行。在python中不当的代码缩进可能造成Bug。如果你的程序中只有一个因为全局变量被错误赋值造成的Bug，那么要找出这个错误赋值出现在什么地方是很困难的。因为你的程序有成百上千行代码这个赋值可能在任何地方出现。相反地，如果是局部变量被错误赋值造成的Bug，你只需要去调用这个局部变量所在函数的地方进行修正就可以了。  

While using global variables in small programs is fine, it is a bad habit to rely on global variables as your programs get larger and larger.  
在小程序中使用全局变量是不会有什么问题的，当您的程序变得越来越长时依靠全局变量就是一个坏习惯了。  

### Local Variables Cannot Be Used in the Global Scope
### 局部变量不能用在全局范围  

Consider this program, which will cause an error when you run it:
思考下运行下面这个程序时，将出现什么错误：
def spam():  
    eggs = 31337  
spam()  
print(eggs)   
If you run this program, the output will look like this:  
如果你运行这个程序会输出如下的错误提示：
Traceback (most recent call last):  
  File "C:/test3784.py", line 4, in <module>  
    print(eggs)  
NameError: name 'eggs' is not defined  

The error happens because the eggs variable exists only in the local scope created when spam() is called. Once the program execution returns from spam, that local scope is destroyed, and there is no longer a variable named eggs. So when your program tries to run print(eggs), Python gives you an error saying that eggs is not defined. This makes sense if you think about it; when the program execution is in the global scope, no local scopes exist, so there can’t be any local variables. This is why only global variables can be used in the global scope.  
因为变量eggs只能在spam()被调用时创建，他的作用范围是局部范围所以会发生错误。当程序运返回spam时，局部作用范围已经破坏。在变量eggs中不存在任何值。所以尝试用print(eggs)来打印python会报告eggs没有被定义的错误。，如果你仔细想想，这是有道理的。当程序在全局范围内运行时，无局部范围存在，所以不能有任何局部变量。这就是为什么全局变量只可以在全局范围内使用。  

###　Local Scopes Cannot Use Variables in Other Local Scopes
### 局部作用范围不能使用其他函数局部变量  

A new local scope is created whenever a function is called, including when a function is called from another function. Consider this program:  
每当函数被调是将创建一个新的局部范围建，包括一个函数从另一个函数调用时。思考下面的程序：  
  def spam():  
➊    eggs = 99  
➋    bacon()  
➌    print(eggs)  
  def bacon():  
      ham = 101  
➍    eggs = 0  
➎ spam()  W
hen the program starts, the spam() function is called ➎, and a local scope is created. The local variable eggs ➊ is set to 99. Then the bacon() function is called ➋, and a second local scope is created. Multiple local scopes can exist at the same time. In this new local scope, the local variable ham is set to 101, and a local variable eggs—which is different from the one in spam()’s local scope—is also created ➍ and set to 0.  
当程序运行时，函数spam()被调用，局部范围被创建。局部变量eggs被赋值99当函数bacon()b被调用是第二个局部范围被创建。两个局部范围同时存在。在新的局部范围内，局部变量ham被赋值101，第二个局部变量eggs不同于函数spam(）中的eggs并且被赋值0.  
When bacon() returns, the local scope for that call is destroyed. The program execution continues in the spam() function to print the value of eggs ➌, and since the local scope for the call to spam() still exists here, the eggs variable is set to 99. This is what the program prints.The upshot is that local variables in one function are completely separate from the local variables in another function.  
当bacon()函数返回时局部范围被破坏。程序继续执行spam()函数并打印eggs的值，因为最开始创建的局部范围还存在，所以eggs的被赋值99。这就是程序运行打印的结果。其结果是，在一个函数中的局部变量是和另一个函数中的局部变量完全独立。  

### Global Variables Can Be Read from a Local Scope  
### 全局变量可以被局部变量读取  

Consider the following program:  
思考下面的程序:  
def spam():  
    print(eggs)  
eggs = 42  
spam()  
print(eggs)  
Since there is no parameter named eggs or any code that assigns eggs a value in the spam() function, when eggs is used in spam(), Python considers it a reference to the global variable eggs. This is why 42 is printed when the previous program is run.  
由于参数eggs在函数spam()中没有任何定义，当在函数spam()中用到eggs参数时，Python会认为变量eggs是一个全局变量。这就是是为什么程序运行打印出来的值是42  

### Local and Global Variables with the Same Name
### 局部变量和全局变量可以具有相同的名称  



