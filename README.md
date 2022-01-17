# Tribute Page

致敬页app链接：[Tribute-Page (codepen.io)](https://codepen.io/lcclcclcc206/full/abLMJmG)

致敬页要求：[响应式网页设计项目 - 制作一个致敬页 | 学习 | freeCodeCamp.org](https://chinese.freecodecamp.org/learn/responsive-web-design/responsive-web-design-projects/build-a-tribute-page)



## 网页结构要点

单列流式布局

所有的元素都在 main 元素下

首先式标题部分，使用 header 元素表示

然后是一个图片和文字说明，使用 figure 表示，文字的说明用 figcaption 表示

然后是一个说明了博士一生的文字，用 article 或 section 表示，因为他有一个标题

最后面有一段引用，使用 blockquote 表示，以文本的形式告知引文的出处，使用 cite 元素



## HTML 元素要点

**HTML `<figure>` 元素**代表一段独立的内容, 经常与说明（caption） [``](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/figcaption) 配合使用, 并且作为一个独立的引用单元。当它属于主内容流（main flow）时，它的位置独立于主体。这个标签经常是在主文中引用的图片，插图，表格，代码段等等，当这部分转移到附录中或者其他页面时不会影响到主体。

**HTML `<article>` 元素**表示文档、页面、应用或网站中的独立结构，其意在成为可独立分配的或可复用的结构，如在发布中，它可能是论坛帖子、杂志或新闻文章、博客、用户提交的评论、交互式组件，或者其他独立的内容项目。

**HTML `<section>` 元素**表示一个包含在HTML文档中的独立部分，它没有更具体的语义元素来表示，一般来说会有包含一个标题。

**HTML `<blockquote>` 元素**（或者 HTML 块级引用元素），代表其中的文字是引用内容。通常在渲染时，这部分的内容会有一定的缩进（[注](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/blockquote#Notes) 中说明了如何更改）。若引文来源于网络，则可以将原内容的出处 URL 地址设置到 cite 特性上，若要以文本的形式告知读者引文的出处时，可以通过 [`<cite>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/cite) 元素。



## CSS 样式要点

首先说明主要的 html、body、main的元素样式

```css
html {
    font-size: 10px;
}
```

html的样式设置了网页的基准字体大小

```css
body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Helvetica Neue', Arial, sans-serif;
    font-size: 1.6rem;
    line-height: 1.5;
    text-align: center;
    color: #333;
    margin: 0;
}
```

字体大小为 1.6rem，代表基准字体大小乘以 1.6

line-height 为 1.5，增加文字排版的间距，更好看

默认字体颜色为黑色

------

```css
img {
    max-width: 100%;
    height: auto;
    display: block;
    margin: auto;
}
```

设置图片自动调节大小，但又不超过原图片的大小