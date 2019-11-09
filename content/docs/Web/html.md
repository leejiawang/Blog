---
weight: 3
bookFlatSection: true
title: "前端基础"
---

# **<i class="fa fa-tags"></i> HTML5 笔记**

`HTML称为超文本标记语言，是一种标识性的语言。它包括一系列标签，通过这些标签可以将网络上的文档格式统一，使分散的Internet资源连接为一个逻辑整体。`


## 简单介绍

{{< columns >}}

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>eyecus</title>
  </head>

  <body>
    <h1>hello world！</h1>
    <p>hello eyecus！</p>
  </body>
</html>

```
<--->
<hr>

` <!DOCTYPE html> ` ：声明为html5文档</br>
` <html> `：html页面的根元素</br>
` <head>`：包含了文档的元(meta)数据</br>
` <title>`：包含了页面标题</br>
` <body>`：包含了可见的页面内容</br>
` <h1>`：一级标题标签</br>
` <p>`：段落标签</br>

{{< /columns >}}
{{< hint warning >}}
**<i class="fa fa-exclamation-triangle"></i> 注意**

对于中文网页需要使用 `<meta charset="utf-8">` 声明编码，否则会出现乱码。
{{< /hint >}}


## 基本概念

### 参考信息 ###
<hr>

**常见属性**

标签 | 描述
:-- | :--
class | 为html元素定义一个或多个类名
id | 定义元素的唯一id
style | 规定元素的行内样式
title | 描述了元素的额外信息


**文本格式化标签**

标签 | 描述 | 预览
:-- | :-- | :-- 
`<b>` | 粗体文本 | <p>原文 <b>文本 Text</b></p>
`<em>` | 着重文字 | <p>原文 <em>文本 Text</em></p>
`<i>` | 斜体字 | <p>原文 <i>文本 Text</i></p>
`<small>` | 小号字 | <p>原文 <small>文本 Text</small></p>
`<strong>` | 加粗 | <p>原文 <strong>文本 Text</strong></p>
`<sub>` | 下标字 | <p>原文 <sub>文本 Text</sub></p>
`<sup>` | 上标字 | <p>原文 <sup>文本 Text</sup></p>
`<ins>` | 下划线 | <p>原文 <ins>文本 Text</ins></p>
`<del>` | 删除字 | <p>原文 <del>文本 Text</del></p>

### 常用功能 ###
<hr>

- 给 `XXXX` 添加 `default.html` 链接

```
<a href="default.html"> XXXX </a>
```
- 换行

```
<p> XXXX</br>XXXX </p>
```
- 添加图片，并定义尺寸

```
<img src="/images/logo.png" width="250" height="200" />
```
- 添加水平线

```
<p>XXXX</p>
<hr>
<p>XXXX</p>
```
- 添加注释

```
<!-- XXXX -->
```
- 添加图片，并定义尺寸

```
<img src="/images/logo.png" width="250" height="200" />
```


<div>&nbsp&nbsp&nbsp&nbsp</div>

<div align="center">  
<h3>👨🏻‍💻 持续更新中...</h3>
</div>

<div>&nbsp&nbsp&nbsp&nbsp</div>

<hr>

<hr>

# **<i class="fa fa-tag"></i> CSS 笔记**

`层叠样式表(Cascading Style Sheets)是一种用来表现HTML或XML等文件样式的计算机语言。CSS不仅可以静态地修饰网页，还可以配合各种脚本语言动态地对网页各元素进行格式化。`


## 简单介绍

> **CSS的常用格式**
{{< columns >}}

```
p {
   color:red;
   text-align:center;
}
```

<--->

 ` p ` **：选择器**是需要改变样式的元素

 ` color `**：属性**是需要改变的样式属性

 ` red` **：值**是属性的描述值

{{< /columns >}}

## 基本属性

### 文本属性 ###

<hr>

属性 | 功能描述 | 值举例
:-- | :-- | :--
color | 颜色 | `#ffffff(颜色代码)`
direction | 文本方向 | `ltr(左到右)` `rtl(右到左)` 
letter-spacing | 字间距 | `-3px(数值)`
line-height | 行高 | `200%(百分数)`
text-align | 对齐 | `center(居中)` </br>`left(左对齐)` </br>`right(右对齐)`
text-decoration | 文本修饰 | `overline wavy red(上划红色波浪线)` </br>`line-through(删除线)` </br>`underline(下划线)`
text-indent | 首行缩进 | `3px(数值)`
text-shadow | 文本阴影 |  `2px 2px #ff0000(XY偏移值、颜色代码)`
text-transform | 字母大小写 | `uppercase(大写)` </br>`capitalize(大小写)` </br>`lowercase(小写)`
vertical-align | 垂直对齐 | `baseline(在父元素的基线上)`</br>`sub(垂直对齐文本下标)`</br>`super(垂直对齐文本上标)`</br>`top( 顶端与行中最高元素顶端对齐)`</br>`text-top( 顶端与父元素字体顶端对齐)`</br>`middle(在父元素的中部)`</br>`bottom(底端与行中最低的元素顶端对齐)`</br>`text-bottom(底端与父元素字体底端对齐)`</br>`-30%(使用line-height的值来排列此元素)`</br>`inherit(从父元素继承属性)`
white-space | 空白区域处理 | `normal(忽略)` </br>`pre(保留)` </br>`nowrap(不换行直到</br>)` </br>`pre-wrap(保留并正常换行)` </br>`pre-line(合并空白符)` </br>`inherit(从父元素继承属性)`
word-spacing | 字间距 | `3px(数值)`

### 背景属性 ###

<hr>

属性 | 功能描述 | 值举例
:-- | :-- | :--
background-color | 背景颜色 | `#ffffff(颜色代码)`
background-image | 背景图像 | `url('paper.gif')(图片URL)` 
background-repeat | 背景图像排列 | `repeat-x(水平平铺)` </br>`repeat-y(垂直平铺)` </br>`no-repeat(不平铺)`
background-position | 背景图像定位 | `right top(左上角)`
background-attachment | 背景图像滚动 | `flase(假)` `true(真)`


> 背景属性简写为`background`，值得写法如下
```
body {background:#ffffff url('img_tree.png') no-repeat right top;}
```

### 字体属性 ###

<hr>

属性 | 功能描述 | 值举例
:-- | :-- | :--
font-family | 字体系列 | `"Times New Roman"(字体名)` </br>`sans-serif(无衬线字体)` </br> `serif(衬线字体)`
font-style | 字体样式 | `normal(正常)` </br>`italic(斜体)`</br> `oblique(倾斜)`
font-size | 字体大小 | `40px(数值)`</br> `2.5em(数值,px/16=em)`</br> `100%(百分数,body属性值*100%)`
font-weight | 字体粗细 | `200(整百分数)` 




<div>&nbsp&nbsp&nbsp&nbsp</div>

<div align="center">  
<h3>👨🏻‍💻 持续更新中...</h3>
</div>

<div>&nbsp&nbsp&nbsp&nbsp</div>

<hr>

<hr>

# **<i class="fa fa-tag"></i> Bootstrap4 笔记**

`Bootstrap 是一套流行的前端框架，轻松构建对移动设备很友好的响应式网站。内置了大量常用界面设计组件，大大简化了建站的过程。`


## 加载 Bootstrap


- **CSS：**复制如下代码到`HTML`的`<head>`标签。
```
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
```
- **JS：**复制如下代码到`HTML`的`</body>`标签之前。
```
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
```

- **简单 Bootstrap 实例**
```
<!DOCTYPE html>
<html>
<head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
        <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
        <title>XXXX</title>
</head>
<body>
        <h1>XXXX</h1>
        <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.3/umd/popper.min.js" integrity="sha384-ZMP7rVo3mIykV+2+9J3UJ46jBk0WLaUAdn689aCwoqbBJiSnjAK/l8WvCWPIPm49" crossorigin="anonymous"></script>
        <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
</body>
</html>
```


## 基本概念

### 容器 ###
<hr>

- 容器是`Bootstrap`中最基本的布局基础。会自动根据屏幕大小来选择合适的宽度。
```
<div class="container">
        XXXX
</div>
```
标签 | 名称 | 描述
:-- | :-- | :--
container | 容器 | 自动根据屏幕大小来选择合适的宽度
container-fluid | 全宽容器 | 跨越 viewport 的整个宽度 

### 响应式断点 ###
<hr>

- 响应式断点指使用少量媒体查询为布局和界面创建合理的断点，以此动态调节显示界面尺寸。
{{< hint info >}}
**<i class="fa fa-exclamation-circle"></i> 提示** 下述代码中具体尺寸更具需要进行更改。
{{< /hint >}}

```
@media (min-width: 576px) and (max-width: 767.98px) {  }
@media (min-width: 768px) and (max-width: 991.98px) {  }
@media (min-width: 992px) and (max-width: 1199.98px) {  }
```

### Z-index ###
<hr>

- `Z-index`值用于正确地分层，确然各个元素的层叠覆盖关系。
```
.XXXX {
         z-index: X;
}
```


<div>&nbsp</div>


<div align="center">  
<h3>👨🏻‍💻 持续更新中...</h3>
</div>

