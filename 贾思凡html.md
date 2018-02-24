# html

- > Hyper  text  markup language  超文本标记语言

  ## 标记 标签

  ### 行标签

  > - a（title  target  href ）  span   i    b   strong  em   time（定义日期/时间)  address(定义地址元素)	   progress (定义任何类型的任务的进度) 
  > - 不会独占一行
  > - 不能设置宽高

  ### 块标签

  > - 独占一行
  > - div(定义文档中的一个部分)	  p  pre(定义预格式化文本)    h1--h6   ul(定义无序列表)   li(定义列表的项目)    al   dl(定义定义列表)	dt(定义定义的项目)    dd(定义定义的描述)	header(文档的头部)	footer(文档的底部)	section(定义文档的一部分)	main(内容的主体部分)	video audio(视频，音频)

  ### 行内块标签

  > - 不会独占一行  也可以设置宽高
  > - img(src(图像的路径)	alt(显示图片加载失败时的信息)	width(设置图片的宽度)	height(设置图片的高度)	border(边框))	input(定义输入域)	textarea(文本区域)	select(定义可选列表)	option fieldset

  ## 实体

  ## &nbsp ;(空格)  &gt ;(大于号)	&lt ;(小于号)	&quot ;(引号)	&amp ;(和号)  &copy ;(版权符号)	&reg ;(注册商标)

  ## 表单

  - form(表单)(action(提交的地址)	method(设置提交的方式) get post)
  - 表单控件
  - 属性 (type  name  value  readonly(只读属性)   disable  checked  selected  maxlength
  - h5  (required(验证)	 placehoder(默认提示文字) 
  - - input类型(text(文本)	password(密码)	radio(单选按钮)	checkbox(多选按钮)	file	hidden	submit(提交按钮)	reset(重置按钮)	button(普通按钮))不需考虑兼容问题
    - h5 { email(邮箱)	url(路径)	date(天)	week(周)	month(月)	time(设置日期时间)	datetime-local(包含年月日)		number(数字)		range(范围)	serach(搜索框)	color(颜色)}

# 4 .css

## 引用方式

- 行内样式  style="width:100px; height:100px;"
- 嵌入样式 <style>.one{width:100px;} <style>
- 外部样式 <link rel="stylesheet" href="CSS/su.css">
- 引入样式 @import url("demo.css")  @import "demo.css"

## 选择器

- 标签选择器  div body   a
- 类名选择器  .one
- id 选择器      # one
- 后代选择器   ul  li
- 群组选择器   .one ,.two
- 交叉选择器    ul.one     .one.two
- 伪类选择器   ：hover  鼠标经过   ：active    鼠标按下  : visited  :鼠标移过   ：link
- 子选择器：div>a    .one>.two
- 同级选择器  div+p(前面必须有div)  div~p(前面有div就行)
- ：nth-child  :first-child   last-child  nth-last-child  only-child    p:nth-child(2)加数字表明第几个被选中
- ：nth-of-type  :first--of-type    last-of-type  nth-last-of-type(n)    only-of-type   区别在u是否是同一类型   p:nth-child(2n)实现条纹效果
- 属性选择器[data]:表示有data 属性的  [data=aa][data^ = aa ][data$=aa][data*=aa]    
- ：before  ：after
- ：checked
- ：target  ：root 

## 属性

### 布局

- width  height  margin  padding  float  position  box-sizing  display  left right   top  bottom  

### 样式

- background(背景)  background-image(背景图片)  background-color(背景颜色) background-repeat(背景是否平铺)  background-position(背景的位置)  background-attachment(背景是否固定或者随着页面的其余部分滚动)  background-size(规定背景图片的尺寸)
- border(边框)	border-width(规定边框的宽度) border-style(规定边框的样式) border-color(规定边框的颜色) background-clip(规定背景的绘制区域) background-origin (规定背景图片的定位区域) border-image border-radius 10px/20px(椭圆形圆角设置)  10px 10px 10px 10px 10px 10px 10px 10px 10px ;最多可以设置8个值box-shadow(阴影)  outline(在边框的外面，不占布局的位置，写法同border相同) outline-offset:20px 偏移

### 渐变

- linear-gradient()(线性渐变)

  repeating-linear-gradient()(重复的线性渐变)

  radial-gradient(径向渐变)

  repeating-radial-gradient(重复的径向渐变)

### 文字

- font-family(文字的字体)   font-size(文字大小)    color(文字颜色)	font-weight(文字粗细)   font-style(文字样式)    text-deecoration   text-align(文本对齐)   text-indent(文本缩进)   line-hight(行高)   word-break(文本换行)    letter-spacing(字间距)    vertical-align(文本垂直居中)

### 动画

- *transition	transition-property(定义过渡属性) 	transition-duration(持续时间)	transition-timing-function(动画函数)	transition-delay(动画延迟)
- @keyframe  animation  

### 转换

- transform	transform-origin	perspective(为 3D 转换元素定义透视视图)

  transform-style	perspective-origin

  translate(定义2D转换)	

  translateX(定义转换，只是用 X 轴的值)	

  translateY(定义转换，只是用 Y 轴的值)

  translateZ(定义 3D 转换，只是用 Z 轴的值)

  translate3d(定义 3D 转换)

  rotate(定义 2D 旋转，在参数中规定角度)

  rotateX(定义沿着 X 轴的 3D 旋)

  rotateY(定义沿着 Y 轴的 3D 旋转)

  rotateZ(定义沿着 Z 轴的 3D 旋转)

  rotate3d(定义 3D 旋转)

  scale(缩放转换)

  scaleX(通过设置 X 轴的值来定义缩放转换)

  scaleY(通过设置 Y 轴的值来定义缩放转换)

  skew(定义2D倾斜转换)

  skewX(定义沿着 X 轴的 2D 倾斜转换)

  skewY(定义沿着 Y 轴的 2D 倾斜转换)

  matrix(定义 2D 转换，使用六个值的矩阵)

# 响应式布局

## 1.随分辨率大小  由大到小变化

```
css：
*{
	box-sizing:border-box;
}
.container{
	width: 1200px;
	height: auto;
	margin: 0 auto;
}
.item{
	width: 100%;
	height: 300px;
	float: left;
	text-align: center;
	background: red;
	line-height: 300px;
	color: #fff;
	font-size: 30px;
	border: 10px solid #fff;

}*

/*媒体查询 根据当前的分辨路来控制某一部分样式是否起作用
		阀值*/
	/*	min-width max-width*/
		/*@media screen  and (max-width:1280px){
```

```
			.container{
				width: 900px;
			}
			.item{
				width: 33.3332%;
			}
		}*/
		/*@media screen  and (max-width:960px){
```

```
			.container{
				width: 600px;
			}
			.item{
				width: 50%;
			}
		}*/
		/*@media screen  and (max-width:640px){
```

```
			.container{
				width: 300px;
			}
			.item{
				width: 100%;
			}
		}*/
	HTML：	
	<div class="box">
		<div class="item"></div>
		<div class="item1"></div>
		<div class="item"></div>
	</div>
```

## 2.随分辨率大小  由小到大变化



```
css：
*{	
	box-sizing:border-box;
}
.container{
	width: 300px;
	height: auto;
	margin: 0 auto;
}
.item{
	width: 100%;
	height: 300px;
	float: left;
	text-align: center;
	background: red;
	line-height: 300px;
	color: #fff;
	font-size: 30px;
	border: 10px solid #fff;

}*
@media screen  and (min-width:640px){
	.container{
				width: 600px;
			}
	.item{
				width: 50%;
			}
}*/
/*@media screen  and (min-width:960px){
	.container{
				width: 900px;
			}
	.item{
				width: 33.3333%;
			}
	.item：last-child{
				display:block;
			} 隐藏某一部分
}*/
/*@media screen  and (min-width:1240px){
	.container{
				width: 1200px;
			}
			.item{
				width: 25%;
			}
		}*/
```

```
html：
	<div class="box">
		<div class="item"></div>
		<div class="item1"></div>
		<div class="item"></div>
	</div>
```

## 3.随分辨率大小  到一定阀值时，先等比例缩小，宽高也等比列缩小，然后继续缩小分辨率，通过流布局实现。



	css；
	*{	
		box-sizing:border-box;
	}
	.container{
		width: 1200px;
		height: auto;
		margin: 0 auto;
	}
	.item{
		width: 50%;
		height: auto;
		/*height: 50%;*/
		float: left;
		text-align: center;
		background: red;
		/*line-height: 300px;*/
		color: #fff;
		font-size: 30px;
		border: 10px solid #fff;
		padding-top: 25%;
		position: relative;
	}
	.content{
		width: 100%;
		position: absolute;
		left: 0;
		top: 0;
	}
	@media screen  and (max-width:1200px){


			.container{
				width: 1000px;
			}
			.item{
				/*width: 33.3332%;*/
			}
		}
		@media screen  and (max-width:1080px){


			.container{
				width: 600px;
			}
			.item{
				width: 100%;
				padding-top: 50%;
			}
			
		}
		@media screen  and (max-width:640px){


			.container{
				width:100%;
			}
			.item{
				width: 100%;
				padding-top: 50%;
			}
			
		}
		html:
		<div class="container">
			<div class="item">
				<div class="content">
					1
				</div>
			</div>
			<div class="item"></div>
			<div class="item"></div>
			<div class="item"></div>
		</div>
		最后得流布局 不能写内容  如果需要 需使用定位。
