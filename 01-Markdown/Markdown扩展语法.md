# Markdown扩展语法

> <https://markdown.p2hp.com/extended-syntax/>

## 总览

John Gruber的原始设计文档中概述的基本语法每天增加了许多所需的元素，但对于某些人来说还不够。这就是扩展语法的用武之地。

一些个人和组织开始通过添加表，代码块，语法突出显示，URL自动链接和脚注等其他元素来扩展基本语法。可以通过使用基于基本Markdown语法的轻量级标记语言，或者通过向兼容的Markdown处理器添加扩展来启用这些元素。

## 可用性

并非所有Markdown应用程序都支持扩展语法元素。您需要检查您的应用程序所使用的轻量级标记语言是否支持您要使用的扩展语法元素。如果没有，仍然可以在Markdown处理器中启用扩展。

### 轻量标记语言

有几种轻量级标记语言是Markdown的超集。它们包括Gruber的基本语法，并通过添加其他元素（例如表，代码块，语法突出显示，URL自动链接和脚注）在此基础上构建。许多最受欢迎的Markdown应用程序使用以下轻量级标记语言之一：

- [通用商标](http://commonmark.org)
- [GitHub风格的Markdown（GFM）](https://github.github.com/gfm/)
- [Markdown Extra](https://michelf.ca/projects/php-markdown/extra/)
- [MultiMarkdown](http://fletcherpenney.net/multimarkdown/)
- [R Markdown](https://rmarkdown.rstudio.com/)

### Markdown处理器

有几十个[Markdown的处理器](https://github.com/markdown/markdown.github.com/wiki/Implementations)使用。它们中的许多允许您添加启用扩展语法元素的扩展。查看处理器的文档以获取更多信息。

## 表格

要添加表，请使用三个或多个连字符（---）创建每列的标题，并使用管道（|）分隔每列。您可以选择在表的任一端添加管道。

```text
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```

呈现的输出如下所示：

句法|描述
--|--
标头|标题
段|文本

像元宽度可以变化，如下所示。呈现的输出将看起来相同。

```text
| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |
```

 提示：使用连字符和管道创建表可能很麻烦。为了加快这一过程，请尝试使用Markdown Tables Generator。使用图形界面构建表，然后将生成的Markdown格式的文本复制到文件中。

### 合并单元格

在插件设置中打开 `enableExtendedTableSyntax`

|a|b|
|--|--|
|>|1|
|2||

|a|b|
|--|--|
|1|2|
|^|2|

### 对齐

您可以通过:在标题行内的连字符的左侧，右侧或两侧添加一个冒号（），以使列中的文本左，右或居中对齐。

```text
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```

呈现的输出如下所示：

句法|描述|测试文字
:--|:--:|--:
标头|标题|这是这个
左|中|右

### 格式化表格中的文字

您可以格式化表格中的文本。例如，您可以添加链接，代码（`仅在刻度线中显示单词或短语，而不能在代码块中添加）和强调。

您不能添加标题，块引用，列表，水平规则，图像或HTML标签。

### 在表中转义管道字符

您可以|使用表格的HTML字符代码（`&#124;`）在表中显示竖线（ `|` ）字符。

## 围栏代码块

Markdown基本语法允许您通过将行缩进四个空格或一个制表符来创建代码块。如果发现不方便，请尝试使用受保护的代码块。根据Markdown处理器或编辑器的不同，您将在代码块之前和之后的行上使用三个刻度线（```）或三个波浪号（~~~）。最好的部分？您不必缩进任何行！

\```
    {
    "firstName": "John",
    "lastName": "Smith",
    "age": 25
    }
\```

呈现的输出如下所示：

```text
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### 语法高亮

许多Markdown处理器都支持围栏代码块的语法突出显示。此功能使您可以为代码编写时使用的任何语言添加颜色突出显示。要添加语法突出显示，请在受防护的代码块之前的对号旁指定一种语言。

\```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
\```

呈现的输出如下所示：

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

## 脚注

脚注使您可以添加注释和参考，而不会使文档正文混乱。创建脚注时，带有脚注引用的链接将出现带有链接的上标编号。读者可以单击链接跳至页面底部的脚注内容。

要创建脚注参考，请在方括号（`[^1]`）内添加插入符号和标识符。标识符可以是数字或文字，但他们不能包含空格或制表符。标识符仅将脚注参考与脚注本身相关联-在输出中，脚注按顺序编号。

在括号内使用另一个插入符号和数字添加脚注，并用冒号和文本（`[^1]: My footnote.`）括起来。您不必在文档末尾添加脚注。你可以把他们的任何地方，除了像列表一样，块报价，和表格等元素里面。

```text
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
```

呈现的输出如下所示：

这是一个简单的脚注,[^1] 是一个较长的脚注。[^bignote]

[^1]: 这是第一个脚注。
[^bignote]: 这是一个包含多个段落和代码的代码。

缩进段落以将其包括在脚注中。
`{ my code }`
添加任意多的段落。

## 标题编号

> **本解释器用不了标号id，因规则不允许标题重复，所以id默认为标题名**

许多Markdown处理器支持标题的自定义ID-一些Markdown处理器会自动添加它们。添加自定义的ID，您可以直接链接到标题，并用CSS修改。要添加自定义标题ID，请在与标题相同的行上用大括号括起该自定义ID。

```text
### My Great Heading {#custom-id}
```

HTML看起来像这样：

```text
<h3 id="custom-id">My Great Heading</h3>
```

### 链接到标题ID

通过创建带有数字符号（）和自定义标题ID 的标准链接，可以链接到文件中具有自定义ID #的标题。

Markdown|HTML|渲染输出
--|--|--
`[Heading IDs](#heading-ids)`|`<a href="#heading-ids">Heading IDs</a>`|[Heading IDs](#链接到标题id)

通过将自定义标题ID添加到网页的完整URL（例如，`[Heading IDs](http://markdown.p2hp.com/extended-syntax#heading-ids)`），其他网站可以链接到标题。

## 定义清单

一些Markdown处理器允许您创建自定义列表和术语及其相应的定义。要创建定义列表，请在第一行上键入术语。下一行，键入一个冒号后跟一个空格和定义。

```text
First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.
```

HTML看起来像这样：

```html
<dl>
  <dt>First Term</dt>
  <dd>This is the definition of the first term.</dd>
  <dt>Second Term</dt>
  <dd>This is one definition of the second term. </dd>
  <dd>This is another definition of the second term.</dd>
</dl>
```

呈现的输出如下所示：

第一学期
: 这是第一个术语的定义。

第二期
: 这是第二项的定义。
: 这是第二项的另一个定义。

## 删除线

您可以通过在单词中心放置一条水平线来“删除”单词。结果看起来像这样。此功能使您可以指示某些单词是一个错误，并不表示要包含在文档中。若要删除单词，请~~在单词前后使用两个波浪号（）。

`~~The world is flat.~~ We now know that the world is round.`
呈现的输出如下所示：

~~世界是平坦的。~~ 我们现在知道世界是圆的。

## 任务清单

任务列表使您可以创建带有复选框的项目列表。在支持任务列表的Markdown应用程序中，复选框将显示在内容旁边。要创建任务列表，请在任务列表项之前添加破折号（`-`）和方括号，并[ ]在其前面加上一个空格（）。要选择一个复选框，请x在方括号（`[x]`）之间添加in 。

``` text
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```

呈现的输出如下所示：

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

## 自动网址链接

许多Markdown处理器会自动将URL转换为链接。这意味着如果您输入`http://www.example.com`，即使您没有使用方括号，您的Markdown处理器也会自动将其转换为链接。

`http://www.example.com`
呈现的输出如下所示：

`http://www.example.com`

## 禁用自动URL链接

如果您不希望自动链接URL，则可以通过将URL表示为带有刻度线的代码来删除该链接。

```text
`http://www.example.com`
```

呈现的输出如下所示：

`http://www.example.com`
