# HTML学习

**修改时间** : 2025.09.25

---

## 0.My First Website:

* `<!DOCTYPE html>`    声明文档类型
* `<html lang="zh-CN">` ...`<html>`  根元素,lang指明语言
* `<head>` ... `</head>`  放元元素,影响界面设定
* `<meta charset="UFT-8">`  表明用UTF-8编码打开
* `<meta name="viewport" content="width=device-width initial-scale=1">` 作移动端的画面大小适配.即宽度为设备显示器宽度，缩放比例为1。
* Contents利于SEO(搜索引擎优化 Search Engine Optimization)
* `<title>`.....`</title>`  标题,显示在浏览器标签页上
* `<body>` .....`</body>`  页面的可见内容区域
* `<h1>` ..... `</h1>`  一级标题
* `<p>` .... `</p>`  表示是一个段落
* `<a href="(website)" target="_blank">` ..... `</a>`  引入超链接,在空白页面打开对应网址
* **HTML的空白与缩进不影响渲染结果**
* `<!-- 这是注释,不会显现! -->`

---

## 1.基础标签及其使用:

### 常用简单标签

* `<h1>`~`<h6>`  1~6级标题
* `<p>`  插入段落
* `<br>` 强制换行
* `<hr>` 插入一条分割水平线
* `<a>`  用来跳转,插入超链接
* `<img>` 插入图片.  (src:图片路径,alt替换文本,width/height调整图片尺寸,一般写一个为佳)
* **html所有的标签内部写成键值对形式,右值均为字符串形式**

### 语义化标签

* `<div>` 通用容器，没有语义
* `<header>` 头部,放标签和导航栏
* `<footer>` 尾部,放版权,联系方式
* `<main>` 标识页面主要内容，一个页面只能有一个main标签
* `<nav>`  导航菜单,放一组链接
* `<section>` 表示某一个主题区块,页面的独立章节
* `<article>` 独立的文章或帖子
* `<aside>` 表示侧边栏内容

---

## 2.文本与列表

### 文本标签

* `<strong>`或者 `<b>`  加粗强调
* `<em>`或者 `<i>`   斜体强调
* `<span>`   行内容器，没有语义。容器作用
* `<blockquote>`  长引用，一整段文字的引用，浏览器会自动缩进
* `<q>`  短引用,默认加引号

### 列表标签

* `<ul>`  无序列表，内容前面加圆点
* `<ol>`  有序列表，内容前面加序号
* `<li>`  用来呈现列表元素
* `<dl>`  定义列表，用来解释术语
* `<dt>`  dl中被解释的词条
* `<dd>`  dl中的解释文字

### 常用修饰标签

* `<mark>` 高亮显示
* `<small>` 小号文字
* `<del>` 删除线
* `<ins>` 下划线
* `<sup>` 上标
* `<sub>` 下标

---

## 3.HTML标签的三大显示特性

### 块级元素(block)

* **结构类：** `<div><header><section><footer><article><nav><main>`
* **文本类：** `<h1>~<h6><p><blockquote>`
* **列表类：** `<ul><ol><li><dl><dt><dd>`
* **表格类：** `<table><tr>`

*这些块类标签独占一行，首尾自动换行，宽度默认撑满父容器*

---

### 行内元素(incline)

* **文本修饰：** `<span><strong><em><b><i><u>`
* **链接图片：** `<a><img>`
* **表单控件：** `<input><label><button>`

*这些行内标签在结束的时候不会换行*

---

### 行内块元素(incline-block)

* `<img><button><input>`

*这些元素行为是行内元素，但是本身可以设置宽高*

---

## 4.表格与表单

### 表格(table)

* `<table border="1">`  创建一个表格标签，边框厚度为1
* `<tr>` 表示一行
* `<th>` 表示表头元素
* `<td>` 表示普通元素

### 表单(form)

* `<form>` 表示表单容器
* `<label>` 用来表示绑定表示表单内的元素。与对应 `<label>`内的元素进行交互可以激活其中的元素
* **`<input>`** 输入框，接受用户输入。
* type类型有:**text**  **password**  **checkbox**  **radio** ,分别对应文本，密码，复选框，单选框
* name键值对就是你的input的类型，value键值对就是这个标签的具体值。也就是用户提交表单后，会补充清楚键值对name:value
* 因此选择题是需要给出value的，输入题是直接拿用户输入当作value.
* `<textarea>` 多行文本输入
* `<select>` 选择表单，搭配name； `<option>` 选项，搭配value
* `<button>` 按钮，搭配type就好。提交type:"submit",可以不贴标签

---

## 5.多媒体与链接

* `<a href=" " target="_blank">` 表示超链接，在空白页打开href指定的网页
* `<img src=" " alt=" " width/height=" ">`  用来展示图片 
* `<audio controls>``<source src=" "  type="audio/mpeg">` 展示音频，指定音频路径与类型
* `<video controls>``<source src=" "  type="video/mp4" >` 展示视频，指定视频路径与类型

## 6.补充

* `<a href="#section1">`  表示跳转到section标签为section1的bufen
* `<a href="tel:96110">`  表示点击拨打电话(移动端)
* `<a href="mailto:ubituous@gmail.com">`  表示点击时打开邮件客户端，预填收件人。
