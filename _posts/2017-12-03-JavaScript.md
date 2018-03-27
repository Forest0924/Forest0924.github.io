---
layout: post
title: javascript小记
author: Forest0924
date: 2017.12.03 10:00:00 +0800
categories: Blog
tag: Blog
---

JavaScript
笔记

一、简单的动态
document document.write()输出
alert alert()弹框
confirm confirm() 带『确认』『取消』按钮的提示框，有布尔型返回值
prompt prompt(str1,str2) 问询提示框，带『确认』 『取消』键，返回值为变量
window.open(url,「窗口名称」,『参数字符串』)打开一个新窗口，返回一个窗口对象
var.close() 关闭窗口。var为窗口对象
document.getElementById(id)通过id获取id对象或者变量。id为html申明
id-var.innerHTML 通过document获取的html元素可通过innerHTML修改
id-var.style.xxx 能过.style可修改相应的css属性
id-var.style.display 修改此属性实现显示(block)或隐藏(none)
id-var.className 修改外观样式
var var-name=function 函数名(){}带参的函数调用时直接传入参数即可，声明时亦不需要指定类型值

二、事件
事件是可以被JavaScript侦测到的行为
主要事件表
onclick
onmouseover
onmouseout
onchange
onselect
onfocus
onblur
onload
onunload 使用window.onunload

三、对象
JavaScript中所有的事物都是对象，每个对象都带有属性和方法
对象的属性：反映对象的某些特定的性质
对象的方法：能够在对象上执行的动作

四、window对象
javascript计时器
setTimeout()	指定的延迟时间来执行这段代码
clearTimeout()	  取消setTimeout()设置
setInterval()			每隔指定的时间执行代码
clearInterval()		取消setInterval()设置
history对象 加载浏览器的历史记录 属性：length，方法：back(),forward(),go();window.history.xx

location对象 获取或设置窗体的URL，并且可以用于解析 window.location.xx
属性： hash,host,hostname,href,pathname,port,protocol,search
方法：assign(),reload(),replace()

Navigator对象 浏览器有关信息，常用于检测浏览器与操作系统的版本 navigator.xx
属性：appCodeName,appName,appVersion,platform,userAgent

screen对象 用于获取用户的屏幕信息 window.screen.xx
属性：avaiHeight availWidth,colorDepth,pixelDepth,height,width

五、DOM （Document Object Model 文档对象模型）
document.getElementsByName(); 获取名字相同的集合元素节点
document.getElementsByTagName(); 获取标签名相同的集合元素节点
elementNode.getAttribute(name); 通过元素节点的属性名称获取属性的值
elementNode.setAttribute(name,value);
DOM中，每个节点都是一个对象。DOM节点的三个重要属性：
nodeName:节点的名称
nodeValue:节点的值
nodeType:节点的类型

