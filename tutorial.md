# pinelang语法教程文档

## 目录

1.语言结构

> 注意

2.基本语法

> 关键字导入部分的语法

>> 所有的关键字

>> 注意

> 主程序部分的语法

>> 注意

> 输出语法

> 数据类型

>> 注意

> 输入语法

3.条件语句

> 语法

4.循环语句

> 语法

5.示例合集

## 一，语言结构

本语言由两部分构成，分别是

* 关键字导入部分
* 主程序部分

整个程序由`BEGINALL`开始，由`ENDALL`结束

关键字导入部分由`BEGINKEYWD`开始，由`ENDKEYWD`结束

主程序部分由`BEGINMAIN`开始，由`ENDMAIN`结束

### 注意

* 开始结束的标识必须大写且位于行首不留空格

## 二，基本语法

### 关键字导入部分的语法

在主程序中需要用到的关键字，需要在此部分导入，否则无法运行

导入关键字的语法

```
import keyword
```

#### 所有的关键字

```
out,int,dec,str,input,if,for,break
```

#### 注意

* 以`import`开头，后接一个空格再写关键字
* `import`位于行首不留空格
* 一个`import`只能导入一个关键字
* 所有的关键字都是小写

### 主程序部分的语法

每一行代码都由关键字和它的方法或参数组成

例如输出代码

```
BEGINALL

BEGINKEYWD
import out
ENDKEYWD

BEGINMAIN
out(“hello world”){}
ENDMAIN

ENDALL
```

可以看出，基本格式为

```
keyword(参数，可以不写){
附属代码块，可以不写
}
```

#### 注意

* 每一行都要写在行首不留空格
* 关键字与括号和括号与大括号之间不留空格
* 如果有附属代码块，要换行，一行一条代码

### 输出语法

```
out(内容){}
```

小括号里的内容只有两种

1.字符串，用英文双引号引起来

2.变量名，下面会说如何使用

### 数据类型

数据类型一共有三种

1.整数

2.小数（浮点数）

3.字符串或字符

整数定义

```
int 变量名=变量值
```

小数（浮点数）定义

```
dec 变量名=变量值
```

字符串或字符定义

```
str 变量名=“变量值”
```

#### 注意

* 以`int`或`dec`或`str`开头，后接一个空格再写变量名
* `int`或`dec`或`str`位于行首不留空格
* 等号两边不留空格
* 变量名全小写

调用或修改变量

输出示例

```
out([变量名]){}
```

修改

```
[变量名]=新变量值
```

注意事项和定义一致

### 输入语法

```
input(提示语句){
在此定义一个变量或放一个[变量名]
}
```

注意事项和输出语法一致

## 三，条件语句

### 语法

```
if(表达式，只能+-*/><=){
语句块
}else{
语句块
}
```

通过上面的文档我们可以看出，整个程序每一行都位于行首不留空格，其它的没有什么要注意的

## 四，循环语句

### 语法

```
for(表达式，只能+-*/><=){
语句块
}

break跳出循环
```

当表达式成立吋才继续循环

## 示例合集

这是我写的一份代码，可以在`code/`目录找到这个源码文件，包含了全部的语法和全部的关键词

代码如下

```
BEGINALL

BEGINKEYWD
import out
import int
import dec
import str
import input
import if
import for
import break
ENDKEYWD

BEGINMAIN
out(“猜数字游戏”){}
int realnumber=25
int your=0
int i=0
dec times=0.00
str onestr=“对了”
str twostr=“错了”

for(i<10){

input(“请输入”){
[your]
}

if([your]=[realnumber]){
out([onestr]){}
break
}else{
out([twostr]){}
[times]=[times]+1
}

}
out([times]){}
ENDMAIN

ENDALL
```
