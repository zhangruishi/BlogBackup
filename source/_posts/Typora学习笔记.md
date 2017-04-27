---
title: Typora学习笔记
date: 2017-04-26 23:02:56
tags: Typora
reward: true

---

`说明：`

- 以下方法并不是唯一的，我只是选择了我验证成功或者比较喜欢的一种
- 以下基本所有操作符都是在英文输入法下进行的，中文输入法有时下达不到所要的效果
- 如果您在浏览本博文的时候发现有侵权行为，请及时与[博主](https://amiao.site/)联系，如果转载也请注明出处
- 后续如果发现其他的比较实用的操作也会陆续更新
- 由于是新手，所述可能欠妥，欢迎留言指正

<!--more-->

[TOC]

### 基础

#### 无序列表

- 这个小点（即无序列表）是”-+空格“实现的（千万不要忘记空格）

#### 有序列表

这是有序列表（一定要注意，.后面有一个空格，如果想跳出列表需要回车键和返回键配合使用）

1. 这是有序列表（一定要注意.后面有一个空格）
   1. 这是嵌套列表，如果使用请注意顺序，先做有序列表，再使用嵌套，可能还有其他方法我不知道
2. 有序列表
3. 有序列表

#### 标签形式

`用英文输入下的Esc键下面的那个键（一对）即可达到此效果，一般用来写单句代码`

#### 字体大小的选择

几个#代表几号字体的标题，只能用来做标题

#### 链接表示

[关于链接：英文输入下的中括号，里面填上你想写的话，然后在后面输入小括号里面贴上链接地址就可以了 ](https://amiao.site/)，它的快捷键是`Ctrl+K`

#### 引用

> 这是一段引用，用>空格（不要忘了空格）来开始

#### 下划线

<u>下划线的效果是一对u把需要斜线的部分填在中间</u>（快捷键是`Ctrl+U`）

#### 加粗或者强调

**粗线是一对双星号\****

#### 斜体

*斜体是一对单星号\**

#### 删除线

~~这是删除线，一对双波浪线（注意要在英文下输入）~~

#### 居中

<center>要居中的文字，用一对`<center></center>`表示，但是只能等到输出文本的时候才会看到效果</center>

#### 脚注

脚注的正确用法：先创建一个，比如我要创建一个名字为“Typora”的脚注，那么我可以这样做，Typora[^ 1]（1可以换成任意字符，是用中括号，里面是个^然后空格（千万不要忘了空格））然后把鼠标放在2的上面他就会出现一个黑色的框框，点击，然后到最下面去编写，这样就完成了

#### 下标

网上教程说用一对波浪线既可以表示，但是我没有试出来。后来又仔细的看了一下，可以了，需要右键insert打开Math Block，效果不是太好，比如水分子的表达式：
$$
H~2~O
$$

#### 上标

跟下标差不多，也需要右键，用的操作符是^,比如
$$
x^2
$$

#### 表情符号

:happy:（两个冒号中间加上描述语，比如这个就是happy）

#### 分割线

用三个”-“连在一起（即”---“）即可

#### 目录制作

在需要插入目录的地方写上[TOC]（大写小写都可以），回车，然后整篇文章的目录就自动形成了，比如最开始的那个目录就是通过这种方法生成的。

![me](../uploads/me.jpg)

### 高级

#### 表格制作

我是通过右键-->insert的形式打开的，当然也可以通过快捷键Ctrl+T来打开。填入行数与列数就可以了

|  姓名  |  性别  |   毕业学校   |
| :--: | :--: | :------: |
|  张三  |  男   | 西安电子科技大学 |
|  李四  |  男   |  华中科技大学  |
|  赵红  |  女   |  中华女子学院  |

#### 图片插入

可以使用拖动的形式，但是得提前修改一下设置，还是在File-->preference-->image insert-->勾选Allow copy……选项，还有就是导出来的pdf格式有图片的，但是html格式是没有的。

![me](/uploads/me.jpg)

#### 数学表达式

关于数学表达式要先启用这个功能，必须先在File-->preference-->Math Blocks中启用,然后用两个美元符号包裹起来，然后结合latex公式法则进行描写，比如下面的这个 \$lim_{x\to\infty}\exp(-x)=0\$

$lim_{x\to\infty}\exp(-x)=0$

LaTeX公式（右键insert选择）
$$
a^2+b^2=c^2
$$
关于更详细的LaTeX公式，可以参考[这篇博客](http://blog.163.com/goldman2000@126/blog/static/167296895201221242646561/)

#### 代码编写

输入三个波浪线然后回车或者直右键插入就可以输入代码块。如果想让显示行数，需要开启，在File-->preference-->Code Fences。Typora支持大部分的编程语言，且支持高亮显示。开始编写之前需要现在右下角选择语言。

```javascript
//var fs;
var fs = require('fs')
	, stdin = process.stdin
	, stdout = process.stdout;

/*fs.readdir(__dirname, function (err, files) {
	console.log(files);
});*/
```



```flow
st=>start: Start
e=>end
op=>operation: My Operation
cond=>condition: Yes or No?

st->op->cond
cond(yes)->e
cond(no)->op
```

以及时序图：

```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

> **提示：**想要了解更多，请查看 **流程图**[语法](http://flowchart.js.org/)以及 **时序图**[语法](http://bramp.github.io/js-sequence-diagrams/)

#### 复选框（或任务列表）

-[空格]空格 文字-----代表没有选中的复选框

-[x]空格 文字------代表选中的复选框

- [x] 数学


- [ ] 英语

### 附加

#### 常用快捷键

加粗：`Ctrl+B`

斜体：`Ctrl+I`

字体：`Ctrl+数字`

下划线：`Ctrl+U`

返回开头：`Ctrl+Home`

返回结尾：`Ctrl+End`

生成表格：`Ctrl+T`	

创建链接：`Ctrl+K`	

#### 参考文献

[Typora快捷键](http://blog.csdn.net/it_guang/article/details/53456026)

[Typora使用教程](http://jingyan.baidu.com/article/09ea3ede151af8c0afde397e.html?qq-pf-to=pcqq.c2c&allowHTTP=1)

[如何优雅地使用Typora](https://sanwen8.cn/p/7e2nNIb.html)

[马克飞象的官方说明文档](https://maxiang.io/)

[^1]: 这是一个注释
[^ 2]: Typora是一款免费的所见即所得的基于markdown语法的编辑工具