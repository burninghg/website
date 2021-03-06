The basic grammar of markdown
<!--more-->
---
title: Markdown.md
date: 2020-06-25 21:34:24
tags: Technique
categories: Trick
---
<!-- TOC -->autoauto- [1. 基础操作](#1-基础操作)auto    - [1.1标题](#11标题)auto    - [1.2 引用](#12-引用)auto    - [1.3 斜体](#13-斜体)auto    - [1.4 加粗](#14-加粗)auto    - [1.5 下划线](#15-下划线)auto    - [1.6 删除线](#16-删除线)auto    - [1.7 分割线](#17-分割线)auto    - [1.8 注脚](#18-注脚)auto    - [1.9 上下标,高亮](#19-上下标高亮)auto    - [1.10 目录](#110-目录)auto- [2. 代码](#2-代码)auto    - [2.1 单行代码](#21-单行代码)auto    - [2.2 多行代码](#22-多行代码)auto    - [2.3 注释](#23-注释)auto- [3. 列表](#3-列表)auto    - [3.1 无序列表](#31-无序列表)auto    - [3.2 多行无序列表](#32-多行无序列表)auto    - [3.3 有序列表](#33-有序列表)auto    - [3.4 多行有序列表](#34-多行有序列表)auto    - [3.5 任务列表](#35-任务列表)auto    - [3.6 表格](#36-表格)auto- [4. 链接](#4-链接)auto    - [4.1 图片](#41-图片)auto    - [4.2 超链接](#42-超链接)auto    - [4.3 框架](#43-框架)auto    - [4.4](#44)auto- [5. 符号的输入](#5-符号的输入)auto    - [5.1 普通符号](#51-普通符号)auto    - [5.2 特殊符号](#52-特殊符号)auto    - [5.3 更多符号](#53-更多符号)auto    - [5.4 表情符号](#54-表情符号)auto- [6. 快捷键](#6-快捷键)auto- [7. HTML特殊字符编码对照表](#7-html特殊字符编码对照表)auto    - [7.1 KBD](#71-kbd)auto    - [字体](#字体)auto    - [注释](#注释)auto    - [指定图片的宽度](#指定图片的宽度)auto    - [## **[对HTML语言的支持](http://support.typora.io/HTML/)**](#-对html语言的支持httpsupporttyporaiohtml)auto- [8. Typora设置](#8-typora设置)auto    - [8.1 偏好设置](#81-偏好设置)auto    - [8.2 模式](#82-模式)auto    - [8.3 主题设置](#83-主题设置)autoauto<!-- /TOC -->
Typora[^1]
[^1]:A markdown editor
[toc]

# 1. 基础操作

## 1.1标题

```markdown
# 		一级标题

## 		二级标题

### 	三级标题

#### 	四级标题

##### 	五级标题

###### 	六级标题
```



## 1.2 引用

```markdown
>  引用内容1
>  引用内容2
>> 引用内容3
```



## 1.3 斜体

```markdown
*斜体*
_斜体_
```



## 1.4 加粗

```markdown
**加粗**
__加粗__
***加粗斜体***
```



## 1.5 下划线

```markdown
<u>下划线</u>
```



## 1.6 删除线 

```markdown
~~删除线~~
```



## 1.7 分割线

```markdown
***
---
___
```



## 1.8 注脚

```markdown
Typora[^1]
[^1]:A markdown editor
```



## 1.9 上下标,高亮

```markdown
5<sup>2</sup>=25
H<sub>2</sub>OCO<sub>2</sub>

#以下需要在文件->偏好设置->markdown->markdown拓展语法勾选
6^2^=36
H~2~O
==高亮==
```



## 1.10 目录

```markdown
[soc] 自动生成目录
```



# 2. 代码

## 2.1 单行代码

```markdown
`String str1 = "hello`
```



## 2.2 多行代码

```html
​```
~~~
~~~python
​```c
```



## 2.3 注释

```html
#html注释
<!-- 注释 -->
#hack方法
[^_^]: # (我是注释，超级萌。)
*[·-·]:注释内容
*[^_^]:注释内容
*[@_@]:注释内容
```

# 3. 列表

## 3.1 无序列表

```markdown
* 无序列表1
+ 无序列表2
- 无序列表3
```



## 3.2 多行无序列表

```markdown
*         无序列表1
TAB *     无序列表2
TAB TAB * 无序列表3
```



## 3.3 有序列表

```markdown
1. 有序列表1
2. 有序列表2
3. 有序列表3
```



## 3.4 多行有序列表

```markdown
1. 多行有序列表1
2. 多行有序列表2
    1. 多行有序列表2-1
    2. 多行有序列表2-2
3. 多行有序列表3
    1. 多行有序列表3-1
    2. 多行有序列表3-2
```



## 3.5 任务列表

```markdown
- [ ] 任务1
- [x] 任务2(打勾的选项)
```



## 3.6 表格

```markdown
Ctrl + t
|姓名|性别|年龄|手机号|
|：---|：--：|：--：|---：|
|张三|男|21|18975346876|
|李四|女|23|17789548964|
|王五|男|25|15876513546|
```
:-左对齐-: 右对齐 :-: 居中


# 4. 链接

## 4.1 图片

```markdown
![typora](图片的绝对地址)	#本地图片
![typora](图片的网络地址)	#网络图片
```



## 4.2 超链接

```markdown
样式1.
	[百度](https://www.baidu.com/)
样式2.
	[CSDN][CSDN网址]
	[CSDN网址]:https://www.csdn.net/
样式3.
	<https://www.csdn.net/>
```



## 4.3 框架

```markdown
<iframe src="链接"...参数...></iframe>
```
## 4.4 站内跳转
Markdown会自动给每一个h1~h6标题生成一个锚，其id就是标题内容。目录树中的每一项都是一个跳转链接，点击后就会跳转到其对应的锚点（即标题所在位置）。你可以点击本文档开始处的目录树尝试一下。
使用Markdown的语法来增加跳转链接：“[名称](#id)”。[1](#9参考文献)


# 5. 符号的输入

## 5.1 普通符号

```markdown
\\
\`
\*
\_
\{\}
\[\]
\(\)
\#
\+
\-
\.
\!
```



## 5.2 特殊符号

```markdown
©   版权
®    注册商标
™  商标
    空格
&    和号
"   引号
'   撇号
<     小于号
>     大于号
≠     不等号
≤     小于等于
≥     大于等于
¢   分
£  磅
€   欧元
¥    元
§   节
×  乘号
÷ 除号
± 正负号
```



## 5.3 更多符号

[HTML特殊字符编码对照表](https://www.jb51.net/onlineread/htmlchar.htm)



## 5.4 表情符号

```markdown
#支持添加emoji表情，输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情。
:smile:
```



# 6. 快捷键

```markdown
Ctrl+1  	一阶标题    
Ctrl+2  	二阶标题    
Ctrl+3  	三阶标题    
Ctrl+4  	四阶标题    
Ctrl+5  	五阶标题    
Ctrl+6  	六阶标题    
Ctrl+B  	字体加粗(Blod)
Ctrl+I  	字体倾斜(Italic)
Ctrl+U  	下划线(Underline)
Ctrl+Z		撤销
Ctrl+T		创建表格(Table)				    
Ctrl+L  	选中某句话   
Ctrl+K  	创建超链接
Ctrl+D  	选中某个单词  
Ctrl+F  	搜索(Find)
Ctrl+H		搜索并替换
Ctrl+\		清楚样式
Ctrl+E  	选中相同格式的文字  
Ctrl+Home	 	返回Typora顶部	
Ctrl+End     	返回Typora底部
Alt+Shift+5 	删除线 
Ctrl+Shift+I    插入图片(Image)
Ctrl+Shift+M    公式块 
Ctrl+Shift+K	代码块
Ctrl+Shift+Q    引用(Quote)
```



# 7. HTML特殊字符编码对照表
## 7.1 KBD

```
<kbd></kbd>
```
<kbd>Ctrl</kbd>


## 字体

`<font face="黑体" color=red size=12>你好hello world</font>`


## 注释

```
<!--  -->
```

## 指定图片的宽度

```
<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">
```

## ## **[对HTML语言的支持](http://support.typora.io/HTML/)**

 <span style='color:red'>This is red</span> 
 ```

 <span style='color:red'>This is red</span> 

 ```

 <kbd>Ctrl</kbd>+<kbd>F9</《》 kbd> 
```
<kbd>Ctrl</kbd>+<kbd>F9</《》 kbd> 

```
 <span style="font-size:2rem; background:yellow;">**Bigger**</span> 
```

 <span style="font-size:2rem; background:yellow;">**Bigger**</span> 
```
 \## <a name="anchor"></a> Header 2 <span style="display:none">I am hidden after export</span> 


# 8. Typora设置

## 8.1 偏好设置
​		文件=>偏好设置
## 8.2 模式

​		视图=>...

​		**「专注模式」**使你正在编辑的那一行保留颜色，而其他行的字体呈灰色。

​		**「打字机模式」**使得你所编辑的那一行永远处于屏幕正中。

​		**「源代码模式」**以源代码显示

## 8.3 主题设置

​		菜单栏=>主题

2. [流程图的实现]( https://www.runoob.com/markdown/md-advance.html )
test[1]

# 9.参考文献

[1] www.google.com
[2] [Markdown目录树、锚（anchor）和页内跳转](https://blog.csdn.net/tearsky253/article/details/78968221)