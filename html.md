## html

html: Hyper Text markup language 超文本标记语言

## 标记/标签

### 行标签

- 不会独占一行

- 不能设置宽高

- a(href  title target{链接位置})    链接        span

  ​    i 、em 斜体  b、 strong 粗体   time 时间  address  地址    progress  进度

### 块标签

* 独占一行

* div   h1~h6 标题   p段落    pre    ul 无序列表   li列表内行的样式     ol 有序列表   dl定义列表    dt定义列表中的项目    dd 描述列表中的项目   header 文档的页眉（介绍信息）     footer 文档或节的页脚    section 文档中的节    

  main 规定文档的主要内容    video 定义视频，比如电影片段或其他视频流    audio 定义声音，比如音乐或其他音频流   form 表单

  > * pre 元素可定义预格式化的文本。被包围在 pre 元素中的文本通常会保留空格和换行符。而文本也会呈现为等宽字体。
  >
  >   ​<pre> 标签的一个常见应用就是用来表示计算机的源代码。
  >
  >   ​	可以导致段落断开的标签（例如标题、[](http://www.w3school.com.cn/tags/tag_p.asp) 和 [ 标签](http://www.w3school.com.cn/tags/tag_address.asp)）*绝不能*包含在 <pre> 
  >
  >   ​	所定义的	块里。尽管有些浏览器会把段落结束标签解释为简单地换行，但是这种行为在所有浏览器上并不都是一样的。
  >
  >    	pre 元素中允许的文本可以包括[物理样式和基于内容的样式变化](http://www.w3school.com.cn/html/html_style.asp)，还有[链接](http://www.w3school.com.cn/tags/tag_a.asp)、[图像](http://www.w3school.com.cn/tags/tag_img.asp)和[水平分隔线](http://www.w3school.com.cn/tags/tag_hr.asp)。当把其他标签（比如 <a> 标
  >
  >   ​	签）放到	 <pre> 块中时，就像放在 HTML/XHTML 文档的其他部分中一样即可。
  >
  > * main  在一个文档中，不能出现一个以上的 <main> 元素。<main> 元素不能是以下元素的
  >
  >   ​	后代：<article>、<aside>、<footer>、<header> 或 <nav>。

### 行内块级标签

- 不会独占一行   也可以设置宽高

- img(src alt  width height border) 图片

  input 用于搜集用户信息。根据不同的 type 属性值，输入字段拥有很多种形式。 

  textarea 多行的文本输入控件

  select 可创建单选或多选菜单

  option   <select&> 元素中的<option >  标签用于定义列表中的可用选项。

  fieldset 可将表单内的相关元素分组。<fieldset> 标签将表单内容的一部分打包，生成一组相关表单的字段。<fieldset> 标签没有

  ​		必需的或唯一的属性

## 实体

###### &nbsp;&nbsp;  空格         &lt ;   <         &gt ;   >        &quot ;    "        &amp ;     &

## 表单（用来提交）

form( action method)

表单控件   

- 类型（文本text    密码password    单选框radio   多选框checkbox    

- 隐藏域hidden   提交submit   重置密码reset   按钮button）

  ​	h5新增:(邮件email  包含*URL* 地址的输入域 url  选取日、月、年date  选取周和年week   选取月、年month  

  ​	选取时间（小时和分钟）time      选取时间、日、月、年（UTC 时间）datetime

  ​	设置完整时间YYYY-MM-DDTHH:mm:ss (选取时间、日、月、年（本地时间）)    datetimea-local     数值的输入域 number 

  ​	 包含一定范围内数字值的输入域range

  ​	 用于搜索域search   颜色color)

  | button   | 定义可点击按钮（多数情况下，用于通过 JavaScript 启动脚本）。 |
  | -------- | ------------------------------------ |
  | checkbox | 定义复选框。                               |
  | file     | 定义输入字段和 "浏览"按钮，供文件上传。                |
  | hidden   | 定义隐藏的输入字段。                           |
  | image    | 定义图像形式的提交按钮。                         |
  | password | 定义密码字段。该字段中的字符被掩码。                   |
  | radio    | 定义单选按钮。                              |
  | reset    | 定义重置按钮。重置按钮会清除表单中的所有数据。              |
  | submit   | 定义提交按钮。提交按钮会把表单数据发送到服务器。             |
  | text     | 定义单行的输入字段，用户可在其中输入文本。默认宽度为 20 个字符。   |

- 属性（ 规定 input 元素的类型type      名称name        输入字段的初始值value       输入字段为只读（不能修改）readonly      

  禁用disable     规定在页面加载时应该被预先选定的 input 元素checked    选定selected）

  ​	h5新增:(require{验证}      提示placeholder)

- *disabled* 属性规定输入字段是禁用的。被禁用的元素是不可用和不可点击的被禁用的元素不会被提交。

- selected规定在页面加载时预先选定该选项。被预选的选项会显示在下拉列表最前面的位置。也可以在页面加载后通过 JavaScript 设置 selected 属性。

## css

## 引用方式

- 行内样式 style="width=100px;height=100px;";
- 嵌入样式<style>.one{width:100px;}</style>
- 外部样式<link rel='stylesheet' href="">
- 引入样式@import url(“demo.css”);  @import "demo.css";

## 选择器

- 标签选择器 div body a 

- 类名选择器   .one

- id选择器   #one

- 后代选择器 ul  li      .one .two

- 群组选择器   .one,.two

- 交叉选择器    ul.one      .one.two

- UI伪类选择器  :link    :hover    :active     :visited 

- 子选择器    div>a      .one>.two

- 同级选择器   div+p   div~p  

- :nth-child()  :first-child   :last-child  :nth-last-child() :only-child          选择器匹配属于其父元素的第 N 个子元素，不论元素的类型。    

- :nth-of-type()  :first-of-type  :last-of-type    :nth-last-of-type()    :only-of-type

  ​                                				选择器匹配属于父元素的特定类型的第 N 个子元素的每个元素.

- 属性选择器  [ data ]  ,[ data=a ]  , [data^=aa]  ,[data$=aa   ]  ,[data*=aa]

- :before    :after                                        选择器在被选元素的内容前、后面插入内容

- :checked                                                   选择器匹配每个选中的输入元素（仅适用于单选按钮或复选框）

- :target 用于选取当前活动的目标元素           :  root  选择器匹配文档根元素。

## 属性

### 布局

宽width  高height  外边距margin   内边距padding  浮动float   定位position  

允许您以特定的方式定义匹配某个区域的特定元素 box-sizing (大部分移动端) 

设置元素如何显示 display   左left  右right  上top 下bottom  设置元素的堆叠顺序z-index

### 样式

- 背景background   背景图 background-image   背景颜色background-color 

  是否及如何重复背景图像。默认地，背景图像在水平和垂直方向上重复。 background-repeat 

​      设置背景图像是否固定或者随着页面的其余部分滚动background-attachment 

​      边框border  边框的宽度border-width  边框样式border-style  边框颜色border-color  背景的绘制区域border-clip 

​      背景的裁剪区域border-origin  边框大小border-size  添加圆角矩形、边框的属性最多8个值 border-radius  阴影 box-shadow

​     outline(轮廓线   与border不同的是在盒子外边且不占大小，不会根据内容的变化而变化) outline-offset（轮廓线偏移）

​    “描边”可叠加 box-shadow :0 0 0 2px #333,0 0 0 3px #ccc,......;     background:radial/-gradient(circle,red 0,blue 100%;transparent 0);

### 渐变

线性渐变linear-gradient()   重复的线性渐变repeating-linear-gradient()    

径向渐变radial-gradient()      重复的径向渐变repeating-radial-gradient()

### 文字

元素的字体系列font-family    文字大小font-size  颜色color  字体粗细font-weight    字体样式font-style  文本修饰 text-decoration

水平居中 text-align  首行缩进text-indent  垂直居中line-hight   自动换行word-break  字母间距letter-spacing   垂直对齐vertical-align

### 动画

transition  过渡效果transition-property  持续时间 transition-duration  

切换效果的速度transition-timing-function  延迟 transition-delay

@keyframe     animation

### 转换

* transform  3d转换情况transform-origin   3D立体视图的可视效果perspective   
* 指定嵌套元素是怎样在三维空间中呈现transform-style   定义 3D 元素所基于的 X 轴和 Y 轴perspective-origin  
* 平移translate    x轴平移translateX  y轴平移translateY  z轴平移translateZ 3d轴平移translate3d()   
* 旋转rotate()  绕x轴旋转rotateX()  绕y轴旋转rotateY()  绕z轴旋转rotateZ()  3d轴旋转rotate3d()  
* 缩放scale()  x轴缩放scaleX()   y轴缩放scaleY() 
* 斜切skew()  x轴斜切skewX()  y轴斜切skewY() 
* 矩阵matrix()    