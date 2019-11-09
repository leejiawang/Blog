---
bookFlatSection: true
title: Win10系统如何关闭自动更新？
date: 2019-04-01 00:30:00
enable: true
tags: 
 - windows
 - Windows update
 - 升级
 - 技巧
 - 教程

---

`为了避免在重要时刻被Windows更新打断，合理的安排更新时间。看看关掉烦人的Win10自动更新。`
<!--more-->
{{< hint warning >}}
**<i class="fa fa-exclamation-triangle"></i> 注意**
由于方法涉及使用运用组策略，故`Windows10家庭版`可能不适用。
{{< /hint >}}

## 步骤速览 ##
- 快捷键`WIN+R`调出运行工具，输入组策略命令`services.msc`，点击确定;
- 在服务中找到`Windows Update`选项，双击;
- 在“启动类型”下选择“禁用”，并点击确定。

![Win10系统如何关闭自动更新](https://cdn.img.wenhairu.com/images/2019/11/07/AEMBU.png)

## 详细图解 ##
> 快捷键`WIN+R`调出运行工具，输入组策略命令`services.msc`，点击确定。

![Win10系统如何关闭自动更新](https://cdn.img.wenhairu.com/images/2019/11/07/AE73G.png)

> 在服务中找到`Windows Update`选项，双击。

![Win10系统如何关闭自动更新](https://cdn.img.wenhairu.com/images/2019/11/07/AEcfv.png)

> 在`启动类型`下选择`禁用`，并点击确定。

![Win10系统如何关闭自动更新](https://cdn.img.wenhairu.com/images/2019/11/07/AEgQ0.png)




