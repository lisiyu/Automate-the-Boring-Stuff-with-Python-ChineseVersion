# list 列表
## [相关视频教程](https://youtu.be/5n6o1MaXDoE)

One more topic you’ll need to understand before you can begin writing programs in earnest is the list data type and its cousin, the tuple. Lists and tuples can contain multiple values, which makes it easier to write programs that handle large amounts of data. And since lists themselves can contain other lists, you can use them to arrange data into hierarchical structures.  
在你真正开始编写程序还有一个重要项目需要明白,这就是列表数据类型和他的表弟，定值列表。列表和定值列表可以包含多个值，这使得它更容易编写处理大量数据的程序。而且，由于列表内部可以包含其他列表，你可以用它们来进行数据排序操作.    
In this chapter, I’ll discuss the basics of lists. I’ll also teach you about methods, which are functions that are tied to values of a certain data type. Then I’ll briefly cover the list-like tuple and string data types and how they compare to list values. In the next chapter, I’ll introduce you to the dictionary data type.  
在本章中，我们将学习列表的基础知识。我也会教你使用函数把数值绑定到某一数据类型的方法.然后，我将简要介绍和列表数据类型类似的定值列表和字符串数据类型，以及他们和列表数据类型的区别.在下一章中，我将向您介绍字典数据类型.  

## The List Data Type 列表数据类型

A list is a value that contains multiple values in an ordered sequence. The term list value refers to the list itself (which is a value that can be stored in a variable or passed to a function like any other value), not the values inside the list value. A list value looks like this: ['cat', 'bat', 'rat', 'elephant']. Just as string values are typed with quote characters to mark where the string begins and ends, a list begins with an opening square bracket and ends with a closing square bracket, []. Values inside the list are also called items. Items are separated with commas (that is, they are comma-delimited). For example, enter the following into the interactive shell:  
列表是包含多个有序序列值的值。术语'列表值'指的是列表本身（这可以存储在一个变量中或像任何其他函数的值一样可以传递），而不是指列表内的元素的值。一个列表的值看起来像这样:['cat', 'bat', 'rat', 'elephant'].他是以左方括号开始中间用引号引起来的区分每个字符串开始和结尾,字符串之间用逗号隔开并以右方括号结束.列表内的值也被称为项目。项目之间用逗号分开（也就是说，它们是用逗号分隔）。例如，输入以下内容到交互窗体：  

	>>> [1, 2, 3]
	   [1, 2, 3]
	   >>> ['cat', 'bat', 'rat', 'elephant']
	   ['cat', 'bat', 'rat', 'elephant']
	   >>> ['hello', 3.1415, True, None, 42]
	   ['hello', 3.1415, True, None, 42]
	>>> spam = ['cat', 'bat', 'rat', 'elephant']
	   >>> spam
	   ['cat', 'bat', 'rat', 'elephant']

The spam variable is still assigned only one value: the list value. But the list value itself contains other values. The value [] is an empty list that contains no values, similar to '', the empty string.  
变量spam还是只分配了一个值：列表值。但列表值本身包含其他值。列表[]不包含任何值，类似于''空字符串/我们成为空列表。

## Getting Individual Values in a List with Indexes
## 用索引来访问列表中的项目值

Say you have the list ['cat', 'bat', 'rat', 'elephant'] stored in a variable named spam. The Python code spam[0] would evaluate to 'cat', and spam[1] would evaluate to 'bat', and so on. The integer inside the square brackets that follows the list is called an index. The first value in the list is at index 0, the second value is at index 1, the third value is at index 2, and so on. Figure 4-1 shows a list value assigned to spam, along with what the index expressions would evaluate to.  
假设你有一个列表['cat', 'bat', 'rat', 'elephant']存储在一个变量spam中.Python代码会将spam[0]值识别为为“cat”，spam[2]识别为“bat”，依此类推。列表中方括号内的整数称为索引.列表中的第一个值是在索引0，第二个值是在索引1中，第三个值是在索引2，依此类推.图4-1显示分配给spam列表的值及对应索引表达式。  
![图4-1](https://automatetheboringstuff.com/images/000074.png)
> Figure 4-1. A list value stored in the variable spam, showing which value each index refers to  

For example, type the following expressions into the interactive shell. Start by assigning a list to the variable spam.  
例如，键入下面的表达式到交互窗体。给变量spam赋值一个列表开始。  

	   >>> spam = ['cat', 'bat', 'rat', 'elephant']
	   >>> spam[0]
	   'cat'
	   >>> spam[1]
	   'bat'
	   >>> spam[2]
	   'rat'
	   >>> spam[3]
	   'elephant'
	   >>> ['cat', 'bat', 'rat', 'elephant'][3]
	   'elephant'
	(1) >>> 'Hello ' + spam[0]
	(2)'Hello cat'
	   >>> 'The ' + spam[1] + ' ate the ' + spam[0] + '.'
	   'The bat ate the cat.'
	   
Notice that the expression 'Hello ' + spam[0] ➊ evaluates to 'Hello ' + 'cat' because spam[0] evaluates to the string 'cat'. This expression in turn evaluates to the string value 'Hello cat'   
请注意，表达“Hello”+spam[0](1)计算结果为'Hello'+'cat'，因为spam[0]计算得到字符串'cat'。这个表达式的字符串值“Hello cat"  
Python will give you an IndexError error message if you use an index that exceeds the number of values in your list value.  
如果使用超过列表值的值数的索引Python将会给你一个IndexError错误消息.  

	>>> spam = ['cat', 'bat', 'rat', 'elephant']
	>>> spam[10000]
	Traceback (most recent call last):
	  File "<pyshell#9>", line 1, in <module>
		spam[10000]
	IndexError: list index out of range

Indexes can be only integer values, not floats. The following example will cause a TypeError error:  
索引只能是整数值，不能是浮点数。下面的例子将导致一个TypeError错误

	>>> spam = ['cat', 'bat', 'rat', 'elephant']
	>>> spam[1]
	'bat'
	>>> spam[1.0]
	Traceback (most recent call last):
	  File "<pyshell#13>", line 1, in <module>
		spam[1.0]
	TypeError: list indices must be integers, not float
	>>> spam[int(1.0)]
	'bat' 
	 
Lists can also contain other list values. The values in these lists of lists can be accessed using multiple indexes, like so:  
列表还可以包含其他列表值。在列表中的这些列表值可以使用多个索引，像这样来访问：
  
	>>> spam = [['cat', 'bat'], [10, 20, 30, 40, 50]]
	>>> spam[0]
	['cat', 'bat']
	>>> spam[0][1]
	'bat'
	>>> spam[1][4]
	50
	
The first index dictates which list value to use, and the second indicates the value within the list value. For example, spam[0][1] prints 'bat', the second value in the first list. If you only use one index, the program will print the full list value at that index.   
第一索引指示要使用哪个列表值，第二表示列表值内的值。例如，spam[0] [1]打印“bat”，他是第一个列表中的第二个值.如果您只使用一个索引，该程序将打印索引处的完整列表值。  

## Negative Indexes 负索引

While indexes start at 0 and go up, you can also use negative integers for the index. The integer value -1 refers to the last index in a list, the value -2 refers to the second-to-last index in a list, and so on. Enter the following into the interactive shell:  
虽然索引从0开始增加，你也可以使用负整数的索引。整数值-1指的是在一个列表中的最后一个索引，值-2是指列表中倒数第二个值的索引，依此类推.输入以下内容到交互窗口： 
 
	>>> spam = ['cat', 'bat', 'rat', 'elephant']
	>>> spam[-1]
	'elephant'
	>>> spam[-3]
	'bat'
	>>> 'The ' + spam[-1] + ' is afraid of the ' + spam[-3] + '.'
	'The elephant is afraid of the bat.'

