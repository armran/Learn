# Markdown基本语法

> 约翰·格鲁伯设计文档中概述的Markdown元素。
> <https://markdown.p2hp.com/basic-syntax/>

## 总览

几乎所有Markdown应用程序都支持John Gruber原始设计文档中概述的基本语法。Markdown处理器之间存在细微的差异和差异-尽可能在线内注明。

**注意：使用Markdown并不意味着您也不能使用HTML。您可以将HTML标签添加到任何Markdown文件中。如果您更喜欢某些HTML标记而不是Markdown语法，这将很有帮助。例如，有些人发现将HTML标签用于图像更容易。**

## 标题

要创建标题，请#在单词或短语的前面添加数字符号（）。您使用的数字符号的数量应与标题级别相对应。例如，要创建标题级别三（`<h3>`），请使用三个数字符号（例如`### My Header`）。

Markdown|HTML|渲染输出
--|--|--
`# Heading level 1`| `<h1>Heading level 1</h1>`|<h1>标题等级1</h1>
`## Heading level 2` | `<h2>Heading level 2</h2>` |<h2>标题等级2</h2>
`### Heading level 3` |`<h3>Heading level 3</h3>` |<h3>标题级别3</h3>
`#### Heading level 4`| `<h4>Heading level 4</h4>` |<h4>标题级别4</h4>
`##### Heading level 5`| `<h5>Heading level 5</h5>` |<h5>标题级别5</h5>
`###### Heading level 6`| `<h6>Heading level 6</h6>` |<h6>标题等级6</h6>

### 替代语法

或者，在文本下方的行上，添加任意数量的==标题级别1的--字符 或 标题级别2的字符。

Markdown |HTML |渲染输出
--|--|--
Heading level 1 <br> =============== |`<h1>Heading level 1</h1>` |<h1>标题等级1</h1>
Heading level 2 <br>--------------- |`<h2>Heading level 2</h2>`|<h2>标题等级2</h2>

## 段落

要创建段落，请使用空白行分隔一行或多行文本。您不应缩进带有空格或制表符的段落。

Markdown| HTML |渲染输出
--|--|--
I really like using Markdown.<br><br>I think I'll use it to format all of my documents from now on. |`<p>I really like using Markdown.</p>`<br><br>`<p>I think I'll use it to format all of my documents from now on.</p>`|我真的很喜欢使用Markdown。<br><br>我想从现在开始，我将使用它来格式化所有文档。

## 换行

要创建换行符（`<br>`），请以两个或多个空格结束一行，然后键入return。

Markdown| HTML |渲染输出
--|--|--
This is the first line.  <br>And this is the second line. |`<p>This is the first line.<br>`<br>`And this is the second line.</p>`|这是第一行。<br>这是第二行。

## 着重

您可以通过使文本变为粗体或斜体来增加着重。

### 粗体

要加粗文本，请在单词或短语的前后添加两个星号或下划线。要加粗一个单词的中部以强调，请在字母周围添加两个星号，且各空格之间不加空格。

Markdown |HTML |渲染输出
--|--|--
`I just love **bold text**.`|`I just love <strong>bold text</strong>.`| 我只喜欢**粗体字**。
`I just love __bold text__.` |`I just love <strong>bold text</strong>.` |我只喜欢**粗体字**。
`Love**is**bold` |`Love<strong>is</strong>bold`| 爱**是**大胆的

### 斜体

要斜体显示文本，请在单词或短语的前后添加一个星号或下划线。要斜体突出单词的中间部分，请在字母周围添加一个星号，中间不要带空格。

Markdown |HTML |渲染输出
--|--|--
`Italicized text is the *cat's meow*.` |`Italicized text is the <em>cat's meow</em>.`| 斜体文字是*猫的叫声*。
`Italicized text is the _cat's meow_.`| `Italicized text is the <em>cat's meow</em>.`| 斜体文字是*猫的叫声*。
`A*cat*meow`| `A<em>cat</em>meow` |一个*猫*喵

### 粗体和斜体

要同时突出显示带有粗体和斜体的文本，请在单词或短语的前后添加三个星号或下划线。

Markdown |HTML| 渲染输出
--|--|--
`This text is ***really important***.`| `This text is <strong><em>really important</em></strong>.`| 这段文字***真的很重要***。
`This text is ___really important___.` |`This text is <strong><em>really important</em></strong>.` |这段文字***真的很重要***。
`This text is __*really important*__.`|`This text is <strong><em>really important</em></strong>.` |这段文字***真的很重要***。
`This text is **_really important_**.`| `This text is <strong><em>really important</em></strong>.` |这段文字***真的很重要***。

### 删除线

~~删除线~~
`~~删除~~`

## 块引用

要创建blockquote，请>在段落前面添加一个。

`> Dorothy followed her through many of the beautiful rooms in her castle.`

呈现的输出如下所示：

> 桃乐丝（Dorothy）跟着她走过了她城堡中许多美丽的房间。

### 具有多个段落的块引用

块引用可以包含多个段落。>在段落之间的空白行上添加一个。

```text
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood. 
```

呈现的输出如下所示：

> 桃乐丝（Dorothy）跟着她走过了她城堡中许多美丽的房间。
> 
> 女巫请她清洗锅碗瓢盆，扫地，并用木柴取火。

### 嵌套块引用

块引用可以嵌套。`>>`在要嵌套的段落前面添加一个。

```text
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```

呈现的输出如下所示：
>桃乐丝（Dorothy）跟着她走过了她城堡中许多美丽的房间。
>
>>女巫请她清洗锅碗瓢盆，扫地，并用木柴取火。

### 具有其他元素的块引用

块引用可以包含其他Markdown格式的元素。并非所有元素都可以使用-您需要进行实验以查看哪些元素有效。

```text
> #### The quarterly results look great
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> *Everything* is going according to **plan**.
```

呈现的输出如下所示：

> #### 季度业绩看起来不错  
>  
> - 收入超出了预期。
> - 利润比以往任何时候都高。
>  
> *一切*都按**计划**进行。

## 清单

您可以将项目组织成有序和无序列表。

### 有序列表

要创建有序列表，请在订单项中添加数字和句点。数字不必按数字顺序排列，但列表应以数字开头。

<table>
  <thead>
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染输出</th>
    </tr>
  </thead>
  <tbody>
  <tr>
    <td>
      <code>
        1. First item<br>
        2. Second item<br>
        3. Third item<br>
        4. Fourth item
      </code>
    </td>
    <td>
      <code>
        &lt;ol&gt;<br>
          &lt;li&gt;First item&lt;/li&gt;<br>
          &lt;li&gt;Second item&lt;/li&gt;<br>
          &lt;li&gt;Third item&lt;/li&gt;<br>
          &lt;li&gt;Fourth item&lt;/li&gt;<br>
        &lt;/ol&gt;
      </code>
    </td>
    <td>
      <ol>
        <li>第一项</li>
        <li>第二项</li>
        <li>第三项</li>
        <li>第四项</li>
      </ol>
    </td>
    </tr>
    <tr>
      <td>
        <code>
          1. First item<br>
          2. Second item<br>
          3. Third item<br>
          4. Fourth item
        </code>
      </td>
      <td>
        <code>
          &lt;ol&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
        </code>
      </td>
      <td>
        <ol>
          <li>第一项</li>
          <li>第二项</li>
          <li>第三项</li>
          <li>第四项</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td>
        <code>
          5. First item<br>
          6. Second item<br>
          7. Third item<br>
          8. Fourth item
        </code>
      </td>
      <td>
        <code>
          &lt;ol&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
        </code>
      </td>
      <td>
        <ol>
          <li>第一项</li>
          <li>第二项</li>
          <li>第三项</li>
          <li>第四项</li>
        </ol>
      </td>
    </tr>
    <tr>
      <td>
        <code>
          9. First item<br>
          10. Second item<br>
          11. Third item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;1. Indented item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;2. Indented item<br>
          12. Fourth item
        </code>
      </td>
      <td>
        <code>
          &lt;ol&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item<br>
              &lt;ol&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
              &lt;/ol&gt;<br>
            &lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ol&gt;
        </code>
      </td>
      <td>
        <ol>
          <li>第一项</li>
          <li>第二项</li>
          <li>第三项
            <ol>
              <li>缩进项</li>
              <li>缩进项</li>
            </ol>
          </li>
          <li>第四项</li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>


### 无序列表

要创建无序列表，请在订单项前添加破折号（-），星号（*）或加号（+）。缩进一个或多个项目以创建嵌套列表。

Markdown HTML 渲染输出
<table class="table table-bordered">
  <thead class="thead-light">
    <tr>
      <th>Markdown</th>
      <th>HTML</th>
      <th>渲染输出</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>
        <code>
          - First item<br>
          - Second item<br>
          - Third item<br>
          - Fourth item
        </code>
      </td>
      <td>
        <code>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>第一项</li>
          <li>第二项</li>
          <li>第三项</li>
          <li>第四项</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <code>
          * First item<br>
          * Second item<br>
          * Third item<br>
          * Fourth item
        </code>
      </td>
      <td>
        <code>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>第一项</li>
          <li>第二项</li>
          <li>第三项</li>
          <li>第四项</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <code>
          + First item<br>
          * Second item<br>
          - Third item<br>
          + Fourth item
        </code>
      </td>
      <td>
        <code>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item&lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>第一项</li>
          <li>第二项</li>
          <li>第三项</li>
          <li>第四项</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <code>
          - First item<br>
          - Second item<br>
          - Third item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>
          &nbsp;&nbsp;&nbsp;&nbsp;- Indented item<br>
          - Fourth item
        </code>
      </td>
      <td>
        <code>
          &lt;ul&gt;<br>
            &lt;li&gt;First item&lt;/li&gt;<br>
            &lt;li&gt;Second item&lt;/li&gt;<br>
            &lt;li&gt;Third item<br>
              &lt;ul&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
                &lt;li&gt;Indented item&lt;/li&gt;<br>
              &lt;/ul&gt;<br>
            &lt;/li&gt;<br>
            &lt;li&gt;Fourth item&lt;/li&gt;<br>
          &lt;/ul&gt;
        </code>
      </td>
      <td>
        <ul>
          <li>第一项</li>
          <li>第二项</li>
          <li>第三项
            <ul>
              <li>缩进项</li>
              <li>缩进项</li>
            </ul>
          </li>
          <li>第四项</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 在列表中添加元素

要在保留列表连续性的同时在列表中添加另一个元素，请将该元素缩进四个空格或一个制表符，如以下示例所示。

#### 段落

```text
- This is the first list item.
- Here's the second list item.

    I need to add another paragraph below the second list item.

- And here's the third list item.
```

呈现的输出如下所示：

- 这是第一个列表项。
- 这是第二个列表项。

    我需要在第二个列表项下面添加另一段。

- 这是第三个列表项。

#### 块引用

```text
- This is the first list item.
- Here's the second list item.

    > A blockquote would look great below the second list item.

- And here's the third list item.
```

呈现的输出如下所示：

- 这是第一个列表项。
- 这是第二个列表项。

    > 在第二个列表项的下方，blockquote看起来不错。

- 这是第三个列表项。

#### 代码块

代码块通常缩进四个空格或一个制表符。当它们在列表中时，将它们缩进八个空格或两个选项卡。

```text
1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.
```

呈现的输出如下所示：

1. 打开文件。
2. 在第21行找到以下代码块：

        <html>
        <head>
            <title>Test</title>
        </head>
3. 更新标题以匹配您的网站名称。

#### 图片

```text
1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.
```

呈现的输出如下所示：

1. 打开包含Linux吉祥物的文件。
2. 惊叹于它的美丽。

    ![Tux，Linux吉祥物](image.png)

3. 关闭文件。

## 代码

要将单词或短语表示为代码，请将其括在勾号（`）中。

Markdown |HTML| 渲染输出
--|--|--
At the command prompt, type \`nano`. |At the command prompt, type `<code>nano</code>.`| 在命令提示符下，键入`nano`。

### 转义刻度线

如果要表示为代码的单词或短语包含一个或多个刻度线，可以通过将单词或短语括在双刻度线（``）中来对其进行转义。

Markdown |HTML |渲染输出
--|--|--
\`\`Use \`code\` in your Markdown file.\`\`| `<code>`Use \`code\` in your Markdown file.`</code>`| Use `code` in your Markdown file.

### 代码块

要创建代码块，请在代码块的每一行缩进至少四个空格或一个制表符。

```text
    <html>
      <head>
      </head>
    </html>
```

呈现的输出如下所示：

        <html>
            <head>
            </head>
        </html>

 注意：要创建没有缩进线的代码块，请使用围栅代码块。

## 水平线

要创建水平线***，请单独在一行上使用三个或更多的星号（），破折号（---）或下划线（___）。

```text
***

---

_________________
```

所有这三个的渲染输出看起来都相同：

***

---
___ 

## 链接

要创建链接，请将链接文本括在方括号（例如[Duck Duck Go]）中，然后立即在URL后面加上括号（例如(https://duckduckgo.com)）中的URL 。

`My favorite search engine is [Duck Duck Go](https://duckduckgo.com).`

呈现的输出如下所示：

我最喜欢的搜索引擎是[Duck Duck Go](https://duckduckgo.com)。

### 添加标题

您可以选择为链接添加标题。当用户将鼠标悬停在链接上时，这将显示为工具提示。要添加标题，请将其括在URL后面的括号中。

`My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").`

呈现的输出如下所示：

我最喜欢的搜索引擎是[Duck Duck Go](https://duckduckgo.com "The best search engine for privacy")。

### 网址和电子邮件地址

要将URL或电子邮件地址快速转换为链接，请将其括在尖括号中。

`<https://markdown.p2hp.com>`
`<fake@example.com>`

呈现的输出如下所示：

<https://markdown.p2hp.com>
<fake@example.com>

### 格式化链接

为了强调链接，请在方括号和括号之前和之后添加星号。

`I love supporting the **[EFF](https://eff.org)**.`
`This is the *[Markdown Guide](https://markdown.p2hp.com)*.`
呈现的输出如下所示：

我喜欢支持 **[EFF](https://eff.org)**。
这是 *[《Markdown指南》](https://markdown.p2hp.com)*。

### 参考样式链接

引用样式链接是一种特殊的链接，它使URL在Markdown中更易于显示和阅读。引用样式的链接分为两部分：与文本保持内联的部分以及在文件中其他位置存储的部分，以使文本易于阅读。

#### 格式化链接的第一部分

参考样式链接的第一部分使用两组括号进行格式化。第一组方括号包围应显示为链接的文本。第二组括号显示了一个标签，该标签用于指向您存储在文档其他位置的链接。

尽管不是必需的，但您可以在第一组和第二组支架之间包含一个空格。第二组括号中的标签不区分大小写，可以包含字母，数字，空格或标点符号。

这意味着以下示例格式对于链接的第一部分大致相同：

- `[hobbit-hole][1]`
- `[hobbit-hole] [1]`
  
呈现的输出如下所示：
[hobbit-hole][1]
[hobbit-hole] [1]

#### 格式化链接的第二部分

引用样式链接的第二部分使用以下属性设置格式：

标签放在方括号中，后紧跟冒号和至少一个空格（例如`[label]: ` ）。

- 链接的URL，您可以选择将其括在尖括号中。
- 链接的可选标题，您可以将其括在双引号，单引号或括号中。
- 这意味着以下示例格式对于链接的第二部分几乎都是等效的：

```text
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)
```

呈现的输出如下所示：
[1]
[这是百度]

[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
[这是百度]: https://www.baidu.com

您可以将链接的第二部分放在Markdown文档中的任何位置。有些人将它们放在出现的段落之后，而其他人则将它们放在文档的末尾（例如尾注或脚注）。

#### 将零件放在一起的示例

假设您添加一个URL作为到段落的标准URL链接，并且在Markdown中看起来像这样：

```text
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole](https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"), and that means comfort.
```

尽管它可能指向有趣的附加信息，但显示的URL确实不会给现有的原始文本增加太多，除了使其难以阅读之外。要解决此问题，您可以改为设置网址格式：

```text
In a hole in the ground there lived a hobbit. Not a nasty, dirty, wet hole, filled with the ends
of worms and an oozy smell, nor yet a dry, bare, sandy hole with nothing in it to sit down on or to
eat: it was a [hobbit-hole][1], and that means comfort.
```

在上述两种情况下，呈现的输出将相同：

在地上的一个洞里住着一个霍比特人。这不是一个肮脏，肮脏，潮湿的洞，里面充满蠕虫的末端和难闻的气味，也没有一个干燥，裸露，沙质的洞，里面没有东西可以坐下或进食：那是一个[霍比特洞][这是百度]，意味着舒适。

链接HTML为：

`<a href="https://en.wikipedia.org/wiki/Hobbit#Lifestyle" title="Hobbit lifestyles">hobbit-hole</a>`

## 图片

要添加图像，请添加感叹号（!），然后在括号中添加替代文本，并在括号中添加图像资源的路径或URL。您可以选择在括号中的URL之后添加标题。

```text
![Philadelphia's Magic Gardens. This place was so cool!](/assets/images/philly-magic-gardens.jpg "Philadelphia's Magic Gardens")
```

呈现的输出如下所示：

![费城的魔法花园。 这个地方真酷！](image-1.png)

### 链接图像

要向图像添加链接，请将图像的Markdown括在方括号中，然后在括号中添加链接。

```text
[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](www.baidu.com)
```

呈现的输出如下所示：

[![沙漠中的一块老石头](image-2.png "Shiprock, New Mexico by Beau Rogers")](https://www.baidu.com)

## 转义字符

要显示原义字符，否则将用于设置Markdown文档中的文本格式\，请在字符前面添加反斜杠（）。

`\* Without the backslash, this would be a bullet in an unordered list.`

呈现的输出如下所示：

`*`如果没有反斜杠，这将是无序列表中的项目符号。

### 你可以转义的字符

您可以使用反斜杠转义以下字符。

字符 |名称
--|--
\ |反斜杠
` |刻度线（另请参见转义刻度线中的代码）
\- |星号
_ |下划线
{} |大括号
[] |中括号
() |括号
\# |井号
\+ |加号
\- |减号（连字符）
. |点
! |感叹号
\| |管道（另请参见表中的转义管道）
