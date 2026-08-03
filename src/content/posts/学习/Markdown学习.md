---
title: Markdown学习
published: 2026-08-03
category: 软件学习
sourceLink: "https://iamhefang.cn/tutorials/Markdown"
---
# Markdown

Markdown 是一种轻量级标记语言，创始人为约翰·格鲁伯。它允许人们使用易读易写的纯文本格式编写文档，然后转换成有效的 XHTML（或者 HTML）文档。这种语言吸收了很多在电子邮件中已有的纯文本标记的特性。1

由于 Markdown 的轻量化、易读易写特性，并且对于图片，图表、数学式都有支援，目前许多网站都广泛使用 Markdown 来撰写说明文件或是用于论坛上发表讯息。如何该网站、GitHub、Reddit、Stack Exchange、OpenStreetMap 、SourceForge、简书等，甚至还能被用来撰写电子书。

Markdown 如今已成为世界上最受欢迎的标记语言之一。
Mardown的优势
- 1.专注于文字内容；  
- 2.纯文本，易读易写，可以方便地纳入版本控制；  
- 3.语法简单，没有什么学习成本，能轻松在码字的同时做出美观大方的排版。  

Markdown 与 World 不同，Markdown 不像 World 是所见是所得的。如果需要把一段文本加粗，在 World 中，点击工具栏的加粗图标，内容就会被加粗。而在 Markdown 中我们可以使用在文本前后添加两个星号（\**粗体**，粗体）来达到同样的目的。

本站使用Visual Studio Code进行编写。


# 段落

## 1.1 常用语法

| Markdown       | HTML               | 预览                                                     |
| -------------- | ------------------ | -------------------------------------------------------- |
| `# 标题 1`     | `<h1>标题 1</h1>`  | <span style="font-size:36px;">**标题 1**</span> |
| `## 标题 2`    | `<h2>标题 2</h2>`  | <span style="font-size:30px;">**标题 2**</span> |
| `### 标题 3`   | `<h3>标题 3</h3>`  | <span style="font-size:24px;">**标题 3**</span> |
| `#### 标题 4`  | `<h4>标题 4</h4>`  | <span style="font-size:20px;">**标题 4**</span> |
| `##### 标题 5` | `<h5>标题 5</h5>`  | <span style="font-size:17px;">**标题 5**</span> |
| `###### 标题 6`| `<h6>标题 6</h6>`  | <span style="font-size:15px;">**标题 6**</span> |

## 1.2 可选语法

标题内容的后面如果也存在空格和 `#` ，也可以构成标题，且标题的级别以前面 `#` 的数量为准。

| Markdown            | HTML               | 预览                                                         |
| ------------------- | ------------------ | ------------------------------------------------------------ |
| `# 标题 1 #`     | `<h1>标题 1</h1>`  | <span style="font-size:36px;">**标题 1**</span> |
| `## 标题 2 ##`    | `<h2>标题 2</h2>`  | <span style="font-size:30px;">**标题 2**</span> |
| `### 标题 3 ###`   | `<h3>标题 3</h3>`  | <span style="font-size:24px;">**标题 3**</span> |
| `#### 标题 4 ####`  | `<h4>标题 4</h4>`  | <span style="font-size:20px;">**标题 4**</span> |
| `##### 标题 5 ######` | `<h5>标题 5</h5>`  | <span style="font-size:17px;">**标题 5**</span> |
| `###### 标题 6 ######`| `<h6>标题 6</h6>`  | <span style="font-size:15px;">**标题 6**</span> |

除了前面加 # 外，标题 1 和标题 2 也可以用下面加横线的形式。标题下面加等号 `=` 会生成标题 1，加减号 `-` 会生成标题 2。等号和减号的数量一般不限制，可以有一个或多个。

| Markdown      | HTML               | 预览                                                         |
| ------------- | ------------------ | ------------------------------------------------------------ |
| `标题 1` <br>` === ` | `<h1>标题 1</h1>` | <span style="font-size:36px;">**标题 1**</span> |
| `标题 2`<br>`---` | `<h2>标题 2</h2>` | <span style="font-size:30px;">**标题 2**</span> |

## 1.3 自定义标题 id

| Markdown                  | HTML                          | 预览                                                         |
| ------------------------- | ----------------------------- | ------------------------------------------------------------ |
| `# 标题 1 {#head1}`       | `<h1 id="head1">标题 1</h1>`  |  <span style="font-size:36px;">**标题 1**</span> |
| `## 标题 2 {#head2}`      | `<h2 id="head2">标题 2</h2>`  | <span style="font-size:30px;">**标题 2**</span> |
| `### 标题 3 {#head3}`     | `<h3 id="head3">标题 3</h3>`  | <span style="font-size:24px;">**标题 3**</span> |
| `#### 标题 4 {#head4}`    | `<h4 id="head4">标题 4</h4>`  | <span style="font-size:20px;">**标题 4**</span> |
| `##### 标题 5 {#head5}`   | `<h5 id="head5">标题 5</h5>`  | <span style="font-size:17px;">**标题 5**</span> |
| `###### 标题 6 {#head6}`  | `<h6 id="head6">标题 6</h6>`  | <span style="font-size:15px;">**标题 6**</span> |


<span style="font-size:24px;">**注意：**</span>

在有些Markdown解析器里面，`#` 和内容之间不加空格也可以识别为标题，但大部分解析器都是需要加空格的，为了兼容性更强我们一般在写标题时都加空格。