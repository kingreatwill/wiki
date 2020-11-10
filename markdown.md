---
title: Markdown 教程
description: Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档。  Markdown 语言在 2004 由约翰·格鲁伯（英语：John Gruber）创建。  Markdown 编写的文档可以导出 HTML 、Word、图像、PDF、Epub 等多种格式的文档。
published: true
date: 2020-11-10T03:22:38.955Z
tags: 
editor: undefined
dateCreated: 2020-11-09T07:29:26.876Z
---

# Markdown
## Markdown demo
### 标题
- 使用 = 和 - 标记一级和二级标题
```
我展示的是一级标题
=================

我展示的是二级标题
-----------------
```
- 使用 # 号标记
使用 # 号可表示 1-6 级标题，一级标题对应一个 # 号，二级标题对应两个 # 号，以此类推。

### 段落
段落的换行是使用两个以上空格加上回车。
当然也可以在段落后面使用一个空行来表示重新开始一个段落。

### 字体
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```
*斜体文本*
_斜体文本_
**粗体文本**
__粗体文本__
***粗斜体文本***
___粗斜体文本___
```

### 分隔线
你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线：
***

* * *

*****

- - -

----------
```
***

* * *

*****

- - -

----------
```

### 删除线
~~wcoder.com~~
`~~wcoder.com~~`

### 下划线
Markdown 并无下划线的原生语法，因为会和链接的默认样式产生混淆。但是可以使用html标签实现
<u>带下划线文本</u>
`<u>带下划线文本</u>`

### 脚注
Markdown 脚注的格式:`[^要注明的文本]`

wcoder [^1]。

[^1]: `wcoder.com` -- a coder in the world!

```
wcoder [^1]。

[^1]: `wcoder.com` -- a coder in the world!
```

### 列表
- 无序列表使用星号(*)、加号(+)或是减号(-)作为列表标记，这些标记后面要添加一个空格，然后再填写内容
- 有序列表使用数字并加上 . 号来表示

#### 列表嵌套
列表嵌套只需在子列表中的选项前面添加四个空格即可：
1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
```
1. 第一项：
    - 第一项嵌套的第一个元素
    - 第一项嵌套的第二个元素
2. 第二项：
    - 第二项嵌套的第一个元素
    - 第二项嵌套的第二个元素
```

### 区块
Markdown 区块引用是在段落开头使用 > 符号 ，然后后面紧跟一个空格符号
另外区块是可以嵌套的，一个 > 符号是最外层，两个 > 符号是第一层嵌套，以此类推
```
> 最外层
> > 第一层嵌套
> > > 第二层嵌套
```
> 最外层
> > 第一层嵌套
> > > 第二层嵌套

### 代码
```
1. `printf()` 函数
2. 代码区块使用 4 个空格或者一个制表符（Tab 键）。
3. 用 ``` 包裹一段代码，并指定一种语言（也可以不指定）
```
`printf()` 函数
```javascript
$(document).ready(function () {
    alert(''wcoder.com'');
});
```

### 链接
```
[链接名称](链接地址)

或者

<链接地址>
```
#### 高级链接
我们可以通过变量来设置一个链接，变量赋值在文档末尾进行：
```
这个链接用 1 作为网址变量 [Google][1]
这个链接用 wcoder 作为网址变量 [wcoder][wcoder]
然后在文档的结尾(也不一定要在结尾，统一在结尾是一个良好的习惯)为变量赋值（网址）

  [1]: http://www.google.com/
  [wcoder]: http://www.wcoder.com/
```
这个链接用 1 作为网址变量 [Google][1]
这个链接用 wcoder 作为网址变量 [wcoder][wcoder]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [wcoder]: http://www.wcoder.com/
  
### 图片
Markdown 图片语法格式如下：
```
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")

```

### 表格
```
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
```
#### 对齐方式
- -: 设置内容和标题栏居右对齐。
- :- 设置内容和标题栏居左对齐。
- :-: 设置内容和标题栏居中对齐。
```
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
```

### 转义
Markdown 使用反斜杠转义特殊字符：
```
**文本加粗** 
\*\* 正常显示星号 \*\*
```


Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：
```
\   反斜线
`   反引号
*   星号
_   下划线
{}  花括号
[]  方括号
()  小括号
#   井字号
+   加号
-   减号
.   英文句点
!   感叹号
```
### 注释
#### html注释
```
<!--哈哈我是注释，不会在浏览器中显示。-->
```
#### hack方法
hack方法就是利用markdown的解析原理来实现注释的。

[comment]: <> (哈哈我是注释，不会在浏览器中显示。)
[//]: <> (哈哈我是注释，不会在浏览器中显示。)
[//]: # (其中，这种方法最稳定，适用性最强)
[^_^]: # (这种方法最可爱，超级无敌萌啊)

### 上标/下标 Subscript/Superscript
```
X<sub>i</sub>
H<sub>2</sub>O  CO<sub>2</sub>
益达<sup>TM</sup>

输入上标 x^2^
输入下标 x~0~
```
X<sub>i</sub>
H<sub>2</sub>O  CO<sub>2</sub>
益达<sup>TM</sup>

输入上标 x^2^
输入下标 x~0~

## 第三方
- [wiki.js](https://docs.requarks.io/en/rendering)的请查看文档支持

### TOC 目录
在文档最上方添加
```
[TOC]
```
### 任务列表 Task List
- [x] 任务1，已完成;
- [x] 任务2，已完成;
- [ ] 任务3，未完成; 

### 扩展选项卡 Expand Tabs
- pymdownx.tabbed
```
=== "Tab 1"
    Markdown **content**.

    Multiple paragraphs.

=== "Tab 2"
    More Markdown **content**.

    - list item a
    - list item b
```
    
- wiki.js
```
### Tabset {.tabset}
#### Tab 1
Markdown **content**.  
Multiple paragraphs.

#### Tab 2
More Markdown **content**.
- list item a
- list item b
```

### Tabset {.tabset}
#### Tab 1
Markdown **content**.  
Multiple paragraphs.

#### Tab 2
More Markdown **content**.
- list item a
- list item b


### 备注
*[HTML]: Hyper Text Markup Language
*[W3C]:  World Wide Web Consortium
The HTML specification
is maintained by the W3C.
> 其实就是转换成`<abbr>`html标签

> warning.{.is-warning}

> success.{.is-success}

> info.{.is-info}

> danger.{.is-danger}



### Emoji
:apple:

### 公式
- mathjax
- KaTeX
- Latex

```
$$
e^{x^2}\neq{e^x}^2
$$

$$H(D_2) = -(\frac{2}{4}\ log_2 \frac{2}{4} + \frac{2}{4}\ log_2 \frac{2}{4}) = 1$$
```

$$
e^{x^2}\neq{e^x}^2
$$

$$H(D_2) = -(\frac{2}{4}\ log_2 \frac{2}{4} + \frac{2}{4}\ log_2 \frac{2}{4}) = 1$$

### 流程图、时序图(顺序图)、甘特图
- [mermaid](http://mermaid-js.github.io/mermaid/)
- [flowchat](http://flowchart.js.org/)
- [Sequence](https://bramp.github.io/js-sequence-diagrams/)
- [PlantUML](https://plantuml.com/zh/)

#### 流程图 Flowchart
- 横向流程图
```mermaid
graph LR
A[方形] -->B(圆角)
    B --> C{条件a}
    C -->|a=1| D[结果1]
    C -->|a=2| E[结果2]
    F[横向流程图]
```

- 竖向流程图

```mermaid
graph TD
A[方形] --> B(圆角)
    B --> C{条件a}
    C --> |a=1| D[结果1]
    C --> |a=2| E[结果2]
    F[竖向流程图]
```
- 标准流程图

```mermaid
graph TD
    A[Start] --> B{Is it?};
    B -->|Yes| C[OK];
    C --> D[Rethink];
    D --> B;
    B ---->|No| E[End];
```
#### 时序图(顺序图) Sequence 

- UML标准时序图

```mermaid
%% 时序图例子,-> 直线，-->虚线，->>实线箭头
  sequenceDiagram
    participant 张三
    participant 李四
    张三->王五: 王五你好吗？
    loop 健康检查
        王五->王五: 与疾病战斗
    end
    Note right of 王五: 合理 食物 <br/>看医生...
    李四-->>张三: 很好!
    王五->李四: 你怎么样?
    李四-->王五: 很好!
```
- 时序图
```mermaid
sequenceDiagram
    Alice->>Bob: Hello Bob, how are you?
    alt is sick
        Bob->>Alice: Not so good :(
    else is well
        Bob->>Alice: Feeling fresh like a daisy
    end
    opt Extra response
        Bob->>Alice: Thanks for asking
    end
```
#### 类图 Class diagram
```mermaid
 classDiagram
      Animal <|-- Duck
      Animal <|-- Fish
      Animal <|-- Zebra
      Animal : +int age
      Animal : +String gender
      Animal: +isMammal()
      Animal: +mate()
      class Duck{
          +String beakColor
          +swim()
          +quack()
      }
      class Fish{
          -int sizeInFeet
          -canEat()
      }
      class Zebra{
          +bool is_wild
          +run()
      }
```

#### 状态图 State diagram
```mermaid
stateDiagram-v2
    [*] --> Still
    Still --> [*]

    Still --> Moving
    Moving --> Still
    Moving --> Crash
    Crash --> [*]
```
#### 实体关系图 Entity Relationship Diagram(ER model)
```mermaid
erDiagram
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ LINE-ITEM : contains
    CUSTOMER }|..|{ DELIVERY-ADDRESS : uses
```
#### User Journey Diagram
```mermaid
journey
    title My working day
    section Go to work
      Make tea: 5: Me
      Go upstairs: 3: Me
      Do work: 1: Me, Cat
    section Go home
      Go downstairs: 5: Me
      Sit down: 5: Me
```

#### 甘特图 gantt

```mermaid
gantt
    title A Gantt Diagram
    dateFormat  YYYY-MM-DD
    section Section
    A task           :a1, 2014-01-01, 30d
    Another task     :after a1  , 20d
    section Another
    Task in sec      :2014-01-12  , 12d
    another task      : 24d
```

#### Pie chart diagram

```mermaid
pie title Pets adopted by volunteers
    "Dogs" : 386
    "Cats" : 85
    "Rats" : 15
```