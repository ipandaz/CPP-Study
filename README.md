# C++零基础学习记录
记录知识盲点

## 1. 基础知识

### 1.1 信息的储存单位
* 位（bit,b)
> 数据的最小单位，表示一位二进制信息
* 字节(byte,B)
> 八位二进制数字组成（1byte=8bit）

### 1.2 R进制缩写
* 二进制：BIN
* 八进制：OCT
* 十进制：DEC
* 十六进制：HEX

### 1.3 R进制->十进制
各位数字与它的权相乘，其积相加
> 例：二进制的1111<sub>2</sub>转换成十进制  
1×2<sup>3</sup>+1×2<sup>2</sup>+1×2<sup>1</sup>+1×2<sup>0</sup>=8+4+2+1=15<sub>10</sub>

### 1.4 十进制整数->R进制整数
除以R取余
> 例：十进制的68<sub>10</sub>转换成二进制  
68/2=34(余数0）  
34/2=17(余数0）  
17?2=8(余数1）  
……  
1/2=0(余数1）  
低位->高位  
得：1000100<sub>2</sub>

### 1.5 十进制小数->R进制小数
乘以R取整
> 例：十进制的0.3125<sub>10</sub>转换成二进制  
0.3125×2=0.625  
0.625×2=1.25  
0.25×2=0.5  
0.5×2=1.0  
高位->低位  
得：0.0101<sub>2</sub>

### 1.6 模数
n位二进制整数的模数为2<sup>n</sup>  
n位小数的模数为2

### 1.7 补数
一个数减去另一个数（加一个负数）  
等于第一个数加第二个数的补数
> 例：8+(-2)=8+10(mod 12)=6

### 1.8 反码的计算规则
1. 负整数：  
原码符号位不变（仍是1）  
其余各位取反（0变1，1变0）
> 例：X=-1100110  
X<sub>原</sub>=11100110  
X<sub>反</sub>=10011001
2. 正整数：原码就是补码

### 1.9 补码的计算规则
反码：作为中间码  
> 负数补码=反码+1  
正数补码=原码

## 2. 标识符
### 2.1 标识符的构成规则
* 以大写字母、小写字母活下划线开始
* 可以由以大写字母、小写字母、下划线或数字0~9组成
* 大写字母和小写字母代表不同标识符
* 不能是C++关键字或操作符




