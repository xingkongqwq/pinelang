# pinelang

一门独创的编程语言，基于`C`和`Python`，后缀名是`.pine`

## 安装此项目

* `git clone https://github.com/ohfxpine/pinelang.git`
* `cd pinelang/`
* `sh build.sh`

## 如何使用

1.编写`.pine`源码放到`code/`目录里

2.运行`change/main.py`，需要输入文件名，例如`hello.pine`

3.运行`run/main.sh`,需要输入文件名，例如`hello.pine`

4.如果没有报错，会在`bin/`目录生成`a.out`或`a.exe`

5.`bin/`目录生成的可直接运行，脱离`Python`,`C`,`pinelang`环境

6.用完记得清空`bin/`和`temp/`目录，以免报错

如果你觉得太麻烦，可以运行`edit_and_translate.sh`，一步到位，自动清理编译产生的缓存文件并编译

## 语言教程

详见`tutorial.md`
## 项目构架

* change

> 语言转换有关

> 将`.pine`转换为`.c`

* run

> 运行有关

> 把`.c`转为`.out`并运行的场所

* code

> `.pine`代码存方的位置

> 必须把写好的`.pine`代码放到此文件夹

* bin

> 编译结果存放

> 存放`.out `文件的场所

* temp

> 缓存文件存放

> 存放`.c `文件的场所

## 参与贡献

* ohfxpine

## 其它

我（ohfxpine）现在是一名初二学生，没有太多时间维护和编写，如有问题或意见，可以[留言](https://ohfxpine.mysxl.cn)
