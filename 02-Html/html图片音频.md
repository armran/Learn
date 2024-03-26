
# 图片音频

## 图片 img

```html
<figure>
  <img
    src="dinosaur_small.jpg"
    alt="一只恐龙头部和躯干的骨架，它有一个巨大的头，长着锋利的牙齿。"
    width="400"
    height="341" />
  <figcaption>曼彻斯特大学博物馆展出的一只霸王龙的化石</figcaption>
</figure>

<div class="figure">
  <img
    src="/images/dinosaur_small.jpg"
    alt="一只恐龙头部和躯干的骨架，它有一个巨大的头，长着锋利的牙齿。"
    width="400"
    height="341" />
  <p>曼彻斯特大学博物馆展出的一只霸王龙的化石</p>
</div>
```

`<figure>` 元素代表一段独立的内容，可能包含 `<figcaption>` 元素定义的说明元素。该插图、标题和其中的内容通常作为一个独立的引用单元。

用css

```css
p {
  background-image: url("images/dinosaur.jpg");
}
```

### 分辨率切换：不同的尺寸

```html
<img
  srcset="elva-fairy-480w.jpg 480w, elva-fairy-800w.jpg 800w"
  sizes="(max-width: 600px) 480px,
         800px"
  src="elva-fairy-800w.jpg"
  alt="Elva dressed as a fairy" />
```

### 分辨率切换：相同的尺寸，不同的分辨率

```html
<img
  srcset="elva-fairy-320w.jpg, elva-fairy-480w.jpg 1.5x, elva-fairy-640w.jpg 2x"
  src="elva-fairy-640w.jpg"
  alt="Elva dressed as a fairy" />
```

### 其他写法

让我们改用 `<picture>`！就像 `<video>` 和 `<audio>`，`<picture>`元素包含了一些 `<source>` 元素，它使浏览器在不同资源间做出选择，紧跟着的是最重要的 `<img>` 元素。responsive.html 的代码如下：

```html
<picture>
  <source media="(max-width: 799px)" srcset="elva-480w-close-portrait.jpg" />
  <source media="(min-width: 800px)" srcset="elva-800w.jpg" />
  <img src="elva-800w.jpg" alt="Chris standing up holding his daughter Elva" />
</picture>
```

像 WebP 和 AVIF 等新型图片格式可以做到高质量的同时保持较低的文件大小，如今这些格式已有相对广泛的浏览器支持，且几乎没有“历史包袱”。

```html
<picture>
  <source type="image/svg+xml" srcset="pyramid.svg" />
  <source type="image/webp" srcset="pyramid.webp" />
  <img
    src="pyramid.png"
    alt="regular pyramid built from four equilateral triangles" />
</picture>
```

## 音视频

### 视频 video

```html
<video src="rabbit320.webm" controls>
  <p>
    你的浏览器不支持 HTML5 视频。可点击<a href="rabbit320.mp4">此链接</a>观看
  </p>
</video>

<video
  controls
  width="400"
  height="400"
  autoplay
  loop
  muted
  poster="poster.png">
  <source src="rabbit320.mp4" type="video/mp4" />
  <source src="rabbit320.webm" type="video/webm" />
  <p>
    你的浏览器不支持 HTML5 视频。可点击<a href="rabbit320.mp4">此链接</a>观看
  </p>
</video>

```

用户必须能够控制视频和音频的回放功能。你可以使用 `controls` 来包含浏览器提供的控件界面，同时你也可以使用合适的 `JavaScript API` 创建自己的界面。界面中至少要包含开始、停止以及调整音量的功能。

#### `width`和`height`

你可以用属性控制视频的尺寸，也可以用 CSS 来控制视频尺寸。无论使用哪种方式，视频都会保持它原始的长宽比 — 也叫做纵横比。如果你设置的尺寸没有保持视频原始长宽比，那么视频边框将会拉伸，而未被视频内容填充的部分，将会显示默认的背景颜色。

#### autoplay

这个属性会使音频和视频内容立即播放，即使页面的其他部分还没有加载完全。建议不要应用这个属性在你的网站上，因为用户们会比较反感自动播放的媒体文件。

#### loop

这个属性可以让音频或者视频文件循环播放。同样不建议使用，除非有必要。

#### muted

这个属性会导致媒体播放时，默认关闭声音。

#### poster

这个属性指向了一个图像的 URL，这个图像会在视频播放前显示。通常用于粗略的预览或者广告。

#### preload

这个属性被用来缓冲较大的文件，有 3 个值可选：

- "none" ：不缓冲
- "auto" ：页面加载后缓存媒体文件
- "metadata" ：仅缓冲文件的元数据

### 音频 audio

```html
<audio controls>
  <source src="viper.mp3" type="audio/mp3" />
  <source src="viper.ogg" type="audio/ogg" />
  <p>你的浏览器不支持 HTML5 音频，可点击<a href="viper.mp3">此链接</a>收听。</p>
</audio>
```

音频播放器所占用的空间比视频播放器要小，由于它没有视觉部件 — 你只需要显示出能控制音频播放的控件。一些与 HTML5 `<video>` 的差异如下：

- `<audio>` 标签不支持 width/height 属性 — 由于其并没有视觉部件，也就没有可以设置 width/height 的内容。
- 同时也不支持 poster 属性 — 同样，没有视觉部件。
  
除此之外，`<audio>` 标签支持所有 `<video>` 标签拥有的特性 — 你可以回顾上面的章节来了解更多的有关信息。

## 重新播放媒体

任何时候，你都可以在 Javascript 中调用 load() 方法来重置媒体。如果有多个由 `<source>` 标签指定的媒体来源，浏览器会从选择媒体来源开始重新加载媒体。

```JS
const mediaElem = document.getElementById("my-media-element");
mediaElem.load();
```

## 音轨增删事件

你可以监控媒体元素中的音频轨道，当音轨被添加或删除时，你可以通过监听相关事件来侦测到。具体来说，通过监听 `AudioTrackList` 对象的 `addtrack` 事件（即 `HTMLMediaElement.audioTracks` 对象），你可以及时对音轨的增加做出响应。

```JS
const mediaElem = document.querySelector("video");
mediaElem.audioTracks.onaddtrack = function (event) {
  audioTrackAdded(event.track);
};
```

## 视频字幕track

一个`media` 元素的任意两个`track` 子元素不能有相同的 `kind`, `srclang`, 和 `label`属性。

```html
<video controls poster="/images/sample.gif">
   <source src="sample.mp4" type="video/mp4">
   <source src="sample.ogv" type="video/ogv">
   <track kind="captions" src="sampleCaptions.vtt" srclang="en">
   <track kind="descriptions"
     src="sampleDescriptions.vtt" srclang="en">
   <track kind="chapters" src="sampleChapters.vtt" srclang="en">
   <track kind="subtitles" src="sampleSubtitles_de.vtt" srclang="de">
   <track kind="subtitles" src="sampleSubtitles_en.vtt" srclang="en">
   <track kind="subtitles" src="sampleSubtitles_ja.vtt" srclang="ja">
   <track kind="subtitles" src="sampleSubtitles_oz.vtt" srclang="oz">
   <track kind="metadata" src="keyStage1.vtt" srclang="en"
     label="Key Stage 1">
   <track kind="metadata" src="keyStage2.vtt" srclang="en"
     label="Key Stage 2">
   <track kind="metadata" src="keyStage3.vtt" srclang="en"
     label="Key Stage 3">
   <!-- Fallback -->
   ...
</video>
```

### WebVTT cues

1. 第一行以时间开始，这是显示下面显示的文本的开始时间。
2. 在同一行上，我们有一个字符串“-->”。
3. 我们用第二个时间结束第一行，这是显示相关文本的结束时间。
4. 然后，我们可以有一行或多行以连字符（-）开头，每行都包含要显示的文本轨道的一部分。
5. NOTE 后面是注释.

```vtt
WEBVTT - This file has cues.

14
00:01:14.815 --> 00:01:18.114
- What?
- Where are we now?

15
00:01:18.171 --> 00:01:20.991
- This is big bat country.

16
00:01:21.058 --> 00:01:23.868
- [ Bats Screeching ]
- They won't get in your hair. They're after the bugs.
```

### 属性

#### `default`

该属性定义了该 track 应该启用，除非用户首选项指定了更合适一个 track。每个媒体元素里面只有一个 `track` 元素可以有这个属性。

#### `kind`

定义了 text track 应该如何使用。如果省略了该属性，默认的 kind 值就是 `subtitles`。下面是允许的关键字：

- `subtitles`
  - 字幕给观影者看不懂的内容提供了翻译。比如英文电影里非英文的对话框或者文字。
  - 字幕可能包含额外的内容，通常有附加的背景信息。比如在电影星球大战开头的文字，或者某个场景的日期，时间，还有地点。
- `captions`
  - 隐藏式字幕提供了音频的转录甚至是翻译。
  - 可能包含重要的非言语的信息，比如音乐提示或者音效。可以指定提示音的源文件 (e.g. music, text, character).
  - 适用于耳聋的用户或者当调成静音的时候。
- `descriptions`
  - 视频内容的文本描述。
  - 适用于失明用户或者当视频不可见的场景。
- `chapters`
  - 章节标题用于用户浏览媒体资源的时候。
- `metadata`
  - 脚本使用的 track。对用户不可见。
- `label`
  - 当列出可用的 text tracks 时，给浏览器使用的 text track 的标题，这种标题是用户可读的。

- src
track 的地址。必须是合法的 URL。该属性必须定义。

- srclang
track 文本数据的语言。它必须是合法的 BCP 47 语言标签。如果 kind 属性被设为 subtitles, 那么 srclang 必须定义。
