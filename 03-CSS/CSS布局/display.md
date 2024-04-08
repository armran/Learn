# display

CSS display 属性设置元素是否被视为块或者内联元素以及用于子元素的布局，例如流式布局、网格布局或弹性布局。

形式上，display 属性设置元素的内部和外部的显示类型。外部类型设置元素参与流式布局；内部类型设置子元素的布局。一些 display 值在它们自己的单独规范中完整定义；例如，在 CSS 弹性盒模型的规范中，定义了声明 display: flex 时会发生的细节。

```css
/* precomposed values */
display: block;         // 块级元素盒， 默认，元素之前或之后会换行。
display: inline;        // 内联元素盒， 内部不会换行。如果同行有空间，下一个元素将会在同一行上。
display: inline-block;
display: flex;
display: inline-flex;
display: grid;
display: inline-grid;
display: flow-root;

/* box generation */
display: none;
display: contents;

/* 双值语法 */
display: block flow;
display: inline flow;
display: inline flow-root;
display: block flex;
display: inline flex;
display: block grid;
display: inline grid;
display: block flow-root;

/* other values */
display: table;
display: table-row; /* all table elements have an equivalent CSS display value */
display: list-item;

/* Global values */
display: inherit;
display: initial;
display: revert;
display: revert-layer;
display: unset;

```

## 分组的值

关键值可以被分组为六个种类。

### 外部表现

`<display-outside>` 这些关键字规定元素的外部显示类型，实际上就是其在流式布局中的角色：

#### block

该元素生成一个块级元素盒，在正常的流中，该元素之前和之后产生换行。

#### inline

该元素生成一个或多个内联元素盒，它们之前或者之后并不会产生换行。在正常的流中，如果有空间，下一个元素将会在同一行上。

> 备注： 浏览器支持双值语法，当仅发现外部值时，例如当指定 display: block 或 display: inline，其将内部值设置为 flow。这种行为是预期的；例如，如果你指定一个元素是块元素，你将期望该元素的子元素将同块和内联元素一样参与正常的流布局。

### 内部表现

`<display-inside>` 这些关键字规定了元素的内部显示类型，其定义了该内容布局时的格式上下文的类型（假设它是一个非替换元素）：

#### flow 实验性

该元素使用流式布局（块和内联布局）来排布它的内容。

如果它的外部显示类型是 inline 或 run-in，并且它参与一个块或者内联格式上下文，那么它将生成一个内联盒子。否则它将生成一个块容器盒。

根据其他属性的值（例如 position、float 或 overflow）以及它自身是否参与到块或者内联格式化上下文，它要么为它的内容建立新的区块格式化上下文（BFC），要么将其内容集成到其父元素的格式化上下文中。

#### flow-root

该元素生成一个块级元素盒，其会建立一个新的区块格式化上下文，定义格式化上下文的根元素。

#### table

该元素的行为类似于 HTML 中的 `<table>` 元素。它定义了一个块级别的盒子。

#### flex

该元素的行为类似块级元素并且根据弹性盒模型布局它的内容。

#### grid

该元素的行为类似块级元素并且根据网格模型布局它的内容。

#### ruby 实验性

该元素的行为类似内联元素并且根据 ruby 格式化模型布局它的内容。它的行为像关联的 HTML 的 `<ruby>` 元素。

> 备注： 浏览器支持双值语法，当仅发现外部值时，例如当指定 display: flex 或 display: grid，其将外部值设置为 block。这种行为是预期的；例如，如果你指定一个元素是 display: grid，你将期望在网格容器中创建的盒子是块级别的盒子。

### 列表元素

`<display-listitem>` 该元素为内容生成一个块级盒子和一个单独的列表元素内联盒子。

list-item 的单独值将导致元素的行为类似于一个列表元素。其可以与 list-style-type 和 list-style-position 一起使用。

list-item 也可以与任意的 `<display-outside>` 关键字和 `<display-inside>` 中的 flow 或 flow-root 关键字组合。

备注： 浏览器支持双值语法，如果没有指定内部值，默认为 flow。如果没有指定外部值，主体盒子将具有 block 的外部显示类型。

## 内部

`<display-internal>`
一些布局模型，例如 table 和 ruby 有一个复杂的内置结构，它们的子孙后代可以扮演几个不同的角色。本节定义的这些“内部”display 值，仅在特定的布局模式下有用。

table-row-group
该元素的行为类似于 HTML 的 `<tbody>` 元素。

table-header-group
该元素的行为类似于 HTML 的 `<thead>` 元素。

table-footer-group
该元素的行为类似于 HTML 的 `<tfoot>` 元素。

table-row
该元素的行为类似于 HTML 的 `<tr>` 元素。

table-cell
该元素的行为类似于 HTML 的 `<td>` (en-US) 元素。

table-column-group
该元素的行为类似于 HTML 的 `<colgroup>` 元素。

table-column
该元素的行为类似于 HTML `<col>` 元素。

table-caption
该元素的行为类似于 HTML 的 `<caption>` 元素。

ruby-base 实验性
该元素的行为类似于 HTML 的 `<rb>` 元素。

ruby-text 实验性
该元素的行为类似于 HTML 的 `<rt>` 元素。

ruby-base-container 实验性
该元素是作为匿名盒子生成的。

ruby-text-container 实验性
该元素的行为类似于 HTML 的 `<rtc>` 元素。

## 盒

`<display-box>`这些关键词定义一个元素到底是否产生 display 盒。

#### contents

这些元素自身不会产生特定的盒子。它们被伪盒子（pseudo-box）和子盒子取代。请注意，CSS Display Level 3 规范中定义了 contents 值如何影响“异常元素”——这些元素不是纯粹由 CSS 盒模型概念呈现的（例如替换元素）。更多的细节请参见附录 B：display 的影响：异常元素的内容。

由于浏览器的一个错误，该元素目前不会被添加到无障碍树中——屏幕阅读器将不会看到里面的内容。更多细节，参见下面的无障碍问题。

#### none

使元素不再显示，其对布局不会有影响（文档渲染得好像这个元素并不存在）。所有的后代元素也不会再显示。为了使元素占据一个它通常占据的空间，但实际上没有渲染任何东西，应该使用 visibility 属性。

## 预组合

`<display-legacy>`
CSS 2 为 display 属性使用单关键字的预组合的语法，对相同布局模式的块级和内联级变体需要单独的关键字。

#### inline-block

该元素生成块级元素盒，如果它是一个单独的内联盒，它将和周围的内容一起流动（行为类似于替换元素）。

它等同于 inline flow-root。

#### inline-table

inline-table 值在 HTML 中没有直接的映射。它行为类似于 HTML 的 `<table>` 元素，但实际是一个内联盒，而不是一个块级盒子。table 盒内部是一个块级上下文。

它等同于 inline table。

#### inline-flex

元素的行为类似于内联元素并且它的内容根据弹性盒模型布局。

它等同于 inline flex。

#### inline-grid

元素的行为类似于内联元素并且它的内容根据网格盒模型布局。

它等同于 inline grid。
