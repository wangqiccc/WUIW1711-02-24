#### html:(hyper Text markup language)	超文本

### 标记	标签

#### 行标签

​	不会独占一行

​	不能设置宽高

​	a（href 	title target）	span	i  em	b  strong	

​	time	address

#### 块标签

​	独占一行

​	div		h1~h6	p	pre		ul（无序列表）		li	ol（有序列表）	dl（定义定义列表）	dt（定义定义项目）	dd（定义定义的描述）	

​	header	footer	section	main

​	video（视频）	audio（音频）

​	form（表单）

#### 行内块标签

​	不会独占一行

​	也可以设置宽高

​	img(src	alt	width	height	border)

​	textarea（定义多行文本输入控件）	select	option（定义选择列表）	fieldset(打包组合)

### 实体

​	&nbsp;&nbsp;空格	&lt;	&gt;	&

### 表单

​	form	(action提交地址	method)

#### 	表单控件

​		类型input(text	password	radio（单选按钮）	chechbox（多选按钮）	file（路径）	hidden（隐藏）	submit	reset重				置		button)

​		(email	url	date	week	month	time	datetime-local（本地时间显示）	number		range（范围）	search（搜素框）	color)

​		属性(type	name	value	readonly（只读）	disable	checked	selected	maclength)

​		(require		placeholder)

### css

#### 	引用方式

##### 		行内样式：style="宽高"

##### 		嵌入样式：<style></style>

##### 		外部样式：<link	rel='stylesheet'	href="">

##### 		引入样式(css中引入其他css)：@import	url("demo.css");		@import	"demo.css";	

#### 	选择器

##### 		标签选择器：div	body	a

##### 		类名选择器：.

##### 		id选择器：#s

##### 		后代选择器：ul	li

##### 		群组选择器：.类名,.类名

##### 		交叉选择器（俩个选择器合起来）：ul.one	.one.two

##### 		UI伪类选择器（用户交互）：:link	:hover		:active（按下）		:vidited（访问）

##### 		子选择器：div.a(div中的子元素)		.one>.two（前一个元素的子元素）

##### 		同级选择器：div+p（紧按）	div~p

##### 		div:nth-child（正数第几个	2n）	:first-child（第一）	:last-child（最后）	:nth-last-child（倒数）	:only-child（唯一）

##### 		:nth-of-type(同类型里的第几个)	:first-of-type	:last-of-type		:last-of-type			:nth-last-of-type		:only-of-type

##### 		属性选择器：[data]data=aa	data^=aa	data$=aa	data*=aa

##### 		:before		:after

##### 		:checked	

##### 		:target		:root

#### 	属性

##### 		布局：

​			width		height		margin		padding	float	position	

​			box-sizing		display	left	top	right  bottom 		z-index（层级）

##### 		样式：

​			background	background-image（背景图片）	background-color	background-repeat（平铺）				 

​			background-			postion（设置背景图的起始位置）	background-attachment（背景图是否固定/随着页面其余部分滚动）

​			border（边框）	border-	width	border-color	border-style		background-clip（背景的绘制区域）

​			background-origin（背景的定位区域）	background-size（背景图大小）			border-image（边框图片）	

​			border-radius（圆角）	

​			box-shadow（阴影,可以写无数组）		outline（轮廓线）	out-line-offset（轮廓线偏移）

​			border-radius:10px	20px	40px	50px/20px	30px	40px	50px;

​			background-position:left	top,right bottom;

##### 		渐变：

​			linear-gradient()（渐变色从左往右/从右往左）	repeating-linear-gradient()（最近边，最远边）	

​			radial-gradient()	（最近角，最远角）			repeating-radial-gradient()（重复渐变）

##### 		文字：

​			font-famiy	font-size	font-weight（字体粗细）		color	font-style（字体样式）	text-decoration（文本添加修饰）				

​			text-align（水平居中）	text-indent（首行缩进）	line-height	word-break（换行）	letter-spacing（字间距）	

​			vertical-align（垂直设置）

##### 		动画：

​			transition		transition-property（属性）	transition-duration（持续时间）	

​			transition-timing-function（）（以同样速度从开始到结束）	trandition-delay（延迟）		@keyframe		animation

##### 		转换：

​			transform		transfrom-origin（改变被转换元素的位置）	perspective（规定3d元素的透视效果）		

​			transfrom-style（被嵌套元素如何在3d中显示）	perspective-origin（规定3d元素的底部位置）	

​			translate（移动元素）			translateX	translateY	translateZ		

​			translate3d()	rotate()（旋转）	rotateX() rotateY() rotateZ rotate3d()		scale()（斜切，放大）scaleX()	scaleY()	

​			skew()（倾斜转换）	skewX()	skewY()		matrix()（使用六个值的矩阵）

### 表格（table）tr（行）td（列）没有设置宽高，宽高取决内容的多少

​	width="";hight="";border="1"（边框粗细）

​	cellspacing="0"（边框间距）	align="center"（居中）	bgcolor

#### 	tr:height="150"（高度一半）	align="center"（文字水平居中）	valign="top"（垂直）	bgcolor

#### 	td:width	align	valign	bgcolor

#### 	css:

##### 		table:width	height	border		border-collapse:collapse（边框合在一起）		margin:0 auto	text-align	

##### 			table-layout:fixed（文本超出）	word-break:break-all（自动换行）

##### 		tr:border

##### 		td:	rowspan="2"（合并行）	

##### 		tr:nth-child

##### 		th:（表头单元格列，文字居中，加粗）colspan="3"（合并列,不同的块里不能合并）

##### 		其它标签：thead		tbody	tfoot	caption（标题，名称）

.mytable2 tr:last-child>td{}子元素

### 响应式：

#### 	媒体查询（根据当前设备的分辨率来控制某一部分样式是否起作用,有特定顺序）

##### 		流式布局：

​			@media screen and (max-width:1040px){.box{width:100%}}（阀值min-width max-width）



##### 		固定布局：box-sizing:border-box;（大-小（max）		小-大（min反））

​			@media screen and(max-width:1240px){.box{width:900px;}.item{width:33.3333%}}

​				当为三个时最后一个隐藏dispaly:none;其他显示display:block;

​			@media screen and(max-width:900px){.box{width:600px;}.item{width;50%}}

​			@media screen and(max-width:640px){.box{width:300px;}.item{width;100%}}



##### 		高宽等比例缩放

​			里边容器：高不设置值,设置padding-top的比例，写内容设置定位position:relative;

​			外边容器：定位position:absolute;width:100%;hight:100%;（内容自动撑开）

​			@media screen and(max-width:1200px){.box{width:1000px;}}



### 动画:

#### 	父元素：transtion

#### 	子元素：transfrom:rotate();

​		animation-name:rotate;名称

​		animation-duration:5s;时间

​		animation-timing-function:linear;速度：匀速

​		animation-delay:2s延迟

​		animation-iterantion-count:2;旋转次数

​		animation-direction:alternate;（正序倒序）

​		animation-fill-mode:forwards/backwards动画播放完的状态

​		animation-play-state:pasued;（移入暂停）

#### 	@keyframes rotate{

​		0%{

​			transfrom:rotate(0deg);

​			}

​		100%{

​			transfrom:rotate(360deg);

​			}



#### 