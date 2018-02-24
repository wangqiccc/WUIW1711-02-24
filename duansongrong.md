# 总结

## 一、HTML			

1.Hyper  Text  markup  language  超文本标记语言

### 2.标记/标签

行内标签：不会独占一行，不能设置宽高	a (href   title鼠标移入以后的提示信息   target目标的位置)	 span   i     em    b   strong	 time    						address  	progress---进度		

块标签	：独占一行 div     h1~h6     p      pre     ul   li    ol   dl     dt    dd      header     footer     section    main   video  audio  form  									

行内块级标签：不会独占一行，也可以设置宽高       img(src  alt  width  height   border)   input  textarea   select   option  fieldset

### 3.实体

空格	&nbsp	&lt	&gt		&quto	&amp

### 4.表单

1）form(action---指定数据的处理文件	method---指定数据提交方式 （*get：速度快，不安全 *post：速度慢，安全）

2）表单控件		input(text	password	radio---单选	checkbox	file--文件域	hidden---隐藏域	submit	reset	button)

​	h5新增：(email	url	  date	week	month	time	datetime-local	number		range滑块展示效果	search	color)

3）属性		type	name	value---设置input的默认值	

​			readOnly	disable	   checked	  selected	maxlength

​			required	---提示必填	placeholder---设置input的提示信息

## 二、css

### 1.引用方式

行内样式		style="width:100px;	height:100px;"

嵌入样式		<style>.one{width:500px;  height:500px;}</style>

外部样式		<link  rel='stylesheet   href="" >  

引入样式		@import  url("demo.css")  ;		@import   "demo.css" ;

### 2.选择器

1）标签选择器	div		a	body

2）类名选择器	.one

3）id选择器		#one

4）后代选择器	.one  p

5）群组选择器	.one, .two

6）交叉选择器	ul.one	.one.two

7）UI伪类选择器	:hover	:active	:visited	:link

8）子选择器		div>a

9）同级选择器	div+p	div~p

10）:first-child	:nth-child()	:last-child	:nth-last-child()	:only-child

​	:first-of-type		:nth-of-type()		:last-of-type		:nth-last-of-child()	:only-of-type

实现条纹效果:nth-child(2n)		:nth-child(2n-1)

11）属性选择器	[data]

​			[data=aa]

​			[data^aa]

​			[data$aa]

​			[data*aa]

12）:before	:after

:checked

:target   锚链接的地址			:root

### 3.属性

#### 1）布局

width	height	margin	padding		float	position		box-sizing	display	left	right	bottom	top	z-index	

#### 2）样式

background	-----	background-image	background-color	background-repeat	background-position	background-attachment

​				background-clip		background-origin	background-size


		/*背景颜色*/
		background-color: red;
		/*背景图*/
		background-image: url('img/1.jpg');
		
		/*设置背景平铺与否*/
		background-repeat: no-repeat;
		
		/*背景图大小(长度/百分比/contain/cover)*/
		background-size: 500px 500px;
		background-size: 100% 100%; 与背景图一样大，图片易变性;
		background-size: contain; 图片等比例缩放，图片可完整展示，会出现覆盖不完整的情况;
		background-size: cover; 覆盖整个盒子，但是会出现显示不完整;
		
		/*图片位置的设置，常设center*/
		background-position:center;
		
		/*设置图片裁剪区域,默认的是border*/
		background-clip: border-box;
		
		/*设置图片绘制的起始位置，默认的是padding*/
		background-origin: border-box;
		
		/*设置背景图是否根据内容滚动*/
		background-attachment: fixed;
border	-----	border-width	border-style		border-color		border-image

​			border-radius	box-shadow阴影

​			box-shadow: inset  20px  -3px  20px  5px  rgba(148, 166, 173, 1);----内外阴影、x、y、模糊度、大小、颜色

轮廓线（设值与边框一致）outline:1px solid  red;	   outline-offset:20px;   偏移

阴影可以设值模拟多边框

#### 3）渐变

linear-gradient()---线性渐变		repeating-linear-gradient()	---重复线性渐变	

radial-gradient()---径向渐变		repeating-radial-gradient()---重复径向渐变

#### 4）文字

font-family	font-color	font-size		font-weight---字体粗细		

font-style---字体样式	text-decoration---文本修饰	     text-align---水平对齐方式	     

text-indent---文本首行缩进	   line-height---行高

word-break---强制换行	letting-spacing---字间距	vertical-align---垂直对齐方式

#### 5）动画

transiton      ---- 	transition-property	transition-duration	transition-timing-function		transition-delay

@keyframe	animation

```
		animation-name: rotate;
		animation-duration: 5s;/*动画持续时间*/
		animation-timing-function: linear;/*动画执行速度：匀速*/
		animation-delay: 2s;/*动画延迟时间*/
		animation-iteration-count: infinite;/*动画执行次数：无数次*/
		animation-direction: alternate;/*正反交替执行*/
		animation-fill-mode: forwards;/*旋转结束后，对象停止的方向*/
		div:hover{
			animation-play-state: paused;/*鼠标指向对象后，旋转停止*/
		}
```

#### 6)转换

transform   -----	transform-origin---设置元素的基点转换位置		perspective---设置景深以及位置		

​				perspetive-origin

​				transform-style----transform-style: preserve-3d

​								transform-style: flat

​								transform-style: inherit	

translate -----	    translateX	translateY	translateZ	translate3d()		

​		旋转：rotate()		rotateX()		rotateY()		rotateZ()		rotate3d()		

​		放大缩小：scale()		scaleX()		scaleY()	

​		斜切：skew()		skewX()		skewY()

​		矩阵：matrix()