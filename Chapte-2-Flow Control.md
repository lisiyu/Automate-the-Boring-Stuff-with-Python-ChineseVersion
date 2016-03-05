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
