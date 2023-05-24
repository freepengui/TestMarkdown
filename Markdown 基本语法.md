



MarKdown 基本语法

[TOC]

# Markdown 基本语法

Markdown 是一种轻量级标记语言，排版语法简洁，让人们更多关注内容本身而非排版。使用易读易写的纯文本格式编写文档，可与HTML混编，可导出HTML、PDF以及本身的 .md 格式的文件。简洁、高效、易读、易写，Markdown被大量使用，如Github、Wikipedia、简书等。

常用的标记符号不超过十个，用于日常写作绰绰有余，不到半小时就能完全掌握。这十个不到的标记符号，却能让人**优雅地沉浸式记录**，专注内容而不是纠结排版。



### Markdown 标题语法

 要创建标题，请在单词或短语前面添加井号（#）。 、# 的数量代表了标题的级别。



|             语法             |           HTML            |        预览效果        |
| :--------------------------: | :-----------------------: | :--------------------: |
|      # Heading level 1       | <h1>Heading level 1</h1>  |   # Heading level 1    |
| \#\#\#\#\#\# Heading level 6 | <h6> Heading level 6</h6> | ###### heading level 6 |

___

##### 可选语法

还可以在文本下方添加任意数量的 == 号来标识一级标题，或者--好来标识二级标题。

|   Markdown语法   |           HTML           |        效果        |
| :--------------: | :----------------------: | :----------------: |
| Heading level  1<br>-------------------------- | <h1>Heading level 1</h1> | # Heading level 1  |
|                  |                          |                    |
| Heading level 2<br>==============  | <h2>Heading level 2</h2> | ## Heading level 2 |

----------------------



### Markdown 段落语法

要创建段落，请使用空白行将一行或者多行文本进行分隔。

I really like using Markdown.



I think I'll use it to format all of my documents from now on.

Note: 不要使用空格 或制表符 tab 缩进段落。



### Markdown 换行语法

几乎每个Markdown应用都支持 HTML的标签 \<br> or \</br> 换行。



### Markdown 强调语法

#### 粗体（bold）

请在单词或短语前后各添加两个星号\** 或者下划线 \__。

I just love **bold text**.

I just love __bold text__.

just**love**bold

#### 斜体（Italic）

前后添加一个星号（asterisk）或下划线（underscore）。

Italized text is the *cat's meow*

Italized text is the _cat's meow_

A*cat*mow

要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个星号或下划线。

this text is ***really important***.

this text is __really important__.

this text is **_really important_**.

this test is __*really important*__.

thistestis***really***important.

note: 尽量用*，下划线_处理不统一。



### Markdown 引用语法

要创建块引用，请在段落前添加一个 \> 符号。

> Dorothy follow her through many of the beautiful rooms in here castle.

>sudo apt-get install automake build-essential clang cmake git libboost-dev libboost-thread-dev libgmp libntl-dev libsodium-dev libssl-dev libtool python3

#### 多个段落的块引用

块引用可以包含多个段落。为段落之间的空白行添加一个 \> 符号。

>Dorothy followed her through many of the beautiful rooms in her castle.
>
>The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with with wood.

#### 嵌套块引用 

在嵌套的段落前添加 \>> 符号。

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> >The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with with wood.

#### 带有其他元素的引用

快引用可以包含其他Markdown格式的元素。并非所有元素都可以使用，需要试试看。

> #### The quarterly results look great!
>
> - Revenue was off the chart.
>
> - Profits were higher than ever.
>
> *Everything* is going according to **plan**.



### Markdown 列表语法

可以将多个条目组织成有序或无序列表。

##### 有序列表

要创建有序列表，请在每个列表项前添加数字并紧跟一个英文局点。数字不必按数学顺序排列，但是列表应当以数字1起始。

1. First item
2. Second item

---

1. first item
2. second item
3. third item 

---

1. first item
8. second item
3. third item
5. forth item

---

1. First item
2. Second item
	1.Indented item
	2.Indented item
3. third item

---

don't use 1) 



##### 无序列表

要创建无序列表，请在每个列表项前面添加**破折号 (-)**、星号 (*) 或加号 (+) **不要混着用**。缩进一个或多个列表项可创建嵌套列表。

- First item

- Second item

  - Indented item

  - Indented item

- Third item



##### 在列表中嵌入其他元素

要在**保留列表连续性**的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：

###### 段落

* This is  the first list item.
* Here's the second list item.

​		I need to add  another paragraph below the second list item.

* And here's the third list item

###### 引用块

* This is  the first list item.

* Here's the second list item.

  > A blockquote would look great below the second list item.

* And here's third list item.

###### 代码块

[代码块](https://markdown.com.cn/basic-syntax/lists.html#code-blocks)通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。

1. Open the file.

2. Find the following code block on line 21:

   <html>

   	<head>
   	    <title>Test</title>
   	</head>

3. Updated the title  to mathc the name of you r website.

###### 图片

1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

   ​	![Tux, the linux mascot](./assets/tux.png)
3. Close the file.

###### 列表

1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item




### Markdown 代码语法

要将单词或短语表示为代码，请将其包裹在反引号 (\`) 中。

例：At the command prompt, type `nano`.

###### 转义反引号

如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(\``)中。

例：``Use `code` in your Markdown file``

###### 代码块

要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。

​	<html>

		<head>
		    <title>Test</title>
		</head>

###### 围栏式代码块 （fenced code blocks）

根据Markdown处理器或编辑器的不同，您将在代码块之前和之后的行上使用三个反引号（\```）或三个波浪号（\~~~）。

```c++
#include <iostream>
#include <string>
using namespace std;

class Person{
    public:
    	string name;
    	int age;
    	string addr;
    Person(string s, int age, string add){
        this->name = s;
        this->age = age;
        this->addr = add;
        cout << "this is construction func"<< endl;
    }
}
int main(){
    Person p = new Person("C++", 22, "GCC")
    cout << "hello world!" << endl;
}
```

例：

```latex
{
	"firstName": "Jhon",
	"lastName": "Smith",
	"age":	25
}
```



### Markdown 公式语法

###### $\LaTeX$ 公式

行内公式:两个 \$ \LaTeX \$ 之间


$m(y)^{(i)} = \sum_{i=1}^{l} \Delta^{(i)} \cdot x^{(i)}_h$


行间公式：

Typaro中输入\$\$然后回车


$$
m(y)^{(i)} = \sum \Delta^{(i)} \cdot x^{(i)}_h
$$

$$
y^{(i)} = \sum_{j=1}^{t} c_j \cdot x^{(i)}_j +\begin{cases}
				c &  x= 1\\
				0 &  x \neq 1
			\end{cases}
$$

$$
\boldsymbol{r} \leftarrow \mathcal{F}_{Rand}(\mathbb{F}^{l+1})
$$


### Markdown 分割线语法

\*** or \--- or \__ 为了兼容性，请在分隔线的前后均添加空白行。


### Markdown 链接语法

###### 普通用法

链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

对应的HTML代码：`<a href="超链接地址" title="超链接title">超链接显示名</a>`

这是一个链接 [MarkDown语法](https://markdown.com.cn "最好的markdown教程").

###### 网址和Email地址

使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

<https://markdown.com.cn>

<290469254@qq.com>

###### 带格式化的链接

1 强调链接，在链接语法前后增加星号。2 要将链接表示为代码，请在方括号中添加反引号。

I love supporting the **[EFF](https://eff.org)**

This is the *[Markdown Guide](https://markdownguide.org)*.

See the section on [`code`](#code).

###### 引用类型链接

引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。*参考样式链接* 分为两部分：与文本保持**内联**的部分以及存储在文件中其他位置的部分，以使文本易于阅读。

**链接的第一部分格式**

引用类型的链接的第一部分使用两组括号进行格式设置。第一组方括号包围应显示为链接的文本。第二组括号显示了一个标签，该标签用于指向您存储在文档其他位置的链接。

尽管不是必需的，可以在第一组和第二组括号之间包含一个空格。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。

以下示例格式对于链接的第一部分效果相同：

- `[hobbit-hole][1]`
- `[hobbit-hole] [2]`
- `[this is a quote link] [3]`



**引用链接的第二部分格式**

引用类型链接的第二部分使用以下属性设置格式：

1. 放在括号中的标签，其后紧跟一个冒号和至少一个空格（例如`[label]:`）。
2. 链接的URL，可以选择将其括在尖括号中。URL中间的空格方式不一样。为了兼容性，请尽量使用%20代替空格。
3. 链接的可选标题，可以将其括在双引号，单引号或括号中。

以下示例格式对于链接的第二部分效果相同：

- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)`
- `[2]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"`
- `[2]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'`
- `[2]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)`

可以将链接的第二部分放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，有些人则将它们放在文档的末尾（例如尾注或脚注）。



### Markdown 图片语法

 要添加图像，请使用感叹号 (!), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。

插入图片Markdown语法代码： ![图片alt](图片链接 "图片title")。

对应的HTML代码：<img src="图片链接" alt="图片alt" title="图片title">

![这是图片](markdown00.jpg "markdown pic")



### Markdown 扩展语法

#### Markdown 表格语法

要添加表格，请使用三个或多个连字符（---）创建每列的标题，并使用管道（|）分隔每列。可选择在表中的任一端添加管道。

:joy:

| Syntax | Description |
| :----: | :---------: |
|        |             |



- `[3]  <https://github.com/freepengui/TestMarkdown/blob/main/Markdown 基本语法.md>`









