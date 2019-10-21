---
weight: 2
bookFlatSection: true
title: "Hugo建站教程"
---

# **Hugo搭建静态网站简易教程**

{{< columns >}}
**Hugo**是由`Go语言`实现的**静态网站生成器**，简单、易用、高效、易扩展、快速部署。

[`Hugo官网`](https://gohugo.io) [`Hugo主题`](https://themes.gohugo.io) [`Hugo中文`](https://www.gohugo.org) [`Hugo仓库`](https://github.com/gohugoio/hugo)

<--->
<div align="center"> 
<img src="https://d33wubrfki0l68.cloudfront.net/c38c7334cc3f23585738e40334284fddcaf03d5e/2e17c/images/hugo-logo-wide.svg" width=250 />
</div>
{{< /columns >}}

{{< hint info >}}
本站即为Hugo博客框架搭建，使用了Hugo-Book主题。
{{< /hint >}}

## **第1步 安装Hugo框架**

> 首先根据自己的系统参照下述方法安装`hugo博客框架`。

{{< tabs "uniqueid" >}}
{{< tab "macOS 🔥" >}}

- macOS操作系统下直接使用`Homebrew`安装，在终端中输入如下代码：
```   
brew install hugo
```
{{< hint warning >}}
**⚠️ 注意**  
执行此操作前请确保macOS安装有[Homebrew](https://brew.sh)。
{{< /hint >}}

{{< /tab >}}

{{< tab "Windows" >}}
- 在[Hugo Releases](https://github.com/gohugoio/hugo/releases)下载最新发布对应操作系统的`ZIP`，将所有内容提取到`C:\Hugo\bin`目录中，包含可执行文件`hugo.exe`、`LICENSE`和`README.md`。

- 然后将Hugo添加到Windows的`PATH`设置中。
  - 右键单击`开始`按钮
  - 单击`系统`
  - 单击左侧的`高级系统设置`
  - 单击底部的`环境变量...`按钮
  - 在`用户变量`部分中找到以PATH开头的行（PATH全部大写）
  - 双击`PATH`
  - 单击`新建…`按钮
  - 键入`C:\Hugo\bin`，完成输入后按`Enter`
  - 在每个窗口中单击`确定`退出

{{< /tab >}}

{{< tab "Linux" >}}
- Linux操作系统下直接使用` Homebrew`安装，在终端中输入如下代码:
```   
brew install hugo
```
{{< hint warning >}}
**⚠️ 注意**  
执行此操作前请确保linux安装有[Homebrew](https://docs.brew.sh/Homebrew-on-Linux)。
{{< /hint >}}

{{< /tab >}}

{{< tab "OpenBSD" >}}
- OpenBSD通过`pkg_add`添加Hugo的软件包：
```   
doas pkg_add hugo
```
{{< /tab >}}

{{< tab "源码安装" >}}
- 在[Hugo Releases](https://github.com/gohugoio/hugo/releases)下载对应操作系统的Hugo安装文件，执行安装。
{{< hint warning >}}
**⚠️ 注意**  
执行源码安装前请确保安装有[`Git`](https://git-scm.com/)、[`Mercurial`](https://www.mercurial-scm.org/)、[`Go`](http://golang.org/)。
{{< /hint >}}

- 设置好`GOPATH`环境变量，获取源码(源码会下载到`GOPATH/src`目录)并编译。
```
export GOPATH=$HOME/go
go get -v github.com/spf13/hugo
```

{{< /tab >}}

{{< /tabs >}}

> 安装完Hugo后，在终端中输入如下代码验证安装。

```
hugo version
```

## **第2步 生成网站**

> 在终端中输入如下代码生成网页。


```
hugo new site test
```
{{< hint info >}}
**💡 提示**  
代码中`test`是所创建的网站文件夹名称，由用户自定义，以下网站名均由`test`代指。
{{< /hint >}}

## **第3步 网站配置(套用主题)**
> 进入网站根目录

```
cd test
```

> 安装`Git`（用于下载主题）

```
git init
```

> 在`主题商店`中选择自己喜欢的主题，查看其Github仓库地址，使用如下代克隆主题至本地。
>  Hugo主题商店地址：[`themes.gohugo.io`](https://themes.gohugo.io/)、[`gohugo.org/theme`](https://www.gohugo.org/theme/)

```
git clone https://github.com/XXXXX/XXXX themes/XXXX
```

{{< hint info >}}
**💡 提示**  
代码中网址为主题Github仓库地址，`XXXX`为主题文件夹名称。
{{< /hint >}}

> 编辑网站根目录中`config.toml`文件，添加代码`theme = "XXXX"`以确认所使用的主题。

- `config.toml`默认格式如下
```
baseURL = "https://example.org/"
languageCode = "en-us"
title = "test"
theme = "XXXX"
```

## **第4步 添加页面**
> 添加新页面，页面内容采用`Markdown`格式。

```
hugo new posts/my-first-post.md
```

- 页面默认格式如下

```
---
title: "My First Post"
date: 2019-10-20T00:00:00+01:00
draft: true
---
```
{{< hint info >}}
**💡 提示**  
代码中`my-first-post`为Markdown页面文件名，`title: "My First Post"`所写内容才是网站显示的标题，页面格式根据主题不同略有不同，详见主题描述。
{{< /hint >}}

## **第5步 运行网站**
> 完成上述操作后，可在终端中输入如下代码运行网站。

```
hugo server -D
```

- 浏览器访问[`http://localhost:1313/`](http://localhost:1313/)预览效果。你可在预览的同时对网站进行编辑，网页将会实时展示修改后的效果，如果出现刷新问题可通过`Ctrl+R`进行强制刷新。

## **第6步 生成静态网页**
> 在终端中输入如下代码生成静态网页。

```
hugo
```
{{< hint info >}}
**💡 提示**  
以上命令并不会生成草稿页面，需要生成的页面请去掉页面头部的`draft: true`。
{{< /hint >}}

- 默认情况下生成的文件会输出到`test/public/`目录下，你可将改文件夹部署到服务器以实现远程访问，也可使用本文第7步所说的方法。

## **第7步 部署 Github Pages**
本文所使用的Github Pages并非部署网页的唯一提供商，你也可以使用`Coding`、`Gitee`等。
{{< hint warning >}}
**⚠️ 注意**  
执行此操作前请确保拥有Github账号，并创建一个以`XXX.github.io`命名的空仓库。(其中`XXX`为你的Github用户名)
{{< /hint >}}

> 在终端中输入如下代码生成最终页面。

```
hugo --theme=XXXX --baseUrl="http://XXX.github.io/"
```

> 在终端中输入下列代码将最终页面部署到Github Pages。

```
cd public
git init
git remote add origin https://github.com/XXX/XXX.github.io.git
git add -A
git commit -m "first commit"
git push -u origin master
```
- 浏览器输入`http://XXX.github.io/`实现远程访问。

<div>&nbsp&nbsp&nbsp&nbsp</div>

<div align="center">  
<h5>MIT Licensed | Copyright © 2019 <strong>世佳</strong></h5>
</div>
