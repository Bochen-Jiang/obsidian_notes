# 4.2 选择语句

## 最简单的if语句

```python 
if 表达式
	语句块
```
表达式可以是一个单纯的布尔值或者变量，类似于“如果……就……”

给出一个例子：
```python 
print("今有物不知其数，三三数之剩二，五五数之剩三，七七数之剩二，问几何?\n”)
number =  int(input("请输入您认为符合条件的数：")) # 输入一个数
if number%3==2 and number%5==3 and number%7==2
	print(number,"符合条件：三三数之剩二，五五数之剩三，七七数之剩二")
```

>[!warning]
>注意，在if语句多于else语句时，会根据缩进来判断else所从属的if
>```python 
>a = -1
>if a >= 0:
>	if a>0:
>		print("a is a positive number")
>	else
>		print("a is a negative number")
>		```



## 4.2.3 if...elif...else 语句
语法格式如下：
```python 
if 表达式1：
	语句块
elif 表达式2：
	语句块
elif 表达式3：
	语句块
···
else 
	语句块n
```

>[!warning]
>注意，**在使用布尔类型时，应当使用下列规范形式：(假设flag是布尔变量)**
>```python 
>if flag :
>if not flag:
>```
>而不是
>```python 
>if flag == True:
>if flag == False:
>```



## 4.3 循环语句

### 4.3.1 while循环

格式如下：
```python
while 条件表达式
	循环体
```



还是黄蓉的题目：
```python 
print("今有物不知其数，三三数之剩二，五五数之剩三，七七数之剩二，问几何?\n”)
none = True 
number = 0
while none:
	number += 1
	if number%3==2 and number%5==3 and number%7==2：
		print ("答曰：这个数是："，number)
		none = False
```


>[!warning]
>！！一定要注意：**在使用while循环的时候，一定要添加将循环变成False的条件**

### 4.3.2 for 循环

格式：
```python 
for 迭代变量 in 对象
	循环体
```

1. 进行数值循环

例如，想要实现1到100的累加：

```python 
print("1到100的加和为：")
result = 0    # 保存累加结果的变量
for i in range(101):
result +=i
print(result)
```

其中，range()函数是Python内置的函数，用来生成整数

其格式为：
range(start,end,step)

解释：
- start :是数字的开始，不写默认为0
- end：结束的数字，**但是不包括该数字本身**
- step：两个数之间的间隔，如果不写那就默认为1。



2. 遍历字符串

```python 
string = '不要再说我不能'
print(string)
for i in string
	print(string)
```
结果：
```python
不要再说我不能
不
要
再 
说
我
不
能
```

## 4.4 break,continue,和pass语句

### 4.4.1 break 语句

break 语句可以终止当前的循环。

**一般会搭配if语句使用，表示达到某个条件循环结束。**

###  4.4.2 continue 语句

continue语句没有break语句那么强大，continue语句只是跳出当前一次循环。

### 4.4.3 pass 语句

在python 中,pass 语句表示空语句，他**不做任何事情**,只起到==占位作用==。

