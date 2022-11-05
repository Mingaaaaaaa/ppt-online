---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://images.unsplash.com/photo-1621237023000-6a628c285938?crop=entropy&cs=tinysrgb&fit=crop&fm=jpg&h=1080&ixid=MnwxfDB8MXxyYW5kb218MHw5NDczNDU2Nnx8fHx8fHwxNjY3NjIxMDU3&ixlib=rb-4.0.3&q=80&utm_campaign=api-credit&utm_medium=referral&utm_source=unsplash_source&w=1920
# apply any windi css classes to the current slide
class: "text-center"
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: false
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS
css: unocss
---

# **HTML 结尾与 CSS 入门**

欢迎大家来听南邮校科协前端组第二次授课 🥳

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---

#### 前情提要 🤤：

上节课，卡密学长带领我们走进了前端世界：

1. ##### 了解了前端是什么

   > 前端即网站前台部分，运行在 PC 端，移动端等浏览器上展现给用户浏览的网页。包括小程序和 App 等展示内容的界面

2. ##### 配置好了前端开发的基本环境，安装了常用到的插件和工具
   并获得了卡密的礼物 😍

<img src="https://cdn.staticaly.com/gh/Mingaaaaaaa/PictureBed@master/xxx/image-20221104164205724.2k8m6zbhddk0.webp" style="zoom: 25%;" />

---

3. ##### 学习了前端三大件之一：HTML 的部分知识

  <img src="https://cdn.staticaly.com/gh/Mingaaaaaaa/PictureBed@master/xxx/image-20221104164616431.44cwfm2erp40.webp" style="zoom:15%;" />

<img src="https://cdn.staticaly.com/gh/Mingaaaaaaa/PictureBed@master/xxx/image-20221104164429434.r7frh98uir4.webp" style="zoom:30%;" />

##### 4.作业讲解

上次课我们也布置了一个小小的作业。

我们也收到了不少同学的作业啦，很高兴！！！在这里，我们简单的演示一下作业的要求。

---

### **HTML 结尾**

这节课我们会学习 HTML 中的 [**表格**](https://developer.mozilla.org/zh-CN/docs/Learn/HTML/Tables)与[**表单**](https://developer.mozilla.org/zh-CN/docs/Learn/Forms)

##### **表格**

用表格来展示数据会大大提升用户的体验。一个好的表格能让浏览者的效率大大提高。

表格的基本元素如下：

```
<table> :表格的标签，表格里的内容都写着<table>标签内
<td> : table data 代表一个单元格
<tr> : table row  在这个标签内的单元格会在同一行
<th> : table head  一般用于表格的行或列的开头
```

<br>
让我们动手写一个表格康康

---

更进一步的：

实际情况中，我们可能我们让一个一个单元格更长更宽

<img src="https://cdn.staticaly.com/gh/Mingaaaaaaa/PictureBed@master/xxx/image-20221104182557585.4jrjr2tlaba0.webp" style="zoom:25%;" />

这时候只需要给指定的单元格加一个 colspan 或者 rowspan 的属性

---

##### 表单

web 表单是用户和 web 站点或应用程序之间交互的主要内容之一。它们允许用户输入数据，大多数情况下会将数据发送到 web 服务器进行处理和存储（见[发送表单数据](https://developer.mozilla.org/zh-CN/docs/Learn/Forms/Sending_and_retrieving_form_data)），或者在客户端使用某种方式立刻更新界面

举例子： 登录的表单 、信息录入……

<img src="https://cdn.staticaly.com/gh/Mingaaaaaaa/PictureBed@master/xxx/image-20221104183445177.52wei34vmco0.webp" style="zoom: 33%;" />

---

刚才表单的源代码为

```html
<form action="/my-handling-form-page" method="post">
  <ul>
    <li>
      <label for="name">Name:</label>
      <input type="text" id="name" name="user_name" />
    </li>

    <li>
      <label for="mail">E-mail:</label>
      <input type="email" id="mail" name="user_mail" />
    </li>

    <li>
      <label for="msg">Message:</label>
      <textarea id="msg" name="user_message"></textarea>
    </li>
    <li class="button">
      <button type="submit">Send your message</button>
    </li>
  </ul>
</form>
```

---

### **CSS 入门**

<br>
<img  src="https://pic3.zhimg.com/bf00a25bae235e3ea9a9936cdfad89ca_b.jpg" alt="img" style=" zoom: 60%;" />
<br>
<br>

可能你也发现了，我们只用 HTML 写出来的网站，怎么和我们平时冲浪时浏览的网站差距这么大！！
<br>
<br>

我们举个栗子

---

#### **什么是 CSS?**

层叠样式表 — 也就是[CSS](https://developer.mozilla.org/zh-CN/docs/Glossary/CSS)。HTML 用于定义内容的结构和语义，CSS 用于设计风格和布局。比如，您可以使用 CSS 来更改内容的字体、颜色、大小、间距，将内容分为多列，或者添加动画及其他的装饰效果。

<img src="https://pica.zhimg.com/80/v2-81c7ec804ac186d33bdcbea061e6cd43_1440w.webp?source=1940ef5c" alt="img" style="zoom:80%;" />

---

##### **CSS 的由来**

[世界上第一个网站 ](https://www.w3.org/History/19921103-hypertext/hypertext/WWW/TheProject.html)

<p style="font-size:10px">随着HTML的成长，为了满足页面设计者的要求，HTML添加了很多显示功能。但是随着这些功能的增加，HTML变的越来越杂乱，而且HTML页面也越来越臃肿。于是CSS便诞生了。

1994 年哈坤·利提出了 CSS 的最初建议。而当时伯特·波斯（_Bert Bos_）正在设计一个名为 Argo 的浏览器，于是他们决定一起设计 CSS。

其实当时在互联网界已经有过一些统一样式表语言的建议了，但 CSS 是第一个含有“层叠”丰意的样式表语言。

哈坤于 1994 年在芝加哥的一次会议上第一次提出了 CSS 的建议，

1995 年的 www 网络会议上 CSS 又一次被提出，博斯演示了 Argo 浏览器支持 CSS 的例子，哈肯也展示了支持 CSS 的 Arena 浏览器。

同年，W3C 组织（_World WideWeb Consortium_）成立，CSS 的创作成员全部成为了 W3C 的工作小组并且全力以赴负责研发 CSS 标准，层叠样式表的开发终于走上正轨。

有越来越多的成员参与其中，例如微软公司的托马斯·莱尔顿(Thomas Reaxdon)，他的努力最终令 Internet Explorer 浏览器支持 CSS 标准。哈坤、波斯和其他一些人是这个项目的主要技术负责人。

1996 年底，CSS 初稿已经完成，同年 12 月，层叠样式表的第一份正式标准（_Cascading style Sheets Level 1_）完成，成为 w3c 的推荐标准。</p>

---

##### **CSS 基础语法**

<p style="font-size:10px">
CSS 是一门基于规则的语言 —— 你能定义用于你的网页中特定元素样式的一组规则。

让我们来给我们的界面加点 CSS

比如“我希望页面中的主标题是红色的大字”

</p>

```
h1 {
    color: red;
}
```

这里由 **[ 选择器](https://developer.mozilla.org/zh-CN/docs/Learn/CSS/Building_blocks/Selectors)** 开头 **h1**

接着跟着一对 大括号 **{ }** ，<br>

大括号内部定义一个或多个形式为 **属性** ： **值；** <br>

（如 color :red； color 是设置 h1 的属性，red 表示设置 h1 的颜色为 red）

---

### 同时 CSS 中还有很多选择器：<img src="https://cdn.staticaly.com/gh/Mingaaaaaaa/PictureBed@master/xxx/image-20221105094626130.xe2c7v3zaps.webp" style="zoom:50%;" />

我们这节课讲比较基础的几个

1. **类型选择器** :也叫元素选择器，通过用节点的名称来给节点加 CSS 样式 `h1{}`
2. **通配符选择器**: 可以理解为全部的意思，单独使用`*{color :red }` 会使所有元素变红
3. **类选择器** :我们可以给一个或多个元素加一个 class 的属性，意思是把它归为一个类 然后我们对一个类进行操作
4. **ID 选择器** :我们给某个特定元素加上 id 的属性，然后就可以单独给它给它加样式

我们在这里分别演示一下它们的使用

---

### 选择器的优先级：

你可能会发现，

某些情况下，一个元素（比如说`<p>`）可能既通过类型选择器添加样式，也有类选择器，id 选择器等多个选择器对它的样式进行设置。假如都对它的颜色进行了不同的设置，那么哪个颜色会生效呢

**选择器的优先级：行内样式>ID 选择器>类选择器>标签选择器（元素选择器）>通用符**

**特殊的 !important**

---

### CSS 代码写在哪里呢？

学习了怎么写 CSS ,那我们怎么把上面那段代码应用到我们的网页中呢？有以下**三种方法**

1. **外联样式(推荐)** ：

   在 HTML 文档的相同目录创建一个文件，保存并命名为 `styles.css`

   然后在文档的开头链接 CSS ，

   ```
    <link rel="stylesheet" href="styles.css">
   ```

2. **内部样式**：

   在 HTML 的`<Body>`标签中 增加一个`<style> </style>`标签 然后在这里面写 CSS

3. **行内样式**

   存在于 HTML 元素的 style 属性之中。其特点是每个 CSS 表只影响一个元素，如：

   ```
      <p style="color:red;">This is my first CSS example</p>
   ```

   我们分别演示一遍

---

### **盒式模型**

在 CSS 中，所有的元素都被一个个的“盒子（box）”包围着，理解这些“盒子”的基本原理，是我们使用 CSS 实现准确布局、处理元素排列的关键。

盒子模型包含了：元素内容、内边距（padding）、边框（border）、外边距（margin）

![image-20221105104546298](https://cdn.staticaly.com/gh/Mingaaaaaaa/PictureBed@master/xxx/image-20221105104546298.7345bqnn1f40.webp)

实践： CSS IS AWESOME

---

### **CSS 是如何运行的呢**

<img src="https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_works/rendering.svg" alt="img" style="zoom: 25%;" />

---

#### 写在最后：

当然啦，本节课我们给大家分享了最基本的 CSS 知识，

但想通过这一节课来掌握 CSS 还是远远不够的。

比如说 CSS 中还有很多有意思的东西等着我们去探索，

如样式化文本、CSS 排版中的 Flex 布局、 Grid 布局和动画 animation 等。

如今大部分网站的使用体验和美观程度已经相当优秀，其中有很大一部分是 CSS 的功劳。

学习并掌握 CSS 也是我们在学习网页开发时必不可缺的一部分

---

##### 课外补充：

无敌的开发者工具

同时我们还可以使用开发者工具（F12/右键检查）去查看并学习优秀网站的 CSS 样式

获取视频封面小技巧:
先按下 Shift +Ctrl + C ,再点击对应的视频封面，这时候右边会出现对应图片信息，鼠标移到信息上就可以看到图片 url 了
