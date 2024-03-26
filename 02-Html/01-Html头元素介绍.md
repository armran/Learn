# Html 头部

```html
<!doctype html>
<html lang="zh-CN">
  <head>
    <meta charset="utf-8" />
    <title>我的测试页面</title>
    <!-- 增加自定义图标 -->
    <link rel="icon" href="favicon.ico" type="image/x-icon" />
    <!-- 引入CSS -->
    <link rel="stylesheet" href="my-css-file.css" />
    <!-- 引入JavaScript -->
    <!-- defer 告诉浏览器在解析完成 HTML 后再加载 JavaScript。 -->
    <script src="my-js-file.js" defer></script>
  </head>
  <body>
    <p>这是我的页面</p>
  </body>
</html>
```

## 声明文档类型

`<!DOCTYPE html>`: 声明文档类型。早期的 HTML（大约 1991-1992 年）文档类型声明类似于链接，规定了 HTML 页面必须遵从的良好规则，能自动检测错误和其他有用的东西。文档类型使用类似于这样：

```HTML
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```

## `<html> 元素`

`<html></html>`: `<html>` 元素。这个元素包裹了页面中所有的内容，有时被称为根元素。

## `<head>` 元素

`<head></head>`: `<head>` 元素。这个元素是一个容器，它包含了所有你想包含在 HTML 页面中但不在 HTML 页面中显示的内容。这些内容包括你想在搜索结果中出现的关键字和页面描述、CSS 样式、字符集声明等等。以后的章节中会学到更多相关的内容。

## `<meta>` 元素

`<meta charset="utf-8">`:`<meta>` 元素。这个元素代表了不能由其他 HTML 元相关元素表示的元数据，比如 `<base>`、`<link>`、`<script>`、`<style>` 或 `<title>`。charset 属性将你的文档的字符集设置为 UTF-8，其中包括绝大多数人类书面语言的大多数字符。有了这个设置，页面现在可以处理它可能包含的任何文本内容。没有理由不对它进行设置，它可以帮助避免以后的一些问题。

### 添加作者和描述

许多 `<meta>` 元素包含了 name 和 content 属性：

- name 指定了 meta 元素的类型；说明该元素包含了什么类型的信息。
- content 指定了实际的元数据内容。
这两个 meta 元素对于定义你的页面的作者和提供页面的简要描述是很有用的。让我们看一个例子：

```html
<meta name="author" content="Chris Mills" />
<meta
  name="作者"
  content="描述内容，这是个什么页面" />
```

## `<title>` 元素

`<title></title>`:`<title>` 元素。这设置了页面的标题，也就是出现在该页面加载的浏览器标签中的内容。当页面被加入书签时，页面标题也被用来描述该页面。

## `<body>` 元素

`<body></body>`: `<body>` 元素。包含了你访问页面时所有显示在页面上的内容，包含文本、图片、视频、游戏、可播放音频轨道等等。

文档类型是一个历史遗留问题，需要包含它才能使其他东西正常工作。现在，只需要知道`<!DOCTYPE html>` 是最短的有效文档声明！
