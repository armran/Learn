# iframe

```html
<iframe
  src="https://developer.mozilla.org/zh-CN/docs/Glossary"
  width="100%"
  height="500"
  frameborder="0"
  allowfullscreen
  sandbox>
  <p>
    <a href="https://developer.mozilla.org/zh-CN/docs/Glossary">
      Fallback link for browsers that don't support iframes
    </a>
  </p>
</iframe>
```

## 属性

[allowfullscreen](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe#attr-allowfullscreen)
如果设置，`<iframe>`则可以通过[全屏 API] 设置为全屏模式（稍微超出本文的范围）。

[frameborder](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe#attr-frameborder)
如果设置为 1，则会告诉浏览器在此框架和其他框架之间绘制边框，这是默认行为。0 删除边框。不推荐这样设置，因为在 CSS 中可以更好地实现相同的效果。border: none;

[src](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe#attr-src)
该属性与 `<video>` / 元素表示文档中的图像。`<img>`一样包含指向要嵌入文档的 URL 路径。

[width](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe#attr-width) 和 [height](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe#attr-height)
这些属性指定你想要的 iframe 的宽度和高度。

备选内容
与 `<video>` 等其他类似元素相同，你可以在 `<iframe></iframe>` 标签之间包含备选内容，如果浏览器不支持 `<iframe>`，将会显示备选内容，这种情况下，我们已经添加了一个到该页面的链接。现在你几乎不可能遇到任何不支持 `<iframe>` 的浏览器。

[sandbox](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe#attr-sandbox)
该属性需要在已经支持其他 `<iframe>` 功能（例如 IE 10 及更高版本）但稍微更现代的浏览器上才能工作，该属性可以提高安全性设置；

> 备注： 为了提高速度，在主内容完成加载后，使用 JavaScript 设置 iframe 的 src 属性是个好主意。这使你的页面可以更快地被使用，并减少你的官方页面加载时间（重要的 SEO 指标）。

### 始终使用 sandbox 属性

想尽可能减少攻击者在你的网站上做坏事的机会，那么你应该给嵌入的内容仅能完成自己工作的权限。当然，这也适用于你自己的内容。一个允许包含在其里的代码以适当的方式执行或者用于测试，但不能对其他代码库（意外或恶意）造成任何损害的容器称为**沙盒**。

未沙盒化（Unsandboxed）内容可以做得太多（执行 JavaScript，提交表单，弹出窗口等）默认情况下，你应该使用没有参数的 sandbox 属性来强制执行所有可用的限制，如我们前面的示例所示。

如果绝对需要，你可以逐个添加权限（sandbox=""属性值内）——请参阅 [sandbox](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/iframe#attr-sandbox) 所有可用选项的参考条目。其中重要的一点是，你永远不应该同时添加 allow-scripts 和 allow-same-origin 到你的 sandbox 属性中——在这种情况下，嵌入式内容可以绕过阻止站点执行脚本的同源安全策略，并使用 JavaScript 完全关闭沙盒。

备注： 如果攻击者可以欺骗人们直接访问恶意内容（在 iframe 之外），则沙盒无法提供保护。如果某些内容可能是恶意的（例如，用户生成的内容），请保证其是从不同的域向你的主站点提供的。

### 配置 CSP 指令

CSP 代表 内容安全策略，它提供一组 HTTP 标头（由 web 服务器发送时与元数据一起发送的元数据），旨在提高 HTML 文档的安全性。在 `<iframe>` 的安全性方面，你可以将服务器配置为发送适当的 X-Frame-Options 标题。这样做可以防止其他网站在其网页中嵌入你的内容（这将导致点击劫持和一系列其他攻击），正如我们之前看到的那样，MDN 开发人员已经做了这些工作。

## 使用该`<embed>`元素嵌入 Flash 影片的示例

```html
<embed
  src="whoosh.swf"
  quality="medium"
  bgcolor="#ffffff"
  width="550"
  height="400"
  name="whoosh"
  align="middle"
  allowScriptAccess="sameDomain"
  allowFullScreen="false"
  type="application/x-shockwave-flash"
  pluginspage="http://www.macromedia.com/go/getflashplayer" />
  ```
  
  ```html
  <object
  data="mypdf.pdf"
  type="application/pdf"
  width="800"
  height="1200"
  typemustmatch>
  <p>
    You don't have a PDF plugin, but you can
    <a href="myfile.pdf">download the PDF file.</a>
  </p>
</object>
```
