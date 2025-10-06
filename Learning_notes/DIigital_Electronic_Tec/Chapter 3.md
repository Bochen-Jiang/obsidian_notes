## **Objective** :
- **Basic Gates : AND, OR, NOT** 
- **Extended Gates : NAND, NOR, Exclusive-OR, Exclusive-NOR Gate**
- **Symbols**

## Gate(门)
![[微信图片_20250301210942.jpg]]
###  The Inverter (反相器， NOT Gate 非门）


- 上面的三角形，Negation(取反符号)，后面的bubblle代表反向的意思，之后的反向的Gate会经常用到

- 取反符号出现的地方，代表着0的存在是active的，即LOW is active,
对于没有bubble的地方(input or output )，HIGH 才是active

- Polarity(极性指示符) is similar to the Negation,与取反符号的规则类似。
- 
- The Inverter performs as the Boolean NOT  operration.When the input is LOW, the output is HIGH,and when the input is HIGH, the output is LOW.

- Timing Diagrams: **理论上**,两者的变化完全相反，但是由于时间延迟的影响，会有一点不同，假设输出为X ，输入为A，那么经过inverter后，X ＝ $\overline{A}$  (just an overbar)



### The AND Gate（与门）


![[815ef7b7031448d4db48a4d46305346d_MD5.jpeg]]


#### The Operation For AND Gate 

| input  | input  | output |
| ------ | ------ | ------ |
| *HIGH* | *HIGH* | *HIGH* |
| *LOW*  | *HIGH* | *LOW*  |
| *HIGH* | *LOW*  | *LOW*  |
| *LOW*  | *LOW*  | *LOW*  |

#### The Logic Expressions For AND Gate 

- The AND gate operation is usually shown with a dot between the variables but it may be implied(not dot). Thus, the AND operation is written as $X=A·B$  or   $X = AB$ (逻辑学上的乘积)

#### Some comprrhension

- The AND operation is used  in computer programming as a *selective mask*. If you want to retain certain bits of a binary number, but reset the other numbits to 0, you could set a mask with 1's in the position of the retained bits.(大致的意思就是说，AND这个语句可以选择某些特定的位置，这被称为selective mask,例如我希望选择某个8位的二进制数的前3位，而消去其后5位，那么只需要将它和11100000相加即可)

- Example of seletive mask:Marking an IP address on the Internet 
	- When an **IP address** is masked with the subnet work,host specific bits are masked off (becomes 0s),so we will be able to tell which subnet hte host is.
	- 作用：高效识别编码所具有的特性，在上述的例子中，我们只需要知道后16位就可以识别是否为本地数据。


### The OR Gate (或门) 



[[04222fea18053be06ed01355ab19d802_MD5 1.jpeg]]
![[04222fea18053be06ed01355ab19d802_MD5 1.jpeg]]
#### The Operation For OR Gate 

| input  | input  | output |
| ------ | ------ | ------ |
| *HIGH* | *HIGH* | *HIGH* |
| *LOW*  | *HIGH* | *HIGH* |
| *HIGH* | *LOW*  | *HIGH* |
| *LOW*  | *LOW*  | *LOW*  |
#### The Logic Expression For OR Gate 
- For OR Gate, it just like the "+" operation in logic,$X=A+B$


#### Some comprehension

- The OR op can be used in computer programming to set certain bits of a binary number to 1.(和AND Gate 一样可以用作selective mask 只不过是将所有的数字变成1) 






### The NAND Gate (与非门) 


![[277b748ca87ff925d91f1d9dcde9ac51_MD5.jpeg]]

- Easy to see, the NAND Gate is just the addition of **an AND Gate** and **an inverter**, or **the rectangular outline**.

| input  | input  | output |
| ------ | ------ | ------ |
| *HIGH* | *HIGH* | *LOW*  |
| *LOW*  | *HIGH* | *HIGH* |
| *HIGH* | *LOW*  | *HIGH* |
| *LOW*  | *LOW*  | *HIGH* |
[[Chapter 3#The AND Gate（与门）]]To compare with AND Gate


![[74db0c4bb2eb76d30d5da7a06fe51fa0_MD5.jpeg]]

- just like the pic up,first you negative it (1 to 0, 0 to 1)
and then you "OR" it.

#### **THE Logic Expression For NAND Gate**

- The Boolean expression for NAND Gate is $$X = \overline{AB}$$