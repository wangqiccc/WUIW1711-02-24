# 一、html: Hyper Text Markup Language  超文本标记语言

### 标记/标签

##### 行标签：

​	本身不会独占一行；不能设置宽高；a（设置href   title  target）、span、i、em、b、strong、time、address、progress（已经完成的进度）

##### 块标签：

​	独占一行；div、h1~h6、ul、li、ol、dl、dt、dd、header、footer、section、main、vedio（视频）、audio（音频）、form

##### 行内块级标签：

​	不会独占一行；可设置宽高；img（src、 alt、  width、height、border）、input 、textarea（定义多行文本框）、select、option、fieldset（对表单进行分组）

##### 实体：空格&absp;(换行)     &lt；&gt；  &quot； &amp；（和）

##### 表单：form(action、method)

##### 表单控件：

​	input（text 、password、radio、checkbox、file、hidden、submit、reset、button） （email、url（地址）、date  week  month time （日期） datetime-local（时间）   number（数字）  range    search   color）

##### 属性：

​	（type、name、value[默认值]    readonly、disable、checked、 selected、maxlength）   （required、placeholder）

# 二、css：引用方式：

##### 行内样式：

​		style="width:100px; height:100px;"

##### 嵌入样式：

​		<style>.one{width:100px;}<style>

##### 外部样式：

​		<link rel='stylesheet' href="">

##### 引入样式：

​		@import url(demo.css);

​	         @import "demo.css"

##### 选择器： 标签选择器	div    body      a

##### 类名选择器	.类名{}

##### id选择器		#id{}

##### 后代选择器	.父类 .子类{}

##### 群组选择器	.one，.two{}

##### 交叉选择器	ul.one     .one.two{}

##### UI伪类选择器  	:link     :hover     :active   :visited

##### 子选择器    div>a     .one>.two

##### 同级选择器	div+p       div~p         (选择的是p标签     必须紧挨着)

​		:nth-child（2）{}    （里面写具体数字   eg：2    eg：2n /2n-1[多个：偶数/奇数]）

​	        :first-child{} （第一个）         

​	        :last-child {} （最后一个）     

​	    	:nth-last-child{}  (倒数第几个)          

​	        :only-child{} （唯一的子元素）	

​		:nth-of-type(2){} (子元素同类型的第几个)

​		:first-of-type{}           :last-of-type{}  

​		:nth-last-of-type{}

​		:only-of-type{}（同类型里 唯一的）

##### 属性选择器:

​	    [data]    

​            [data=aa]

​	    [data^=aa]

​	    [data$=aa]

​	    [data*=aa]

​		:before          :after         

​		:checked       :selected        :target

​		:root

##### 属性：

​	布局：

​		width    height     margin      padding 

​		float     position      box-sizing(定义当前盒子模型的宽高包括方式  content-box      border-box)

​		display     left    right       top        bottom

​		z-index

​	样式：

​		background    background-image（背景图）        background-color （背景颜色）     

​		 background-position （位置）     	background-repeat（是否重复）

​		background-attachment   （定义背景图片随滚动轴的移动方式）

​		border        border-width（边框宽度）             border-style （边框样式）       border-color（边框颜色）

​		background-clip （图片裁剪）      background-origin（图片起始位置）        background-size(背景大小)

​		border-image （指定作为div元素周围边框的图像）

​		border-radius（圆角）

​		box-shadow（阴影）

​		outline:1px solid #000;（不占布局位置   在边框外再加一层）

​		outline-offset( 轮廓线偏移 视觉效果  不占布局位置)

​	渐变：

​		linear-gradient（）    （线性渐变）

​		repeating-linear-gradient（）     （创建一个由重复线性渐变组成的 image）

​		radial-gradient（）    （径向渐变）

​		repeating-radial-gradient（）         （ 创建一个从原点辐射的重复渐变组成的 image）

​	文字：

​		font-family（字体）       font-size（字体大小）   color       font-weight       text-decoration（下划线）    

​		 text-align（文本居中）     text-indent（首行缩进）       line-height（垂直居中）

​		word-break（自动换行）          letter-spacing（字间距）         vertical-align（垂直对齐）

​	动画：

​		transition        transition-property（过渡属性）   transition-duration（持续时间）    transition-timing-function（动画过渡函数）

​		transition-delay（延迟）

​		@keyframe         animation（动画）

​	转换：

​		transform     transform-origin（起始点）   perspective（景深）     transform-style      perspective-origin（转换的基本点）

​		translate           translateX（）     translateY（）          translateZ （）         translate3d（）      平移   

​		rotate（）       rotateX（）          rotateY（）   rotateZ（） rotate3d（）    旋转

​		scale（）        scaleX（）         scaleY（）       放大缩小

​		skew（）      skewX（） 	skewY（）                斜切

​		matrix（）  矩阵

# 三、表格

##### 只有表格可用

			border-collapse: collapse;
			table-layout: fixed;
```
<table width="600" height="300" border="1" cellspacing="0" align="center" bgcolor="skyblue">
	<tr height="150" align="center" valign="top" bgcolor="pink">
		<td width="300" align="left" valign="top" bgcolor="yellow">12345</td>
		<td>12345</td>
		<td>12345</td>
		<td>12345</td>
	</tr>
</table>
```

# 四、响应式布局

##### 1.从大到小

```
<style>	
	*{
		box-sizing: border-box;
	}
	.container{
		width: 1200px;
		height: auto;
		margin: 0 auto;
	}
	.item{
		width: 25%;
		height: 300px;
		float: left;
		background-color: pink;
		font-size: 30px;
		color: #fff;
		text-align: center;
		line-height: 300px;
		border: 10px solid #fff;
	}
	@media screen and (max-width: 1280px){
		.container{
			width: 900px;
		}
		.item{
			width: 33.3333%;
		}
	}
	@media screen and (max-width: 960px){
		.container{
			width: 600px;
		}
		.item{
			width: 50%;
		}
	}
	@media screen and (max-width: 640px){
		.container{
			width: 300px;
		}
		.item{
			width: 100%;
		}
	}
</style>
```

```
<body>	
	<div class="container">
		<div class="item">1</div>
		<div class="item">2</div>
		<div class="item">3</div>
		<div class="item">4</div>
	</div>
</body>	
```

##### 2.从小到大

```
<style>	
	*{
		box-sizing: border-box;
	}
	.container{
		width: 1200px;
		height: auto;
		margin: 0 auto;
	}
	.item{
		width: 25%;
		height: 300px;
		float: left;
		background-color: pink;
		font-size: 30px;
		color: #fff;
		text-align: center;
		line-height: 300px;
		border: 10px solid #fff;
	}
	@media screen and (max-width: 1280px){
		.container{
			width: 900px;
		}
		.item{
			width: 33.3333%;
		}
	}
	@media screen and (max-width: 960px){
		.container{
			width: 600px;
		}
		.item{
			width: 50%;
		}
	}
	@media screen and (max-width: 640px){
		.container{
			width: 300px;
		}
		.item{
			width: 100%;
		}
	}
</style>

<body>
	<div class="container">
		<div class="item">1</div>
		<div class="item">2</div>
		<div class="item">3</div>
		<div class="item">4</div>
	</div>
</body>
```

# 五、流式布局



	<style>	
		*{
			box-sizing: border-box;
		}
		.container{
			width: 1200px;
			height: auto;
			margin: 0 auto;
		}
		.item{
			width: 50%;
			height: auto;
			float: left;
			background-color: pink;
			font-size: 30px;
			color: #fff;
			text-align: center;
			border: 10px solid #fff;
			padding-top: 50%;   /*相对于当前容器的宽度*/
			position: relative;
		}
		.content{
			width: 100%;
			height: 100%;
			position: absolute;
			left: 0;
			top: 0;
		}
		@media screen and (max-width: 1200px){
			.container{
				width: 1000px;
			}
		}
		@media screen and (max-width: 1080px){
			.container{
				width: 600px;
			}
			.item{
				width: 100%;
			}
		}
		@media screen and (max-width: 640px){
			.container{
				width: 100%;
			}
			.item{
				width: 100%;
			}
		}
	</style>
	
	<body>
		<div class="container">
			<div class="item">
				<div class="content">1</div>
			</div>
			<div class="item"></div>
			<div class="item"></div>
			<div class="item"></div>
		</div>
	</body>
# 六、动画

	<style>
		@keyframes rotate{
			0%{
				transform: rotate(0);
			}
			100%{
				transform: rotate(360deg);
			}
		}
		div{
			width: 300px;
			height: 300px;
			background-color: pink;
			transition: transform 1s linear;
			animation-name: rotate;
			animation-duration: 5s;
			animation-timing-function: linear;   /*动画方式 */ 
			animation-delay: 2s;    /*延迟*/
			animation-iteration-count: infinite;   /*动画一直转*/
			animation-direction: alternate;   /*倒转*/
			animation-fill-mode: forwards;     /* 开始方向forwards       结束方向backwards*/
			animation: rotate 5s linear 1 alternate forwards;         /*整合*/
		}
		div:hover{
			transform: rotate(360deg);
			animation-play-state: paused;    /*鼠标移入停止转动*/
		}
	</style>


	<body>	
		<div class="box"></div>
	</body>






