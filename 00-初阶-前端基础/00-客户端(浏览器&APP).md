---
title: 00-客户端(浏览器&APP)
---
> 记录日期: 2023-09-19

阿里巴巴知识图谱如下:
![](https://blog.oss.yeetu.com/230919/00-00-01.png)

这里的客户端是其实就是网页运行的平台,我们用`HTML&CSS&JS`编写出来的代码,需要一种工具去解释执行它,从而变成我们能看见的网页.上图的Chrome、Safari、小程序或WebView其实就是解释执行`HTML&CSS&JS`的工具. 

## 常见的浏览器
常见的浏览器有谷歌（Chrome）、Safari、火狐（Firefox）、IE、Edge、Opera等。如下图所示：

![](https://blog.oss.yeetu.com/230919/00-00-02.png)
上图中:
- Chrome(最常用)、Firefox(常用)、Safari(苹果系统自带),这三个浏览器相对是标准浏览器.
- IE(非标准浏览器,不太符合W3C的标准)
- 微信(里面有小程序)

## 浏览器的组成
浏览器分成两部分：
- 渲染引擎(即: 浏览器内核)
- JS 引擎

### 渲染引擎(浏览器内核)
浏览器所采用的「渲染引擎」也称之为「浏览器内核」，用来解析 HTML与CSS。渲染引擎决定了浏览器如何显示网页的内容以及页面的格式信息。_渲染引擎是浏览器兼容性问题出现的根本原因_

渲染引擎的英文叫做 Rendering Engine。通俗来说，它的作用就是：读取网页内容，计算网页的显示方式并显示在页面上。

常见浏览器的内核如下：

|浏览器 | 内核|
|:-------------:|:-------------:|
| chrome | Blink(webkit的升级版本)  |
| 欧鹏  | Blink(webkit的升级版本)  |
|360安全浏览器| Blink(webkit的升级版本)|
|360极速浏览器| Blink(webkit的升级版本)|
|Safari|Webkit|
|Firefox 火狐|Gecko|
|IE| Trident |

备注：360的浏览器，以前使用的IE浏览器的Trident内核，但是现在极速模式已经改为使用 chrome 浏览器的 Blink内核。如果浏览政府网页,可以更换成兼容模式(Trident内核)

### 2、JS 引擎

也称为 JS 解释器。 用来解析网页中的JavaScript代码，对其处理后再运行。

浏览器本身并不会执行JS代码，而是通过内置 JavaScript 引擎(解释器) 来执行 JS 代码 。JS 引擎执行代码时会逐行解释每一句源码（转换为机器语言），然后由计算机去执行。所以 JavaScript 语言归为脚本语言，会逐行解释执行。

常见浏览器的 JS 引擎如下：

|浏览器 | JS 引擎|
|:-------------:|:-------------|
|chrome / 欧鹏   | V8   |
|Safari|Nitro|
|Firefox 火狐|SpiderMonkey（1.0-3.0）/ TraceMonkey（3.5-3.6）/ JaegerMonkey（4.0-）|
|Opera|Linear A（4.0-6.1）/ Linear B（7.0-9.2）/ Futhark（9.5-10.2）/ Carakan（10.5-）|
|IE|Trident |


## 浏览器工作原理

浏览器主要由下面这个七个部分组成：

![](https://blog.oss.yeetu.com/230919/00-00-03.png)

1、User Interface（UI界面）：包括地址栏、前进/后退按钮、书签菜单等。也就是浏览器主窗口之外的其他部分。

2、Browser engine （浏览器引擎）：用来查询和操作渲染引擎。是UI界面和渲染引擎之间的**桥梁**。

3、Rendering engine（渲染引擎）：用于解析HTML和CSS，并将解析后的内容显示在浏览器上。

4、Networking （网络模块）：用于发送网络请求。

5、JavaScript Interpreter（JavaScript解析器）：用于解析和执行 JavaScript 代码。

6、UI Backend（UI后端）：用于绘制组合框、弹窗等窗口小组件。它会调用操作系统的UI方法。

7、Data Persistence（数据存储模块）：比如数据存储  cookie、HTML5中的localStorage、sessionStorage。

## 必读重要文章：

- 英文版：[How Browsers Work: Behind the scenes of modern web browsers](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/)
---