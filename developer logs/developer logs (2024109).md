# developer logs (2024/10/9)

## 任务

### markdown语法学习 并用typora实操

# markdown标题语法

| Markdown语法                     | HTML                       | 预览效果        |
| -------------------------------- | -------------------------- | --------------- |
| `Heading level 1===============` | `<h1>Heading level 1</h1>` | Heading level 1 |
| `Heading level 2---------------` | `<h2>Heading level 2</h2>` | Heading level 2 |

一级标题可用“#”实现，并且可在一级标题下一行使用任意个“=”来实现

=========

二级使用“--”

————————

一到六级标题都可用'#'实现，‘#’个数依次增加

“#号”和标题之间保持一个空格

| Markdown语法             | HTML                       | 预览效果        |
| ------------------------ | -------------------------- | --------------- |
| `# Heading level 1`      | `<h1>Heading level 1</h1>` | Heading level 1 |
| `## Heading level 2`     | `<h2>Heading level 2</h2>` | Heading level 2 |
| `### Heading level 3`    | `<h3>Heading level 3</h3>` | Heading level 3 |
| `#### Heading level 4`   | `<h4>Heading level 4</h4>` | Heading level 4 |
| `##### Heading level 5`  | `<h5>Heading level 5</h5>` | Heading level 5 |
| `###### Heading level 6` | `<h6>Heading level 6</h6>` | Heading level 6 |



# markdown段落语法

要创建段落，要使用空白行将一行或多行间隔开



就像这样，并且不要用space或tab键缩进段落

# markdown换行语法

几乎每个 Markdown 应用程序都支持两个或多个空格进行换行，称为 `结尾空格（trailing whitespace)` 的方式，但这是有争议的，因为很难在编辑器中直接看到空格，并且很多人在每个句子后面都会有意或无意地添加两个空格。由于这个原因，你可能要使用除结尾空格以外的其它方式来换行。幸运的是，几乎每个 Markdown 应用程序都支持另一种换行方式：HTML 的 `<br>` 标签。

为了兼容性，请在行尾添加“结尾空格”或 HTML 的 `<br>` 标签来实现换行。

还有两种其他方式我并不推荐使用。CommonMark 和其它几种轻量级标记语言支持在行尾添加反斜杠 (`\`) 的方式实现换行，但是并非所有 Markdown 应用程序都支持此种方式，因此从兼容性的角度来看，不推荐使用。并且至少有两种轻量级标记语言支持无须在行尾添加任何内容，只须键入回车键（`return`）即可实现换行。



# makdown强调语法

## 粗体（Bold）

要加粗文本，请在单词或短语的前后各添加两个星号（asterisks）或下划线（underscores）。如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号（asterisks）。

| Markdown语法                 | HTML                                      | 预览效果                   |
| ---------------------------- | ----------------------------------------- | -------------------------- |
| `I just love **bold text**.` | `I just love <strong>bold text</strong>.` | I just love **bold text**. |
| `I just love __bold text__.` | `I just love <strong>bold text</strong>.` | I just love **bold text**. |
| `Love**is**bold`             | `Love<strong>is</strong>bold`             | Love**is**bold             |

**粗体**

__粗体__

这是我要**强调**的

## 斜体（Italic）

要用斜体显示文本，请在单词或短语前后添加一个星号（asterisk）或下划线（underscore）。要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格。

| Markdown语法                           | HTML                                          | 预览效果                             |
| -------------------------------------- | --------------------------------------------- | ------------------------------------ |
| `Italicized text is the *cat's meow*.` | `Italicized text is the <em>cat's meow</em>.` | Italicized text is the *cat’s meow*. |
| `Italicized text is the _cat's meow_.` | `Italicized text is the <em>cat's meow</em>.` | Italicized text is the *cat’s meow*. |
| `A*cat*meow`                           | `A<em>cat</em>meow`                           | A*cat*meow                           |

### 斜体（Italic）用法的最佳实践

要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个星号或下划线。要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。

| ✅ Do this    | ❌ Don't do this |
| ------------ | --------------- |
| `A*cat*meow` | `A_cat_meow`    |

## 粗体（Bold）和斜体（Italic）

要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个星号或下划线。要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。

| Markdown语法                              | HTML                                                         | 预览效果                                 |
| ----------------------------------------- | ------------------------------------------------------------ | ---------------------------------------- |
| `This text is ***really important***.`    | `This text is <strong><em>really important</em></strong>.`   | This text is ***really important\***.    |
| `This text is ___really important___.`    | `This text is <strong><em>really important</em></strong>.`   | This text is ***really important\***.    |
| `This text is __*really important*__.`    | `This text is <strong><em>really important</em></strong>.`   | This text is ***really important\***.    |
| `This text is **_really important_**.`    | `This text is <strong><em>really important</em></strong>.`   | This text is ***really important\***.    |
| `This is really***very***important text.` | `This is really<strong><em>very</em></strong>important text.` | This is really***very\***important text. |

***bold and italic***

### 粗体（bold）和斜体（italic）用法的最佳实践粗体（Bold）和斜体（Italic）用法的最佳实践

Markdown 应用程序在处理单词或短语中间添加的下划线上并不一致。为了实现兼容性，请使用星号将单词或短语的中间部分加粗并以斜体显示，以示重要。

| ✅ Do this                                 | ❌ Don't do this                           |
| ----------------------------------------- | ----------------------------------------- |
| `This is really***very***important text.` | `This is really___very___important text.` |

  

# markdown引用语法

> 正在引用这么写--mrzhan
>
> > 还可以嵌套引用
> >
> > > 可以无限吗
> > >
> > > > 要我一直嵌套吗
> > > >
> > > > > 话说咋么会上一层嵌套  
> > > >
> > > > 原来两次回车就回到上一次引用了
> > >
> > > 神奇吧
> >
> > 我自己发现的
>
> 厉害吧



# markdown列表语法

有序列表

> 要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。

1.  first
2.  second
3.  third
4. fourth
5. fifth

无序列表

> 要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。

- first
  - 嵌套列表
  - - 嵌套
    - - 嵌套
      - 
- second
- third
- fourth
- fifth

> 要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：

```text
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.
```

- 列表
  - 列表
    - 列表



> 要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：
>
> 段落

```text
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.
```

> 引用

```text
*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.
```

> 代码块通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。
>
> ```text
> 1.  Open the file.
> 2.  Find the following code block on line 21:
> 
>         <html>
>           <head>
>             <title>Test</title>
>           </head>
> 
> 3.  Update the title to match the name of your website
> ```

# mrakdown代码语法

> 要将单词或短语表示为代码，请将其包裹在反引号 (```) 中。

比如我要打`printf()`

> ## 转义反引号

> 如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号(````)中。

``I want to use `code` can use "two '`' " ``

> ## 代码块
>
> 要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。

​	include <stdio.h>

​	main(){

​		printf("hello world");

​		return(0);

​			}

# markdown分隔线语法

> 要创建分隔线，请在单独一行上使用三个或多个星号 (`***`)、破折号 (`---`) 或下划线 (`___`) ，并且不能包含其他内容。

我想要使用分割线



____

上面有了一根

***

又有了

---

为了兼容性，请在分隔线的前后均添加空白行。



***



使用

## markdown链接语法

> 链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

> 超链接Markdown语法代码：`[超链接显示名](超链接地址 "超链接title")`

> 对应的HTML代码：`<a href="超链接地址" title="超链接title">超链接显示名</a>`

> ***注意要使用英文符号***

 

[好康的](https://markdown.com.cn/ “markdown语法教程”)

这是一个链接 [Markdown语法](https://markdown.com.cn/)

> 链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。

[good](https://markdown.com.cn/ “bad”)



> ## 网址和email地址

> 使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

<https://markdown.com.cn/>

<mr.zhan20042023@outlook.com>

<https://markdown.com.cn>

> 强调链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。

*<https://markdown.com.cn>*

**<https://markdown.com.cn>**

***<https://markdown.com.cn>***

See the section on [`code`](https://markdown.com.cn).

## 引用类型链接

> 引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。参考样式链接分为两部分：与文本保持内联的部分以及存储在文件中其他位置的部分，以使文本易于阅读.

#### 链接的第一部分格式

引用类型的链接的第一部分使用两组括号进行格式设置。第一组方括号包围应显示为链接的文本。第二组括号显示了一个标签，该标签用于指向您存储在文档其他位置的链接。

尽管不是必需的，可以在第一组和第二组括号之间包含一个空格。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。

以下示例格式对于链接的第一部分效果相同：

- `[hobbit-hole][1]`
- `[hobbit-hole] [1]`

[markdown learn][6]

#### 链接的第二部分格式

引用类型链接的第二部分使用以下属性设置格式：

1. 放在括号中的标签，其后紧跟一个冒号和至少一个空格（例如`[label]:`）。
2. 链接的URL，可以选择将其括在尖括号中。
3. 链接的可选标题，可以将其括在双引号，单引号或括号中。

以下示例格式对于链接的第二部分效果相同：

- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'`
- `[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)`
- `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"`
- `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'`
- `[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)`

可以将链接的第二部分放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，有些人则将它们放在文档的末尾（例如尾注或脚注）。

[6 ]: https://markdown.com.cn/basic-syntax/links.html#code



# markdown图片语法

> 要添加图像，请使用感叹号 (`!`), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。
>
> 插入图片Markdown语法代码：`![图片alt](图片链接 "图片title")`。
>
> 对应的HTML代码：`<img src="图片链接" alt="图片alt" title="图片title">`



![this is picture](D:\图片\原神\1722607916931.jpg "原神，启动！")

### 链接图片

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

```text
[![沙漠中的岩石图片](/assets/img/shiprock.jpg "Shiprock")](https://markdown.com.cn)
```

渲染效果如下：

[![原神四周年](D:\图片\原神\1727451636491.jpg)](https://ys.mihoyo.com/)



# markdown转义字符语法

>要显示原本用于格式化 Markdown 文档的字符，请在字符前面添加反斜杠字符 \ 。

```text
\* Without the backslash, this would be a bullet in an unordered list.
```

渲染效果如下：

\* Without the backslash, this would be a bullet in an unordered list.

### 可做转义的字符

以下列出的字符都可以通过使用反斜杠字符从而达到转义目的。

| Character | Name                                                         |
| --------- | ------------------------------------------------------------ |
| \         | backslash                                                    |
| `         | backtick (see also [escaping backticks in code](https://markdown.com.cn/basic-syntax/escaping-characters.html#escaping-backticks)) |
| *         | asterisk                                                     |
| _         | underscore                                                   |
| { }       | curly braces                                                 |
| [ ]       | brackets                                                     |
| ( )       | parentheses                                                  |
| #         | pound sign                                                   |
| +         | plus sign                                                    |
| -         | minus sign (hyphen)                                          |
| .         | dot                                                          |
| !         | exclamation mark                                             |
| \|        | pipe (see also [escaping pipe in tables](https://markdown.com.cn/extended-syntax/escaping-pipe-characters-in-tables.html)) |



## 特殊字符自动转义

在 HTML 文件中，有两个字符需要特殊处理： `<` 和 `&` 。 `<` 符号用于起始标签，`&` 符号则用于标记 HTML 实体，如果你只是想要使用这些符号，你必须要使用实体的形式，像是 `<` 和 `&`。

`&` 符号其实很容易让写作网页文件的人感到困扰，如果你要打「AT&T」 ，你必须要写成「`AT&T`」 ，还得转换网址内的 `&` 符号，如果你要链接到：

```
http://images.google.com/images?num=30&q=larry+bird
```

你必须要把网址转成：

```
http://images.google.com/images?num=30&amp;q=larry+bird
```

才能放到链接标签的 `href` 属性里。不用说也知道这很容易忘记，这也可能是 HTML 标准检查所检查到的错误中，数量最多的。

Markdown 允许你直接使用这些符号，它帮你自动转义字符。如果你使用 `&` 符号的作为 HTML 实体的一部分，那么它不会被转换，而在其它情况下，它则会被转换成 `&`。所以你如果要在文件中插入一个著作权的符号，你可以这样写：

```
&copy;
```

Markdown 将不会对这段文字做修改，但是如果你这样写：

```
AT&T
```

Markdown 就会将它转为：

```
AT&amp;T
```

类似的状况也会发生在 `<` 符号上，因为 Markdown 支持 [行内 HTML](https://markdown.com.cn/basic-syntax/#内联-html) ，如果你使用 `<` 符号作为 HTML 标签的分隔符，那 Markdown 也不会对它做任何转换，但是如果你是写：

```
4 < 5
```

Markdown 将会把它转换为：

```
4 &lt; 5
```

需要特别注意的是，在 Markdown 的块级元素和内联元素中， `<` 和 `&` 两个符号都会被自动转换成 HTML 实体，这项特性让你可以很容易地用 Markdown 写 HTML。（在 HTML 语法中，你要手动把所有的 `<` 和 `&` 都转换为 HTML 实体。）



# markdown内嵌html标签

> 对于 Markdown 涵盖范围之外的标签，都可以直接在文件里面用 HTML 本身。如需使用 HTML，不需要额外标注这是 HTML 或是 Markdown，只需 HTML 标签添加到 Markdown 文本中即可。
>
> ## 行级內联标签
>
> HTML 的行级內联标签如 `<span>`、`<cite>`、`<del>` 不受限制，可以在 Markdown 的段落、列表或是标题里任意使用。依照个人习惯，甚至可以不用 Markdown 格式，而采用 HTML 标签来格式化。例如：如果比较喜欢 HTML 的 `<a>` 或 `<img>` 标签，可以直接使用这些标签，而不用 Markdown 提供的链接或是图片语法。当你需要更改元素的属性时（例如为文本指定颜色或更改图像的宽度），使用 HTML 标签更方便些。
>
> HTML 行级內联标签和区块标签不同，在內联标签的范围内， Markdown 的语法是可以解析的。
>
> ```text
> This **word** is bold. This <em>word</em> is italic.
> ```
>
> 渲染效果如下:
>
> This **word** is bold. This *word* is italic.
>
> ## 区块标签
>
> 区块元素──比如 `<div>`、`<table>`、`<pre>`、`<p>` 等标签，必须在前后加上空行，以便于内容区分。而且这些元素的开始与结尾标签，不可以用 tab 或是空白来缩进。Markdown 会自动识别这区块元素，避免在区块标签前后加上没有必要的 `<p>` 标签。
>
> 例如，在 Markdown 文件里加上一段 HTML 表格：
>
> ```
> This is a regular paragraph.
> 
> <table>
>     <tr>
>         <td>Foo</td>
>     </tr>
> </table>
> 
> This is another regular paragraph.
> ```
>
> 请注意，Markdown 语法在 HTML 区块标签中将不会被进行处理。例如，你无法在 HTML 区块内使用 Markdown 形式的`*强调*`。
>
> ### HTML 用法最佳实践
>
> 出于安全原因，并非所有 Markdown 应用程序都支持在 Markdown 文档中添加 HTML。如有疑问，请查看相应 Markdown 应用程序的手册。某些应用程序只支持 HTML 标签的子集。
>
> 对于 HTML 的块级元素 `<div>`、`<table>`、`<pre>` 和 `<p>`，请在其前后使用空行（blank lines）与其它内容进行分隔。尽量不要使用制表符（tabs）或空格（spaces）对 HTML 标签做缩进，否则将影响格式。
>
> 在 HTML 块级标签内不能使用 Markdown 语法。例如 `<p>italic and **bold**</p>` 将不起作用。



		This is a regular paragraph.

<table>
    <tr>
        <td>**Foo**</td>
    </tr>
</table>


This is another regular paragraph.



# markdown扩展语法

## markdown表格

> 要添加表，请使用三个或多个连字符（`---`）创建每列的标题，并使用管道（`|`）分隔每列。您可以选择在表的任一端添加管道。

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

要添加表，请使用三个或多个连字符（`---`）创建每列的标题，并使用管道（`|`）分隔每列。您可以选择在表的任一端添加管道。

```text
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

呈现的输出如下所示：

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

单元格宽度可以变化，如下所示。呈现的输出将看起来相同。

```text
| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |
```

**Tip:** 使用连字符和管道创建表可能很麻烦。为了加快该过程，请尝试使用[Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)。使用图形界面构建表，然后将生成的Markdown格式的文本复制到文件中。

## 对齐

您可以通过在标题行中的连字符的左侧，右侧或两侧添加冒号（`:`），将列中的文本对齐到左侧，右侧或中心。

```text
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

呈现的输出如下所示：

| Syntax    | Description |   Test Text |
| :-------- | :---------: | ----------: |
| Header    |    Title    | Here’s this |
| Paragraph |    Text     |    And more |

| 标题   | description |
| ------ | ----------- |
| header | title       |

## 格式化表格中的文字

您可以在表格中设置文本格式。例如，您可以添加链接，代码（仅反引号（```）中的单词或短语，而不是代码块）和强调。

您不能添加标题，块引用，列表，水平规则，图像或HTML标签。

## 在表中转义管道字符

您可以使用表格的HTML字符代码（`|`）在表中显示竖线（`|`）字符。



# markdown围栏式代码块

Markdown基本语法允许您通过将行缩进四个空格或一个制表符来创建[代码块](https://markdown.com.cn/basic-syntax/code-blocks.html)。如果发现不方便，请尝试使用受保护的代码块。根据Markdown处理器或编辑器的不同，您将在代码块之前和之后的行上使用三个反引号（(`````）或三个波浪号（~~~）。

~~~text
```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
~~~

呈现的输出如下所示：

```text
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

**Tip:**要在代码块中显示反引号？请参阅了解如何[转义](https://markdown.com.cn/basic-syntax/escaping-backticks.html)它们。

```c#
#include <stdio.h>
main(){
	printf("hello world");
	return(0);
}
```

## 语法高亮

许多Markdown处理器都支持受围栏代码块的语法突出显示。使用此功能，您可以为编写代码的任何语言添加颜色突出显示。要添加语法突出显示，请在受防护的代码块之前的反引号旁边指定一种语言。

~~~text
```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
~~~

呈现的输出如下所示：

{ "firstName": "John", "lastName": "Smith", "age": 25 }

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

