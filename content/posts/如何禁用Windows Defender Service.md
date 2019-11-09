---
bookFlatSection: true
title: 如何禁用Windows Defender Service？
date: 2019-04-01 00:00:00
tags: 
 - windows
 - Windows Defender
 - 技巧
 - 教程
---

`微软推出的Windows10操作系统自带了Windows Defender防病毒程序，给予了电脑一定的反病毒攻击的能力，与此同时也给用户带来了一些困扰。一些用户希望能够关闭这个功能，看看应该如何操作吧。`
<!--more-->

{{< hint info >}}
**<i class="fa fa-exclamation-circle"></i> 提示**  点击了解什么是[Windows Defender Service](https://www.microsoft.com/zh-cn/windows/comprehensive-security)？
{{< /hint >}}

## 步骤速览 ##
- 使用快捷键`WIN+R`调出运行工具，输入组策略命令`gpedit.msc`，点击确定。
- 进入组策略后按照如下路径找到对应项：
`计算机配置/管理模板/Windows组件/Windows Defender防病毒程序/关闭Windows Defender防病毒程序。`
- 双击`关闭Windows Defender防病毒程序`，在弹出的窗口中选择`已启用`，点击`确定`，退出组策略编辑器。
- 在任务栏空白处点击鼠标右键，打开任务管理器，点击`启动选项卡`，右键单击`Windows Defender`将其禁用。
- 完成上述操作后重启计算机。

## 详细图解 ##
> 使用快捷键`WIN+R`调出运行工具，输入组策略命令`gpedit.msc`，点击确定。

![如何禁用Windows Defender Service](https://cdn.img.wenhairu.com/images/2019/11/07/AEy1N.png)

> 进入组策略后按照如下路径找到`关闭Windows Defender防病毒程序`：
```
计算机配置/管理模板/Windows组件/Windows Defender防病毒程序/关闭Windows Defender防病毒程序。
```

![如何禁用Windows Defender Service](https://cdn.img.wenhairu.com/images/2019/11/07/AEH4B.png)

> 双击`关闭Windows Defender防病毒程序`，在弹出的窗口中选择`已启用`，点击`确定`，退出组策略编辑器。

![如何禁用Windows Defender Service](https://cdn.img.wenhairu.com/images/2019/11/07/AEQhn.png)


> 在任务栏空白处点击鼠标右键，打开`任务管理器`，点击`启动`选项卡，右键单击`Windows Defender`将其禁用。

![如何禁用Windows Defender Service](https://cdn.img.wenhairu.com/images/2019/11/07/AEkEA.png)


![如何禁用Windows Defender Service](https://cdn.img.wenhairu.com/images/2019/11/07/AEocT.png)


> 完成上述操作后重启计算机


