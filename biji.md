# HTML

HTML:     Hyper Text markup language  超文本标记语言

## 标签

### 行标签

* 不会独占一行
* 不能设置宽高
* a、（属性：herf链接地址,title标题,target目标的位置）    span/i/em/b/strong；time、  address、  progress

### 块标签

* 独占一行
* 可以设置宽高
* div块元素  、  
* h1~h6定义 HTML 标题、  
* p定义段落、 
* pre定义预格式文本、 
* ul定义无序列表、 
* li定义列表项、 
* ol定义有序列表、
* dl定义定义列表、
* dt定义定义项目、 
* dd定义定义的描述；
* header定义页面主体上的头部，
* header标签往往在一对body标签之中、 
* footer定义页面的底部（页脚）、
* section定义 用于表达书的一部分或一章，或者一章内的一节、 
* main、
* video视频标签：定义视频，比如电影片段或其他视频流、  
* audio音频标签：定义声音，比如音乐或其他音频流、  
* form 

### 行内块级标签

* 不会独占一行
* 可以设置宽高
* img图片(src地址 alt 说明 width宽 height高 border边框)、  
* input一个简单的 HTML 表单，包含两个文本输入框和一个提交按钮：
* textarea、标签定义多行的文本输入控件
* select、密码框
* option 元素定义下拉列表中的一个选项（一个条目）。
* fieldset 元素可将表单内的相关元素分组

## 实体

&nbsp 空格     &lt 小于号     &gt 大于号    &quot 引号    &amp 和号

## 表单

form(action提交地址，method提交方式)

表单控件

* 类型：input（text   password  radio   checkbox   file  hidden 规定元素的类型  submit提交   reset     button   ；email    url     date  week  month  time  datetime-local   number  range滑块展示效果   search   color）

  ```
  文本字段 text
  密码 password
  隐藏域 hidden
  文本区域 textarea
  复选框 checkbox
  单选按钮 radio
  选择列表 select
  图像域 image
  文件域 file
  按钮 button 
  提交按钮 submit
  ```

* 属性：type   name  value  readonly只读  disable   checked   selected   maxlength  ； required  placeholder  

  ```
  <form>表单常用属性有以下几种:
  name:用来标识这个表单,在javascript中可以通过 document.表单名 来取得这个表单
  action:表示这个表单提交时的跳转路径
  method:表示提交方式,可以选择post和get,默认为get方式.两种方式的区别:
      post:所有提交的参数都会隐藏,没有参数的大小限制,建议使用该方式
      get:所有提交参数都会在地址栏显示,参数总量最大4-5K.不建议使用
  enctype:表示表单的封装方式,只有在进行文件上传时才会使用,当执行文件上传时,必须将这个值设置为 enctype="multipart/form-data"
  onsubmit:当表单提交时自动执行的javascript事件,一般在需要进行提交验证时使用.

  表单中的常用控件:
  <input type="text">:文本框,输入单行文本
  <input type="password">:密码框,输入密码信息,所有输入的信息会隐藏显示
  <input type="button">:普通按钮,一般用来完成javascript功能的
  <input type="submit">:表单提交按钮,点此按钮提交表单
  <input type="reset">:表单重置按钮,点此按钮表单中的数据回到填写之前.
  <input type="radio">:单选按钮
  <input type="checkbox">:多选按钮
  <input type="hidden">:隐藏域,将一个值隐藏传递.
  <input type="image">:功能和submit提交按钮相同,但可以显示图片.
  <textarea></textare>:文本域,输入多行文本
  <select>:下拉列表,需要结合option一起使用
  <option>:通过该值为<select>设置选项 
  ```

# css

## 引用方式

* 行内样式  style="width:100px;height=100px;"
* 嵌入样式  <style>.one{wight:100px;}</style>
* 外部样式  <link rel='stylesheet' href="">
* 引入样式  @import url("demo.css");      @import "deom.css"

## 选择器

* 标签选择器     div{}    body{}   a{}  

* 类名选择器      .+类名{}

* ID选择器          #+名字{}

* 后代选择器       ul  li{}          .+类名 .+类名{}

* 群组选择器       .+类名,.+类名{}

* 交叉选择器      将两个标签合起来       ul.+类名   

* UI伪类选择器       :hover（鼠标经过）； :active(鼠标按下) ； :active()；:visited()

* 子选择器       表示选择前一个标签  div>a      .one>.two 

* 同级选择器       div+p紧挨着div     div~p要求不严格，前杠只要有盒子就好

* :nth-child(n)     规定属于其父元素的第n个子元素 

  e.g.规定属于其父元素的第二个子元素的每个 p 的背景色：

  p:nth-child(2)
  {
  background:#ff0000;
  }

   :first-child       选择属于其父元素的首个子元素

  e.g.选择属于其父元素的首个子元素的每个 <p> 元素，并为其设置样式：

  p:first-child
  { 
  background-color:yellow;
  }

  :last-child       指定属于其父元素的最后一个子元素

  e.g.指定属于其父元素的最后一个子元素的 p 元素的背景色：

  p:last-child
  { 
  background:#ff0000;
  }

  :nth-last-child()    规定属于其父元素的第n个子元素的每个 p 元素，从最后一个子元素开始计数

  e.g.规定属于其父元素的第二个子元素的每个 p 元素，从最后一个子元素开始计数：

  p:nth-last-child(2)
  {
  background:#ff0000;
  }

  :only-child     唯一的子元素,规定属于其父元素的唯一子元素

  e.g.规定属于其父元素的唯一子元素的每个 p 元素：

  p:only-child
  {
  background:#ff0000;
  }

* :nth-of-type  规定属于其父元素的第n个 p 元素的每个 p：

  e.g.规定属于其父元素的第二个 p 元素的每个 p：

  p:nth-of-type(2)
  {
  background:#ff0000;
  }

  :last-of-type    指定父元素的最后一个 p 元素

  e.g.指定父元素的最后一个 p 元素的背景色：

  p:last-of-type
  {
  background:#ff0000;
  }

  :nth-last-of-type()    规定属于其父元素的第n个 p 元素的每个 p，从最后一个子元素开始计数：

  e.g.规定属于其父元素的第二个 p 元素的每个 p，从最后一个子元素开始计数：

  ```
  p:nth-last-of-type(2)
  {
  background:#ff0000;
  }
  ```

  :only-of-type   指定属于父元素的特定类型的唯一子元素的每个 p 元素

  e.g.指定属于父元素的特定类型的唯一子元素的每个 p 元素：

  ```
  p:only-of-type
  {
  background:#ff0000;
  }
  ```

* 属性选择器     [date]


[date=aa]

[date^=aa]

[date$=aa]

[date*=aa]

* :before .在每个元素的内容之前插入新内容

  e.g.在每个 <p> 元素的内容之前插入新内容：

  ```
  p:before
  { 
  content:"台词：";
  }
  ```

  :after  在每个元素的内容之后插入新内容

  e.g.在每个 <p> 元素的内容之后插入新内容：

  ```
  p:after
  { 
  content:"台词：";
  }
  ```

* :checked

  e.g.为所有被选中的 input 元素设置背景色：

  ```
  input:checked
  { 
  background-color: #ff0000;
  }
  ```

* :target 

  e.g.突出显示活动的 HTML 锚：

  ```
  p:target
  { 
  border: 2px solid #D4D4D4;
  background-color: #e5eecc;
  ```

​         :root   选择当前文档的

e.g.设置 HTML 文档的背景色：

```
:root
{ 
background:#ff0000;
}
```

## 属性

### 布局

width  宽height 高 margin  padding   float   position(定位)  box-sizing(用来定义当前盒子宽高的计算方式   例如：border-box)    display(属性)  left  right  top  bottom  z-index

### 样式

集合属性：

background：background-image背景图片  background-color背景颜色  background-repeat规定如何重复背景图像  background-position 规定背景图像的位置 background-attachment 规定背景图像是否固定或者随着页面的其余部分滚动  

border:： border-width 边框宽 border-style边框 样式  border-color边框颜色  background-clip 背景裁剪 background-origin  background-size 背景图片大小 border-image  border-radius  可设8个值：10px/20px用斜杠隔开表示x/y轴的值  border-shadow阴影 （用逗号隔开设置多个阴影可以模拟多边框） 

outline(轮廓线)缺点，不会跟着盒子形状圆角改变，不像边框随和，但是不占位置，不用计算实际大小    outline-offset(轮廓线的偏移)，偏移后不占位置

### 渐变

liner-gradient() 线性渐变      repeating-liner-gradient()  重复渐变     radial-gradient()   径向渐变   repeating-radial-gradient() 重复径向渐变

### 文字

font-family       font-size      color      font-weight     font-style   text-decoration    text-align    text-indent   line-height   word-break   letter-spacing   vertical-align

### 动画的实现

transition    transition-property定义过渡属性    transition-duration持续的时间，一段时间，表示时间的长度     transition-timing-function    transition-delay延迟 

@keyframe    animation

### 转换

2D/3D转换

transform 属性向元素应用 2D 或 3D 转换。该属性允许我们对元素进行旋转、缩放、移动或倾斜     transform-origin  属性允许您改变被转换元素的位置     perspective  景深   transform-style  过渡样式     perspective-origin

属性定义 3D 元素所基于的 X 轴和 Y 轴。该属性允许您改变 3D 元素的底部位置

translate   移动  translateX  X轴移动    translateY  Y轴移动   translateZ Z轴移动   translate3d()  3D移动 rotate()     旋转rotateX()    X轴旋转      rotateY()   Y轴旋转      rotateZ()  Z轴旋转  rotate3d()   3D旋转  scale() 缩放    scaleX()    X缩放scaleY() Y轴缩放  scale()   scale()    skew()   斜切   skewX()    X斜切    skewY()  Y斜切   matrix()  

## 表格table

快捷创建表格   table>tr*3>td{123456}*3   右箭头     table>tr * 3>td{123456} * 3

	<table>
		<tr>
			<td>123456</td>
			<td>123456</td>
			<td>123456</td>
		</tr>
		<tr>
			<td>123456</td>
			<td>123456</td>
			<td>123456</td>
		</tr>
		<tr>
			<td>123456</td>
			<td>123456</td>
			<td>123456</td>
		</tr>
	</table>
tr：     <tr> </tr>     行，每一行

td:      <td> </td>    放置要展示的东西

th:       <th></th>    放置要展示的东西，等同于td，有文字自动加粗效果

e.g.一个简单的 HTML 表格（宽600px,高300px，边框1px,cellspacing间距，指单元格之间的距离,align设定图像的对齐方式, bacolor背景颜色），包含两行两列：

<table border="1" width="600" height="300" cellspacing="0" align="center" bgcolor="#ccc">align="center"在此处表示整个大框在页面中居中

<caption>……表 </caption>       caption表示当前表格的标题，文字自动居中

  <tr height="150" align="center"文字水平居中 valign="top"垂直上对齐 bgcolor="yellow">     align="center"在此处表示文字水平居中align="right"表示文字水平右对齐

    <th colspan="3">Month</th>         colspan="3"合并三列
    <th>Savings</th>            <th> </th>有字体加粗的效果
  </tr>

```
<table border="1">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td rowspan="2">$100</td>             合并两行
    <td>
    	<table>
    		 <tr>
               <th>Month</th>
               <th>Savings</th>
             </tr>
    	</table>
    </td>
  </tr>
</table>
```

  <tr>

    <td width="300" align="left"  valign="top" bgcolor="blue">January</td>
    <td>$100</td>
  </tr>
</table>

注：border-collapse: collapse;    合并大框和每一格的边框（在大框css中设置）

​        若某一个单元格内容较长，不想出现自动撑开的效果，在大框css中设置table-layout: fixed;宽度固定，另外要求自动换行，设置强制换行word-break: break-all;

​        <thead>   </thead>  

​        <tbody>   </tbody>

​        <tfoot>     </tfoot>

caption表示当前表格的标题，文字自动居中

### 响应式布局

`<!doctype html>

<html lang="en">

<head>

​    <meta charset="UTF-8">

​    <meta name="viewport"

​          content="width=device-width,user-scalable=no, initial-scale=1.0, maximum-scale=1.0,minimum-scale=1.0">

​    <metahttp-equiv="X-UA-Compatible" content="ie=edge">

​    <title>Document</title>

​    <style>

​        *{

​            box-sizing: border-box;

​        }

​        .box{

​            width: 1200px;

​            height: auto;

​            margin: 0 auto;

​        }

​        .item{

​            width: 25%;

​            height: 300px;

​            float: left;

​            background-color: yellow;

​            text-align: center;

​            line-height: 300px;

​            font-size: 30px;

​            color: #fff;

​            border: 10px solid #fff;

​        }`

​        













