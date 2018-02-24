#### 一.hyper text market language  超文本标记语言

#### 二.标记标签

​	1行标签：不会独占一行，不能设置宽高（a（href链接地址，titlt标题，target目标位置） ，span，i，em，b，strong，time，address）

​	2块标签：独占一行，（div，h1-h6，p，pre，ul，li，ol，dl，dt，dd，header，footer，section，main，video，audio）

​	3.行内块级标签：不会独占一行，也可以设置宽高（img（src，alt，width，height，border），input，textarea，select，option，					       		fieldset，

#### 三.实体

​	空格等

#### 四.表单

​		form(action(提交地址) method（提交方式）)

​		表单类型：（text(单行文本框)，		password(密码框)，		radio(单选按钮)，		checkbox(复选框)，		file(文件上传框)，				hidden(隐藏域)，		submit(提交按钮)，		reset(重置按钮)，		button()普通按钮）		（新增	email(限制输入电子邮件地址)，				url(限制输入url地址)，		date(限制输入日期，日期选择器一般会出现在输入字段中)，week(允许用户选择周和年)，				month(允许用户选择月份和年)，				time(允许用户选择时间)，			datetime-local(允许用户选择日期和时间)，	number(限制输入数字)，	range(限制只能输入一定范围内的值)，			search(搜索文本，类似单行文本)，		color(限制输入颜色，颜色选择器一般会出现在输入字段中)）

​		属性type：(类型name(名称)，	v	alues(默认值)，			readonly（表示该框中只显示，不可修改），		disabled(表示不可更改和点击，不会被提交，不需要值)，	checked(带预选定的复选框)，			selected(下拉框)，				maxlength(输入的最大长度)）（新增required(布尔属性，必须填写内容，不需要值)，				placeholder(提示信息，显示在用户输入信息之前)）

#### 五.css引入方式

​	1.行内样式 style=“width:5px；height：1px；”

​	2.嵌入样式 <style>.a{width:5px;}</style>			   

​	3.外部样式<link>

​	4.引入样式@import url（"index.css");/@import "index.css"(新版本)   先link引入a.css，然后a里import b.css

#### 六.选择器

​	1.标签选择器

​	2.类名选择器

​	3.id选择器

​	4.后代选择器

​	5.群组选择器

​	6.交叉选择器ul.a    .one.two

​	7.UI伪类选择器      ：hover鼠标移入          ：link未被选择的样式    ：active正在点击时的样子     ：visited鼠键点击后的效果

​	8.子选择器     div>a          .one>.two

​	9.同级选择器    div+p/div~p       p紧挨着div才行/ p不紧挨着div也行

​	10.:nth-child()      :first-child     :last-child     :nth-last-child()   :only-child                           :first-child父元素的 第一个元素(括号里面加数字表示从前向后第几个，  :nth-last-child() 示从后向前第几个，可以加2n表示第2，4.6个（2的倍数），也可以3n-1)

​		nth-of-type()      :first-of-type     :last-of-type     :nth-last-of-type()     :only-of-type     :first-of-type类型相同的第一个子元素  

​	10.属性选择器([data],[data==a],[data^=aa],[data$=aa],[data*=aa])

​	11.:before   :after

​	12.:checked

​	13.:target   :root

#### 七.属性	

布局：

width(宽),		height(高),		margin(外边距),		padding(内边框),		float(浮动),		position(定位),		box-sizing(盒子计算范围),		display(定义元素类型),					left(左，结合定位使用),right(右，结合定位使用),top(上，结合定位使用),bottom(下，结合定位使用),		z-index(层级关系)

样式：

background,(背景)

background-image(规定要使用的背景图片),		background-color(规定背景颜色),		background-repeat(规定如何重复背景图片，是否平铺),		background-position(规定背景图片的位置),		background-attachment(规定背景图片是否固定或随页面滚动),		background-clip(设置图片裁剪区域),		background-origin(设置图片绘制的起始位置),		background-size(设置背景图片的大小),

border(边框)：

,border-width(边框的宽),		border-style(边框的风格：实线，虚线等),			border-image(边框图片),		border-ridius(圆角边框)（10px 20px代表左上右下10，左下右上20，10px/20px代表w10，h20的角不是圆的）,			box-shadow（盒子阴影可以弄无数层）,		outline(轮廓线),		outline-offset(轮廓线的偏移，四面距离一样，视觉效果，不占位置)

渐变：

liner-gradient()(线性渐变),			repeating-liner-gradient()(重复性的线性渐变),			redial-gradient()(径向渐变),			repeating-redial-gradient()(重复性的径向渐变)

文字：

font-family(字体类型),		font-size(字体大小),		font-weight(字体粗细),			color(字体颜色),		font-style(字体样式),		text-decoration(文本修饰),	text-align(水平对齐方式),	text-indent(首行缩进),			line-height(行高，可是让文字垂直居中),		word-break(换行),		letter-spacing(字间距),		vertical-align(垂直对齐)

动画：

transiton

 transistion-property(过渡效果应用在谁身上),		transition-duration(过渡时间长度)，		transition-timing-function（时间函数，规定过渡的速度）,		transition-delay(过渡延迟)

@keyframe( 指定动画名称和动画效果),animation( 所有动画属性的简写属性)

转换：

transform

transform-origin,perspective,transform-style,perspective-origin(观察点)，translate()(平移),translateX()(x轴平移), translateY()(y轴平移),translateZ()(z轴平移),translate3d()(定义3d转换),rotate()(旋转),rotateX()(沿x轴旋转),rotateY()(沿y轴旋转),rotateZ()(沿z轴旋转),rotate3d()(定义3d转换),scale()(缩放),scaleX()(沿x轴缩放),scaleY()(沿y轴缩放),skew() (沿着 X 和 Y 轴的 2D 倾斜转换)。,skewX()(沿着 X轴倾斜),skewY()(沿着 y轴倾斜),matrix( ax+cy+e:bx+dy+f)

#### 八：table

		.a{
			border-collapse: collapse;/* 合并边框 */
			table-layout: fixed; /* 列宽由表格宽度和列宽度设定  */
			word-break: break-all;/* 换行 */
			width: 500px;
			border: 1px solid red;
		}
		.a td{
			border: 1px solid red;
		}
		.a tr:first-child{
			height: 200px;
		}
		.b{
			border: 1px solid green;
		}
		</style>
	</head>
	<body>
		<table width="500" height"500" border="1" cellspacing="0" align="center" bgcolor="#999">
			<thead>
			<caption>xxx</caption>
			<tr height="150" align="center" valign="top" bgcolor="red" ><!-- 只设置高度 -->
				<th colspan="2" rowspan="2">zzzzzzzz
					<table class="b">
						<tr class="b">
						<th class="b">lll</th>
						</tr>
					</table>
				</th><!-- colspan合并行单元格  rowspan合并行单元格，必须在同一个thead或者tbody或者tfoot-->
				
			</tr>
			<tr height="150" align="center" valign="top" bgcolor="red">
			</tr>
			</thead>
			<tbody>
			<tr height="150">
				<td width="250" align="left" valign="top">zzzzzzzz</td>
				<td>zzzzzzzz</td>
			</tr>
			</tbody>
			<tfoot>
			<tr>
				<td>zzzzzzzz</td>
				<td>zzzzzzzz</td>
			</tr>
			</tfoot>
		</table>
		<table class="a">
						<tr >
							<td>001zzzzzzzzzzzzzzzzzzzzzzzaaaaaaaaaaasdddddddd</td>
							<td>002</td>
							<td>003</td>
						</tr>
						<tr>
							<td>001</td>
							<td>002</td>
							<td>003</td>
						</tr>
						<tr>
							<td>001</td>
							<td>002</td>
							<td>003</td>
						</tr>
		</table>			
	</body>
		th标题头用，自动居中加粗
		caption标题，自动居中
		想要分割一个就在那一个里头加table
#### 九：/* 媒体查询（应用响应式首页）

：根据当前设备分辨率来控制某一部分样式是否起作用 */

	/* 阀值 */
	/* min-width max-width(小于等于)
		@media screen and (max-width:1280px){
			.box{
				width: 900px;
			}
			.item{
				width: 33.3333%;
			}
		} 
		@media screen and (max-width:960px){
			.box{
				width: 600px;
			}
			.item{
				width: 50%;
			}
		}
		@media screen and (max-width:640px){
			.box{
				width: 300px;
			}
			.item{
				width: 100%;
			}
		}
		注意优先级，如果.box写下面的话所有的宽都是1200，min-width一定要从小往大写，max-width一定要从大往小写
		*{
			box-sizing: border-box; 
		}
		.box{
			width: 1200px;
			height: auto;
			background-color: red;
			margin: 0 auto;
		}
		
		.item{
			width:50%;
			background-color: yellow;
			float: left;
			text-align: center;
			line-height: 300px;
			color: #fff;
			border: 10px solid #fff;
			padding-top: 25%;/* 导致不能加内容，可以定位添加 */
			
		}
		/* .item:nth-child(2){
			background-color: green;
		}  */
		/* 媒体查询：根据当前设备分辨率来控制某一部分样式是否起作用 */
		/* 阀值 */
		/* min-width max-width(小于等于)
		@media screen and (max-width:1040px){
			.box{
				width: 100%;
			}
		} */
		@media screen and (max-width:1200px){
			.box{
				width: 1000px;
			}
			.item{
				width: 50%;
			}
		} 
		@media screen and (max-width:1080px){
			.box{
				width: 600px;
			}
			.item{
				width: 100%;
				padding-top: 50%;
			}
		}
		
		</style>
	</head>
	<body>
	<div class="box">
		<div class="item"></div>
		<div class="item"></div>
		<div class="item"></div>
		<div class="item"></div>
	</div>		
	</body>
	</html>
#### 十：定义一个动画：

@keyframes rotate{

​	0%{

​		 rotate:(0deg);}

​	}100%{

​		 rotate:(360deg);

​	}

}

div{

​	animation-name:rotate;动画名字

​	animation-name:rotate;定义时间

​	animation-time-function:linear;匀速

​	animation-delay:1s;间隔时间

​	animation-iteration-count:infinite;重复次数，无数次

​	animation-direction:alternate;方向，正方向转完反方向转，交叉循环

​	animation-fill-mode;forwards; 当动画完成后，保持最后一个属性值

​	animation-play-state:paused;暂停

}