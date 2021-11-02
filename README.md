# tmux

1.session  window pane 

<https://www.runoob.com/markdown/md-tutorial.html>  

ctrl + b % 左右切分当前窗格

tmux new -s 会话名（session）s -t 窗口名（windows）

[![](https://img.shields.io/badge/shield.io-github-orange)](https://github.com/Tantalus-pala?tab=repositories)




1.使用=和-标记一级标题和二级标题
====

一级标题  
====

二级标题

----



2.使用#来标记标题

使用#号可表示1-6级标题，一级标题对应一个#号，二级对应2个。以此类推 #与标题之间带空格

# 一级标题 （# 一级）

## 二级标题 （## 二级）

### 三级标题  （### 三级）

#### 四级标题 （#### 四级）

##### 五级标题  （##### 五级）

###### 六级标题   （###### 六级）





段落的换行是使用 文末加2个以上空格回车  



字体表示 :*斜体*   _斜体_ **粗体** __粗体__ ***粗斜体文本*** ___粗斜体文本___

### 分割线

你可以在一行中用三个以上的星号(*)、减号(-)、底线来建立一个分割线，行内不能有其他东西。你也可以在星号或减号中加入空格。下面每种写法都可以建立分割线：

***

---



## 删除线

如果段落上的文字要添加删除线，只需要在文字两端添加两个波浪线~~即可，实例

makedown

~~makedown~~

## 下划线

下划线可以通过HTML的<u>标签来实现<u> makedown </u>：

<u>makedown</u>

## 脚注

脚注是对文本的补充说明。 格式为[^脚注]。

[^脚注]: 类似tip的功能



## 列表

### 无序列表 无序列表使用星号（*）、加号（+）、减号（-）作为列表标记，这些标记后面要添加一个空格，然后在填写内容，实例如下

+ 第一项

+ 第二项

- 第三项



### 有序列表 使用数字加.来表示 如下

1. 第一项



## 列表嵌套

列表嵌套只需要在子列表的前面添加4个空格即可：

1. 第一项
   * 子项
2. 第二项
   + 子项
3. 第三项
   - 子项
   - 2项







## makedown区块

Makedown区块引用是在段落开头使用>符号，然后紧跟一个空格符号：

> 区块引用
>
> 菜鸟教程

另外区块也可以嵌套，一个>符号是最外层，2个>符号是一层嵌套：

> 最外层
>
> > 第二层
> >
> > > 第三层



区块中使用列表

> 1. first
>
> 2. second
>
> * third

列表中使用区块

* A

  > first
  >
  > ???

* B

  > second

* C

  > third

## Markdown代码 

如果是段落上的一个函数或片段的代码可以用反引号把它包起来（`），例如：

`print()`函数

### 代码区块

代码区块使用4个空格或者一个制表符（Tab键）。实例如下

​	<?php

​	echo 'MAKEDOWN' ;

​	function test(){

​	echo 'test';

​	}





也可以使用```包裹一段代码，并指定一种语言（也可以不指定）：

```javasc
$(document).ready(function(){
	alert("makedown");
});
```





## Makedown链接

链接使用方法如下：

[Github链接](https://github.com/Tantalus-pala?tab=repositories) 或者直接使用地址 <https://github.com/Tantalus-pala?tab=repositories>

### 高级链接

可以设置变量来设置一个链接，变量赋值在文档末尾进行：

这个链接用 1 来作为网址变量[Google][1]

![](https://img.shields.io/badge/shield.io-github-orange)



[![](https://img.shields.io/badge/shield.io-github-orange)](https://github.com/Tantalus-pala?tab=repositories)





## Makedown表格

makedown用 | 来分隔不同的单元格，用 - 来分隔表头和其他行

| 表头 |  1   |    2 |
| :--- | :--: | ---: |
|      |      |      |



对齐方式

**我们可以设置表格的对齐方式：**

- **-:** 设置内容和标题栏居右对齐。
- **:-** 设置内容和标题栏居左对齐。
- **:-:** 设置内容和标题栏居中对齐。



## makedown高级技巧

### 支持HTML元素

不在Makedown涵盖范围之内的标签都可以直接在文档里用HTML撰写

目前支持的HTML元素有：<kbd><b><i><em><sup><br> 等

使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

```
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
```

### 转义

Makedown使用了很多特殊符号来表示特定的含义，如果需要显示特定符号则需要使用转移符号，Makedown使用反斜杠转义特殊字符：

**文本加粗**

\*\*正常显示星号\*\*

\ `*_{}[]()#+-.! 这些符号可以通过反斜杠来转义

### 公式

当你需要插入数学公式时，可以使用两个$$美元符号包裹TeX或者LaTeX格式的数学公式来实现。

```
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$
```


$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
${$tep1}{\style{visibility:hidden}{(x+1)(x+1)}}
$$






























[1]:https://www.google.com







