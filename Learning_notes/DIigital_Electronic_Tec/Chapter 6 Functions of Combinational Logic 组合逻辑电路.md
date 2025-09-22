
# 6.1 Half and Full Adders 


## 6.1.1 half-adder

- 回想第二章的运算规则：
>[!note] 异或的法则
>0 + 0 = 0
>0 + 1 = 1
>1 + 0 = 1
>1 + 1 = 10

This operations are performed by a logic called a half-adder.

![[Screenshot_2025-03-13-21-24-17-098_md.obsidian.png]]

1. $C_{out} = AB$
2. $\sum = A\oplus B$  
3. 用于处理两个一位的二进制数相加，输出包括和输出以及进位输出



![[Screenshot_2025-03-13-21-28-21-897_com.jideos.jnotes.png]]


### 6.1.2 全加法器

1. Composed of two half-adders, it receives two inputs and an input carry and generates an sum output and an output carry.
![[Screenshot_2025-03-13-21-34-01-779_md.obsidian.png]]

2.  运算规则：
$$\Sigma = (A \oplus B) \oplus C_{in}$$
>[!note] 对于加法器的简单理解
实际上，加法器就是手算的过程，例如A＝1，B＝1  $C_{in}$=1,
那么结果是，11，所以最右边的位置是$\sum=1,C_{out} = 1$ 


$$C_{out} = AB + (A \oplus B)C_{in} $$

# 6.2 Parallel Binary Adders 

**Clearly,两个或多个Full adders 组合起来便成为了Parallel Binary Adders.

由于一个加法器可以解决1-bit的二进制数字相加，那么相应的**2-bit二进制数字需要两个Full-Adders组成**。




