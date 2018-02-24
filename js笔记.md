# js笔记

安装webstorm

HTML是超文本标记语言（hyper text markup language）

## 一、标记/标签：

​	块标签：div 、 h1-h6、  p 、 pre、ul、li、 ol dl  dt  dd  header  footer section main  vidio audio  form

​	行标签：a(target替换还是打开新的页面)  span 、i、em   strong  time  address  prigess表示进度

​	行内块级标签img :（src  alt  width  hight  boder）、input、textarea 、select、option、fieldset

实体：&nbsp；&lt；&gt；&map；&quote；

## 二、表单

### 	form（action提交的地址  、  method:get/post)

​		table-layout：fixed；固定每个单元格的大小

​		border-collapse：collapse；

​		word-break: break-all;自动换行

​		colspan="3"合并三列

​		rowspan="2"合并俩行

​		<caption>xxx表</caption>标题

### 	表单控件

​			input{password  text  radio  checkbox   file  hidden  submit  botton  reset }

​			(新增  email  url   date  week  month  time  datetime-local  number  range:滑块的展示效果  search  color)

​			属性( type name  value  readOnly   disable  checked  selected maxlength )(require  pleaceholder)

## 三、css回顾

### 1.选择器

#### 标签选择器

​			div   body  a

#### 类名选择器

​			.one

#### ID选择器

​			 #one

#### 后代选择器

​			 .one .two   ul li

#### 群组选择器

​			  .one,.two

#### UI伪类选择器    

​			：link标签为选择的样式      ：hover鼠标经过的样式     ：active鼠标按下的样式        ：visited标签选择过的样式

#### 子选择器

​			div>a        .one>.two

#### 同级选择器   

​			   div+p 选择的是p标签   意思是前边必须有div标签的p标签

​			   div~p  选择的是p标签

#### 交叉选择器    

​			 ul.one      one.two

#### 特殊选择

​			:nth-child()（父元素里第几个）可以结合变量    :first-child()（父元素里第一个）     :last-child() （父元素里最后一个）    :nth-last-child() （父元素里倒数第几个）    :ony-child() （父元素里唯一的）  

​			：nth-of-type()（同类型的第几个）     ：first-of-type()       ：last-of-type()       ：nth-last-of-type()       :only-of-type()

#### 属性选择器

​			[data]（data）data=aa（开始）[data$=aa]（结束）[data*=aa]

:before    :after

:checked    （被选中）

:target    :root

### 2.属性

#### 	布局

​			width宽     hight高     margin元素间距    padding内容和边框的距离     float浮动    position定位，有四个（相对定位、绝对定位、固定定位、默认定位） left   right   top  bottom   z-index层级关系设置     box-sizing以特定的方式定义匹配某个区域的特定元素，默认值是content-box.   display块元素、行内元素、行内块元素十七可以相互具有本身没有的功能，可以设置容器，隐藏三个功能。

#### 	样式

​		背景：background  background-color设置背景颜色   background-image设置背景图片  background-position背景位置   background-repeat 背景图不重复  background-attachment背景图是否固定    	background-clip背景绘画区域    background-origin背景绘画起始点      background-size设置大小   

边框  border   border-width边框宽     border-color边框颜色     border-style边框的样式        box-shadow（可以重复设值，盒子的阴影           box-shadow: 0 0 10px 20px #000, 0 0 10px 20px blue;）   border-radius ：border-radius: 10px 20px 30px 40px/20px 30px 40px 50px;      /* 左上角横轴10px，纵轴20px,右上角横轴20px，纵轴30px，左下角横轴30px，纵轴40px，右左下角横轴40px，纵轴50px */  ）  outline和border一样的写法，不占盒子大小，在border外边      outline-offset偏移，即往外扩展

#### 	渐变

​			线性渐变linear-gradient（）     repeating-linear-gradient（）   径向渐变 radial--gradient（）    repeating-radial-gradient（）  

#### 	文字

​			work-break文字自动换行    letter-spacing字间距    vertical-align设置垂直方向对齐方式    text-indent首字缩进

#### 	动画

​			1.transition设置过度属性     transition-property定义过度属性    transition-duration定义过度持续时间      transition-timing-function动画函数    transition-delay动画的延迟

​			设置动画的方式1.@keyframe       2. animation

#### 	转换

​			transform     transform-orign      transform-style       perspective       perspective-orign

​			translate     translateX             translateY             translateZ      translate3d（）平移

​			rotate（）        rotateX（）    rotateY（）    rotateZ（）    rotate3d（）旋转

​			scale（）     scaleX（）   scaleY（）       skew（）      skewX（）  skewY（）放大缩小

​			matrix（）矩阵	  

### 3.引用方式

- 行内样式 style="width:100px;height:100px;"
- 嵌入样式 <style>.one{width:100px;height:100px;};</style>
- 外部样式 <link rel='stylesheet' href="">
- 引入样式 @import url("demo.css");   @import  "demo.css"



