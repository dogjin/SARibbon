# 简介
 这是一个轻量级的Ribbon控件(Office样式UI),界面截图：

![](https://github.com/czyt1988/SARibbon/raw/master/doc/screenshot/001.gif)

# 编译方法

 使用Qt Creator直接打开SARibbonBar.pro，并编译即可，会编译出SARibbonBar库和一个（目前只有一个例子）例子，lib和例子的目录位于bin目录下

# 使用方法

可以把编译好的整个目录移动到需要的工程目录下，然后在项目的pro文件中,`include SARibbonBar.pri`即可，示例如下：
```
include($$PWD/SARibbonBar/SARibbon/SARibbonBar.pri)
```
使用cmakefile的话自己手撸

# 题外

这个Ribbon主要靠`QSS`实现而不是重写样式(`QStyle`)，主要是重写样式工作量巨大，一些`QSS`无法实现的，重写了界面，如RibbonToolButton，

目前只完成了最基本的一些功能如:Ribbon的整体界面，Ribbon的ToolButton等基本功能，像RibbonGallery这样的功能仍然需要完善

更多界面截图可看：

[https://github.com/czyt1988/sa](https://github.com/czyt1988/sa)

SARibbon项目是SA项目的子项

具体Ribbon的生成代码可见：
[https://github.com/czyt1988/sa/blob/master/src/signA/MainWindowPrivate.cpp](https://github.com/czyt1988/sa/blob/master/src/signA/MainWindowPrivate.cpp)
