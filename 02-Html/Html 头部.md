# Html 头部

```html
<!doctype html>
<html lang="zh-CN">
  <head>
    <meta charset="utf-8" />
    <title>我的测试页面</title>
  </head>
  <body>
    <p>这是我的页面</p>
  </body>
</html>
```

## 添加作者和描述

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

## 在你的站点增加自定义图标

将其保存在与网站的索引页面相同的目录中，以 .ico 格式保存（大多数浏览器支持更通用的格式，如 .gif 或 .png）
将以下行添加到 HTML 的 · 块中以引用它：

```html
<link rel="icon" href="favicon.ico" type="image/x-icon" />
```

## 在 HTML 中应用 CSS 和 JavaScript

```html
<link rel="stylesheet" href="my-css-file.css" />

<script src="my-js-file.js" defer></script>
```
