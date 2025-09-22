
# 6.1 字典

简介：
字典是无序的，可变的，保存的内容是以**键-值对**的形式储存的。

- [!] 通过键，而不是索引读取，字典有时被称为关联数组或者散列表(hash table)
- [1] 字典是任意对象的无序集合。字典是无序的。
- [！] 字典是可变的并且可以任意嵌套可以在原处增长或者缩短(无需生成副本)，并且它支持任意深度的嵌套（即他的值可以是列表或者其他的字典）
- [去] 字典的键，==必须唯一==，假如出现两次，那么将记住后一次的值。。
- [！] 字典中的键，不可变，所以可以使用数字，字符串或者元组。但是不能是列表。


## 6.1.1 字典的创建和删除

语法格式：
```python 
dictionary = {'key1':'value1','key2':'value2',...,'keyn':'valuen'}
```

**参数说明：
1. dictionary:字典名称。
2. key: 表示元素的键，必须是唯一的。
3. value：表示元素的值。

**空字典的创建

```python 
dictionary = {}
#OR
dictionary = dict{}
```

`dict()`方法不仅可以创建一个空字典，同时还可以通过已有的数据快速创建字典，主要表现为以下的形式：

### 1. 通过映射函数创建字典


语法格式：
```python 
dictionary = dict(zip(list1,list2))
```
参数说明：
- [1] zip()函数:用于将**多个列表或者元组对应位置的元素组合为元组**，并且返回这些内容的zip对象。如果想得到元组，可以使用`tuple()`函数将zip对象转化为元组 ,if you wanna get a list ,just use list() to switch it to list 
- [!] list1:  a list ,用于指定要生成字典的key
- [!] list2: a list ,用于要生成字典的值


E.G.

```python
name = ['jerry','mike','Simson']
sign = ['big guy','smoke','bad ass']

```


# 6.2 集合

The set in python is similar to the set in math, they are both used to save different elements.

Therefore, it's easy to  know when to use it: when you need to find the same element in the array, just use it 


## To create a set

### 1. directly use "{}"  to create one 

```python
setname = {elem1,elem2,...,elem n}
```

**when you input repeat element Python will just keep only one**

