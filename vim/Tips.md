各种Tip
=======
## 格式化文本
Normal模式下：`gg=G`
## 录制宏
1. Normal模式下，按q+寄存器名开始录制,比如：`qa`
2. 再次按q结束录制。
3. 使用@+寄存器名执行该宏，比如：`@a`

## 显示TAB
Normal模式下:`set list`  
然后TAB会显示成`^I`，并且行尾会显示`$`，从而看出行尾空格。
## ctags插件
首先使用**ctags -R**在当前目录下生成tags文件。然后再次用vim编辑文件的时候，即可实现函数和宏跳转。  
使用`<Ctrl>-]`可以跳转到函数，宏定义处。

---------------------------------------
## 程序员技巧
### 函数相关的跳转
|按键|说明
|---|---
|[[|如果在函数体内，则跳到函数起始**{**处，如果已经再该位置则跳转到上一个函数的**{**处
|][|如果在函数体内，则跳到函数结尾**}**处，如果已经再该位置则跳转到下一个函数的**}**处
|]]|跳转到下一个函数的起始**{**处
|[]|跳到上一个函数的结尾**}**处

### 宏，变量相关
|按键|说明
|---|---
|]+i|查看变量的定义
|[+d|查看宏的定义
|g+d|跳转到变量定义处

### 查看man手册
在单词位置按**K**（`<shift>-k`）。
