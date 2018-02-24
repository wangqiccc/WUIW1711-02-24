# html

> * Hyper Text markuo language
> * 超文本标记语言  

### 标记/标签

	#### 行标签：

> * 不会独占一行  不能设置宽高    
> * a (href  tittle  target )  span 	i	em	strong	b	time	address	progress

​	

### 块标签：

> * 独占一行     
> * div	h1~h6	p	pre		ul 	li	ol	dl	dt	dd	footer header main section   form

	### 行内块标签

> * 不会独占一行  也可以设置宽高
> * img（src    alt   width   height   border） input  textarea   select  option  fieldset

### 实体

> * &nbsp ;  &lt ;  &gt ; &amp ;  &quot ;

### 表单

* form(action(在提交表单时执行的动作)	method(在提交表单时所用的 HTTP 方法))

* 表单控件

  > * input(表单控件)(text(文本框)	password(密码框)	radio(单选按钮)	checkbox(多选按钮)	file(文件上传框)	hidden(隐藏域)	submit(提交按钮) 		reset(重置按钮) 	button(普通按钮))（email(用于应该包含电子邮件地址的输入字段)	 url（用于应该包含 URL 地址的输入字段）	date(用于应该包含日期的输入字段)	week(用于应该包含日期的输入字段)	month(用于应该包含日期的输入字段)	time（允许用户选择时间（无时区））	datetime-local(允许用户选择日期和时间（有时区）)	number（ 用于应该包含数字值的输入字段）	range(用于应该包含一定范围内的值的输入字段)	search(用于搜索字段（搜索字段的表现类似常规文本字段）)	color(用于应该包含颜色的输入字段））
  >   * 属性（type(类型)	name(名称)	value(文本框的初始值)		readOnly(规定输入字段为只读)	disable(当 input 元素加载时禁用此元素）	checked	(首次加载时应当被选中)	selected(下拉框) 	maxlength(最多输入的字符数)		required	(指示输入字段的值是必需的)	placeholder(帮助用户填写输入字段的提示)）

# css

### 引用方式

> * 行内样式（style="width:100px" height="100px"）
> * 嵌入样式<style>
>   * .one{width:100px;}<style>
> * 外部样式 link
> * 引入样式
>   * 旧版本 	@import  url("demon.css")
>   * 新版本     @import "demon.css"

### 选择器

> * 标签选择器： 标签名{样式1；}
>
> * 类名选择器：  .类名{样式1；}
>
> * id选择器：     #id名{样式1}
>
> * 后代选择器   父类  子类{样式1}
>
> * 群组选择器：.类名1，.类名2，.类名3{}   用,隔开
>
> * 交叉选择器：	ul.one	.one.two
>
> * UI伪类选择器：
>
>   * :liink	:hover	:active	:vistted
>
> * 子选择器：	div>a	.one>.two
>
> * 统计选择器		div+p(选择p标签，紧挨着div标签)		div~p(选择p标签)
>
> * :nth-child(2)(选择父元素中的第2个子元素)	：first-child	：last-child	:nth-last-child()	only-child
>
> * :nth-of-type(2)(选择父的子元素中同类元素的第2个)		：first-of-type		:last-of-type		：nth-last-of-type()	:only-of-type
>
>   ​			:nth-of-type(2n-1)	（选择奇数的）		:nth-of-type(2n)	（选择偶数的）
>
> * 属性选择器：[data][data=aa] [data^=aa][data$=aa][data*=aa]
>
> * :before	:after
>
> * :checked
>
> * :target	:root
>
> * 通用选择器  *{}

### 属性

> * 布局
>   * width(宽度)	height(高度)	margin(外边距)	padding(内填充)		float(浮动)	position	(定位)	box-sizing(以特定的方式定义匹配某个区域的特定元素)	

### 样式

> * backcground	(背景)	background-image(背景图片)	background-color(背景颜色)	background-repeat(背景平铺)	background-position(背景位置)		background-attachment(背景滚动模式)
> * border(边框)		border-width(边框宽度)		border-color(边框颜色)		border-style(边框样式)		background-clip(背景裁剪区域)		background-origin(背景绘制区)	background-size(背景大小)		border-image(边框图片)	border-radius(边角半径,给盒子设置圆角)
> * box-shadow	(盒子阴影)		
>   * outline（轮廓线）	outline-offset(轮廓的偏移量)

### 渐变

> - linear-gradient（线性渐变）
> -  repeating-linear-gradient（重复的线性渐变）
> - radial-gradient（径向渐变）
> - repeating-radial-gradient（重复径向渐变）

### 文字

> * font-family(字体类型) 		font-size	(字体大小)	 color(字体颜色)	 font-weight(字体粗细情况)		 font-style(字体样式)	 text-decoration(字体修饰)		 text-align(文字水平对齐方式)	 text-indent(字体缩进)	 	line-height(文字垂直居中)	 word-break(文字换行)		 letter-spacing(字间距)	 vertical-align(垂直对齐)

#### 动画

> * transition(过渡)	
> * transition-property(指定过渡或动态模拟的CSS属性)
> * transition-duration(指定完成过渡所需的时间)
> * transition-timing-fuction(规定动画的速度曲线)	
> * transition-delay(指定开始出现的延迟时间)
> * @keyframes(规定动画)		
> * animation(所有动画属性的简写属性)
> * animation-name(规定 @keyframes 动画的名称)
> * animation-iteration-count(规定动画被播放的次数)
> * animation-direction(规定动画是否在下一周期逆向地播放)
> * animation-fill-mode(规定对象动画时间之外的状态)

### 转换

> * transform(向元素应用 2D 或 3D 转换)	transform-origin(允许你改变被转换元素的位置)		perspective(规定 3D 元素的透视效果)		transform-style(规定被嵌套元素如何在 3D 空间中显示)		perspective-origin(规定 3D 元素的底部位置)
> * translate(平移)	translateX(定义转换，只是用 X 轴的值)	translateY(定义转换，只是用 Y 轴的值)	translateZ(定义 3D 转换，只是用 Z 轴的值)	translate3d()	(定义 3D 缩放转换)
> * rotate(定义 2D 旋转，在参数中规定角度)	rotateX(定义沿着 X 轴的 3D 旋转)		rotateY(定义沿着 Y 轴的 3D 旋转)		rotateZ(定义沿着 Z 轴的 3D 旋转)
> * scale(定义 2D 缩放转换)	scaleX(通过设置 X 轴的值来定义缩放转换)		scaleY(通过设置 Y 轴的值来定义缩放转换)
> * skew(定义沿着 X 和 Y 轴的 2D 倾斜转换)	skewX(定义沿着 X 轴的 2D 倾斜转换)		skewY(定义沿着 Y 轴的 2D 倾斜转换)
> * matrix(定义 2D 转换，使用六个值的矩阵)