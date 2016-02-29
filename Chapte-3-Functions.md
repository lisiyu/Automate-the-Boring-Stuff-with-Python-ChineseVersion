# Functions
## https://youtu.be/WB4hJJkfhLU相应的视频教程

 You’re already familiar with the print(), input(), and len() functions from the previous chapters. 
 Python provides several builtin functions like these, but you can also write your own functions. 
 A function is like a mini-program within a program.

 在前面的章节你已经熟悉的print()，input()和len()函数。
 Python提供了一些这样的内建函数，你也可以编写自己的函数。
 函数就像一个程序中的一个小程序。

 To better understand how functions work, let’s create one. Type this program into the file editor and save it as helloFunc.py:

 理解函数的工作原理的最好方法是我们创建一个试试。在文件编辑器里面输入这段代码到并保存为helloFunc.py：

def hello():
	print('Howdy!')
	print('Howdy!!!')
	print('Hello there.')
hello()
hello()
hello()

 The first line is a def statement [1], which defines a function named hello().
 The code in the block that follows the def statement[2]， is the body of the function. 
 This code is executed when the function is called, not when the function is first defined.

 第一行的def我们成为函数声明语句。def为函数声明关键词。我们将这个函数名称定义为hello.
 紧跟着函数声明语句的代码块我们成为函数体。
 当函数被调用的时候函数的代码才会执行，而不是在首次定义函数的时候执行该代码。

 The hello() lines after the function are function calls. In code,  a function call is  just the  function’s name 
 followed by  parentheses, possibly with some number of arguments in between the parentheses.  When the  program execution
 reaches these  calls, it  will jump  to the  top line  in the function and begin executing the code there. When it reaches the end 
 of the function, the execution eturns to the line  that called the function  and continues moving through  the code as before. 
 Since  this program calls hello()  three times, the code  in the hello() function is executed three times. When you run this program, 
 the  output looks like this:

Howdy!
Howdy!!!
Hello there.
Howdy!
Howdy!!!
Hello there.
Howdy!
Howdy!!!
Hello there.

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

In general, you always want to avoid duplicating code, because if you ever decide to update the code—if, for example, you find a bug you need to fix—you’ll have to remember to change the code everywhere you copied it.

一般情况下，你总是希望避免重复的代码。举个例子，当你发现程序片段中有bug需要修复，你需要记得把你到处复的所有代码中的错误都进行修复。这是很痛苦的。

## def Statements with Parameters
## 带参数的函数声明语句 def

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

The definition of the hello() function in this program has a parameter called name .A parameter is a variable that an argument is stored in when a function is called. The first time the hello() function is called, it’s with the argument 'Alice'. The program execution enters the function, and the variable name is automatically set to 'Alice', which is what gets printed by the print() statement.
我们在这段代码中定义Hello（）函数有一个参数叫name。当函数被调用时该参数被当成一个变量存储在函数中。当第一次调用Hello（）函数时它被赋值为‘Alice'.当程序执行时，变量name就被自动赋值为'Alice'并且能够传递给print()函数。

One special thing to note about parameters is that the value stored in a parameter is forgotten when the function returns. For example, if you added print(name) after hello('Bob') in the previous program, the program would give you a NameError because there is no variable named name. This variable was destroyed after the function call hello('Bob') had returned, so print(name) would refer to a name variable that does not exist.
需要注意的是参数有一个特别之处，当函数返回时存储在一个参数的值将被清空。举例，在前面的程序中如果你在hello('Bob')后添加代码print（name)，程序会报NameError错误，因为变量name没有被赋值。name的值在函数调用hello('Bob')返回后就被清空了。所以print(name)将指向一个不存在值的变量name。

This is similar to how a program’s variables are forgotten when the program terminates. I’ll talk more about why that happens later in the chapter, when I discuss what a function’s local scope is.

这类似于程序终止时，程序的变量被清空。在后面的章节中讲到函数的局部范围时我们在做更多地讨论。

## Return Values and return Statements
## 返回值和返回语句
