---
title: 00-黑马pink前端HTML5&CSS3入门教程观看笔记
---

> [黑马程序员pink老师前端入门教程，零基础必看的h5(html5)+css3+移动端前端视频教程](https://www.bilibili.com/video/BV14J4114768/?share_source=copy_web&vd_source=baf8348521aa1eac9683e0e70620876c)

## P01 前言
---
老师的自我介绍...

## P02 基础班学习路线
---

主要学习PC端网站布局

最终网站: 品优购静态网站

目的: 精通网页布局

![](https://blog.oss.yeetu.com/231006/01.png)

## P03 HTML 简介导读
---
无知识点

## P04 网页的相关概念
---

### 什么是网页?
网页是构成网站的基本元素, 它通常由图片、链接、文字、声音、视频等元素组成.通常我们看到的网页,常以.html或.html后缀结尾的文件, 因此将其俗称为 HTML 文件.


### 什么是HTML?
HTML 指的是超文本标记语言(Hyper Text Markup Language), 它是用来描述网页的一种语言. HTML 不是一种编程语言, 它是一种标记语言.

## P05 常见浏览器以及内核
---

浏览器是网页显示、运行的平台.常见的浏览器有IE、火狐(Firefox)、谷歌(Chrome)、 Safari和Opera等

|浏览器 | 内核|
|:-------------:|:-------------:|
| chrome | Blink(webkit的升级版本)  |
| 欧鹏  | Blink(webkit的升级版本)  |
|360安全浏览器| Blink(webkit的升级版本)|
|360极速浏览器| Blink(webkit的升级版本)|
|Safari|Webkit|
|Firefox 火狐|Gecko|
|IE| Trident |

## P06 WEB标准
---

web标准是由w3c组织和其他标准化组织制定的一系列标准的集合, w3c(万维网联盟)是国际最著名的标准化组织.

**web标准的构成**

主要包括结构(Structure)、 表现(Presentation)、行为(Behavior)三个方面

|标准 | 说明|
|:-------------:|:-------------:|
| 结构 | 结构用于对网页元素进行整理和分类,现阶段主要学习的是HTML  |
| 表现 | 表现用于设置网页元素的版式、颜色、大小等外观样式, 主要指CSS |
| 行为 | 行为是指网页模型的定义及交互的编写, 现阶段主要学习的是Javascript |

## P07 HTML 标签导读
---
无知识点

## P08 HTML 语法规范
---
标签符号 `<>`, 一般是双标签`<html></html>`, 也有单标签`<br />`, 标签有包含关系和并列关系

```html
<html>
  <head></head>
  <body></body>

  <!-- html 包含 head, head和body是并列关系 -->
</html>
```

## P09 HTML基本结构标签
---

```html
<html>
  <head>
    <title>第一个页面</title>
    <body>
      这里是页面的主主体部分
    </body>
  </head>
</html>
```

## P10 VSCODE工具创建页面
---
按`!` 再按`tab`键, 可以创建基础的html骨架结构

## P11 VSCODE插件安装以及快捷键
---
见 01-初阶-研发工具 内的文章

## P12 DOCTYPE和lang以及字符集的作用
---

`<!DOCTYPE html>` 文档类型的声明标签, 作用是告诉浏览器使用哪个HTML版本来显示网页.
`<html lang="zh-CN">` 定位网页的语言类型, 对于浏览器和搜索引擎有一定的作用
`<meta charset="UTF-8">` 规定html文档应该使用的编码方式

## P13 标签语义
---
就是标签的含义, 即这个标签是用来干嘛的,根据标签的语义, 在合适的地方给一个最为合理的标签,可以让页面结构更清晰

## P14 标题标签
---

`<h1> <h2> <h3> <h4> <h5> <h6>` 作为标题使用

加了标题标签后:

- 文字会加粗
- 成为一段 

## P15 段落标签和换行标签
---

`<p></p>` 段落标签

`<br />` 换行标签

## P16 体新闻案例
---

`h1 + h6 + p + p + h6 + p + p + <br />`

## P17 文本格式化标签
---
标签语义: 突出重要性 比普通文字更重要

- `<strong></strong>` 加粗
- `<em></em>` 倾斜
- `<del></del>` 删除线
- `<ins></ins>` 下划线

## P18 div和span标签
---
这两个标签是没有语义的,它们是一个盒子, 是用来装内容的
`<div>`: 独占一行
`<span>`: 一行可以放多个

## P19-21 图像标签
---
`<img src="图像url" />` 

| 属性 | 属性值 | 说明 |
|:---- |:----- |:----|
| src | 图片路径 | 必须属性 |
| alt | 文本 | 替换文本,图像不能显示的文字 |
| title | 文本 | 鼠标放到图像上, 显示的文字 |
| width | 像素 | 设置图像的宽度 |
| height | 像素 | 设置图像的高度 |
| border | 像素 | 设置图像的边框粗细 - <em>弃用</em> |

## P22 目录文件夹和根目录
---

- 目录文件夹: 普通的文件夹,网页相关的素材,都放这里
- 根目录: 打开目录文件夹的第一层就是根目录

## P23-25 相对路径和绝对路径
---
- 相对路径: 以引用文件所在的位置为参考基础, 而建立出的目录路径.
- 绝对路径: 目录下的绝对位置, 通常从盘符开始的路径 

## P26-28 链接标签
---
`<a href="跳转目标" target="目标窗口的弹出方式"> 文本或图像 </a>`

| 属性 | 作用 |
|:---- |:----- |
| href | 跳转的目标, 必填 | 
| target | _self 或 _blank |

## P29 注释标签和特殊字符
---
`<!-- -->` 注释

[特殊字符](https://www.w3cschool.cn/html/html-css-entities.html)

## P33-39 表格标签
---
表格是用来展示数据的

```html
<table>
  <thead>
    <tr>
      <th>表头的单元格</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>单元格内的文字</td>
    </tr>
  </tbody>
</table>
```

表格有相关的属性, 但是通常用css来写

**合并单元格**
- 跨行合并: `rowspan = "合并单元格的个数"`
- 跨列合并: `colspan = "合并单元格的个数"`

```html
<table width="500" height="250" border="1" cellspacing="0">
  <tr>
    <td></td>
    <td colspan="2"></td>
  </tr>
  <tr>
    <td rowspan="2"></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td></td>
  </tr>
</table>
```

## P40-43 列表标签
---

表格是用来显示数据的, 那么列表就是用来布局的

列表最大的特点就是整齐、整洁、有序, 它作为布局会更加的自由和方便

- 无序列表 

```html
  <ul>
    <div><li>榴莲</li></div>
    <li>臭豆腐</li>
    <li>苹果</li>
  </ul>
```

- 有序列表

```html
  <ol>
    <li>刘 1000</li>
    <li>李 100</li>
    <li>皮 1</li>
  </ol>
```

- 自定义列表

```html
  <dl>
    <dt>标题一</dt>
    <dd>解释1</dd>
    <dd>解释2</dd>
  </dl>
```

## P44-55 表单相关的标签
---
表单是用于收集用户信息的

- 表单域
包含表单元素的区域, 在HTML中, `<form>`标签用于定义表单域, 以实现用户信息的收集和传递,表单域会把表单元素的信息送给后台

- 表单控件(表单元素)
在表单域中可以定义各种表单元素, 这些表单元素就是允许用户在表单中输入或者选择的内容控件

- input type="属性值"

| input属性值| 属性值 | 描述
|:--- |:--- |:----|
| name | 用户自定义 | 定义input元素的名称 |
| value | 用户自定义 | 规定input元素的值 |
| checked | checked | 规定此input元素首次加载的时候被选中 |
| maxlength | 正整数 | 规定输入字段中的字符的最大长度 |

name 和 value 是每个表单元素都有的属性值, 主要给后台人员使用

name 表单元素的名字, 要求单选按钮和复选框要有相同的name值

| type属性值| 描述|
|:--- |:--- |
| button | 定义可点击按钮(多数情况下,用于通过js启动脚本)|
| checkbox | 复选框|
| file |  定义输入字段和浏览按钮, 供文件上传 |
| hidden |  定义隐藏的输入字段 |
| image |  定义图像形式的提交按钮 |
| password |  定义密码字段,该字段中的字符被掩码 |
| radio |  定义单选按钮 |
| reset |  定义重制按钮 |
| submit |  定义提交按钮 |
| text |  定义单行的输入字段,默认20字符 |

- `<label>` 标签

`<label>`标签为input元素定义标注, 用于绑定一个表单元素, 当点击`<label>`标签内的文本时, 浏览器会自动将焦点转到对应的表单元素上

- select 下拉列表
- textarea 文本域

```html

<form action="demo.php" method="POST" name="firstForm">
  用户名: <input type="text" name="username" value="" maxlength="10" placeholder="请输入用户名"> <br />
  密码: <input type="password" name="pwd" value="" placeholder="请输入密码"> <br />

  性别: <input type="radio" name="sex" value="男" checked="checked" id="myForm_sex_male">
  <label for="myForm_sex_male">男</label>

  <input type="radio" name="sex" value="女" id="myForm_sex_female">
  <label for="myForm_sex_female">女</label> <br />

  爱好: <input type="checkbox" name="hobby" value="吃饭" checked="checked" id="myForm_hobby_eat">
  <label for="myForm_hobby_eat">吃饭</label>

  <input type="checkbox" name="hobby" value="睡觉" id="myForm_hobby_sleep">
  <label for="myForm_hobby_sleep">睡觉</label> <br />

  <input type="button" value="获取短信验证码"> <br />

  上传头像: <input type="file" value="获取短信验证码"> <br />

  <select name="city" id="myForm_city">
    <option value="山东" selected="selected">山东</option>
    <option value="浙江">浙江</option>
    <option value="上海">上海</option>
  </select>

  <br />

  <textarea name="" id=""></textarea>

  <input type="submit" value="免费注册">
  <input type="reset" value="重置">
</form>

```

## P56-59 综合案例-注册页面
---

## P60 学会查阅文档
---

## P61-71 CSS 选择器

标签选择器、类选择器、ID选择器、通配符选择器

```css

/* 标签选择器 */
p {
  color: red;
}

/* 类选择器 */
.class-name {
  font-size: 12px;
}

/* ID选择器 */
#id-name {
  width: 200px;
}

/* 通配符选择器 */
* {
  color: green;
}
```

## P72-77 字体属性

```css

font-family: '微软雅黑';
font-size: 12px;
font-weight: 400;
font-style: italic;

```

## P78-83 CSS文本属性

```css
color: #ff5555;
color: rgb(255, 0, 0);
text-align: center; /*left, right, center */
text-decoration: none;  /* none, underline, overline, line-through */
text-indent: 10px;  /* 10px, 2em */
line-height: 22px;  /* 22px, 1.5em */
```

## P84-87 CSS引入样式
- 内部样式表
- 行内样式表
- 外部样式表

## P94-95 Emmet语法

1. 快速生成html结构语法
2. 快速生成css样式语法

## P97-105 复合选择器

- 后代选择器
- 子选择器
- 并集选择器
- 伪类选择器

```css
/* 后代 */
ol li {
  
}

/* 子选择器 */
ul > li {

}

/* 并集选择器: 选择多组标签, 同时为它们定义样式 */
div, p, .pig li {

}

/* 伪类选择器: 最大的特点使用:表示 */

a:link {
  color: #333;
}

a:hover {
  color: blue;
}

input:focus {
  background-color: skyblue;
}


```
## P106- 元素的显示模式

作用:网页的标签很多, 在不同的地方用到不同类型的标签,了解它们可以更好的网页布局.

元素显示模式就是标签以什么方式进行显示,比如`<div>`自占一行,一行可以放多个`<span>`

HTML 元素一般分为块元素和行内元素

常见的块元素
```html
h1 ~ h6, p, div, ul, ol, li
```

常见的行内元素,也叫内联元素
```html
a,strong,b,em,i,del,s,ins,u,span

```
行内块元素
```html
img, input, td 同时具有块元素和行内元素的特点
```
