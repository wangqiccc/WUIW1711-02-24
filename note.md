# html

> Hype Text markup language 超文本标记语言

## 标记 /标签

### 行标签

> * 不会独占一行
> * 不能设置宽高
> * a (href title target) span i em b strong time address progress

### 块标签

> * 独占一行
> * div h1-h6  p pre ul li ol dl dt dd header footer section main video audio form

### 行内块标签

> * 不会独占一行，可以设置宽高
> * img(src alt width height border) input textarea select option fieldset 

## 实体

* &nbsp；&lt；&gt；

## 表单

* form(action（在提交表单时执行的动作） method（在提交表单时所用的 HTTP 方法）)
* 表单控件
  * 类型(text（常规文本） password（密码） radio（单选按钮） checkbox（复选框） file（文件上传框） hidden（隐藏域） submit（提交按钮） reset（复位按钮） button（普通按钮）) (email（用于应该包含电子邮件地址的输入字段） url（用于应该包含 URL 地址的输入字段） date（用于应该包含日期的输入字段） week（允许用户选择周和年） month（允许用户选择月份和年份） time（允许用户选择时间（无时区）） datetime-local（允许用户选择日期和时间（有时区）） number（ 用于应该包含数字值的输入字段） range（用于应该包含一定范围内的值的输入字段） search（用于搜索字段（搜索字段的表现类似常规文本字段））color（用于应该包含颜色的输入字段）)
* 属性(type(类型) name（名称） value（文本框的初始值） readOnly （规定输入字段为只读）disable（当 input 元素加载时禁用此元素） checked（首次加载时应当被选中） selected（下拉框） maxlength（最多输入的字符数）) (required（指示输入字段的值是必需的） placeholder（帮助用户填写输入字段的提示）) 

# css

## 引用方式

* 行内样式(style="width:100px;height:500px;")
* 嵌入样式<style>.one{width:100px;}</style>
* 外部样式<link rel='stylesheet' href="">
* 引入样式@import url("demo.css");  @import "demon.css"

## 选择器

* 标签选择器 div body a
* 类名选择器 .one
* id选择器 #one
* 后代选择器 ul li 
* 群组选择器 .one,.two
* 交叉选择器 ul.one .one.two
* UI伪类选择器:link :hover :active :visited
* 子选择器 div>a .one> .two
* 同级选择器 div+p div~p
* :nth-child :first-child :last-child :nth-last-child() :only-child 父元素中的子元素
* :nth-of-type :last-of-type  :nth-last-of-type() :only-of-type 父元素中同类型的子元素
* 属性选择器 [data][data=aa] [data^=aa][data$=aa] [data=*aa]
* :before :after
* :checked
* :target :root

## 属性

### 布局

* width（宽度） height（高度） margin（外边距） padding（内填充）float （浮动）position（定位） box-sizing（以特定的方式定义匹配某个区域的特定元素） display（规定元素应该生成的框的类型） left（左） right（右） top（上） bottom（下） z-index（设置元素的堆叠顺序）

### 样式

* background（背景） background-image（背景图） background-color（背景颜色） background-repeat（重复背景图像） background-position（背景图像的位置） background-attachment（背景图像是否固定或者随着页面的其余部分滚动） border（边框） border-width（边框宽度） border-style（边框样式） border-color（边框颜色） background-clip（背景的绘制区域） background-origin（背景图片的定位区域） background-size（背景图片的尺寸） boder-radius（边框圆角）（具备8个值） border-image（边框背景） box-shadow（阴影） outline(轮廓线) outline-offset（轮廓线的偏移）

### 渐变

* linear-gradient（线性渐变） repeating-linear-gradient（重复的线性渐变）radial-gradient（径向渐变）repeating-radial-gradient（重复径向渐变）

### 文字

* font-family（字体类型） font-size（字体大小） color（字体颜色） font-weight（字体粗细） font-style(字体样式) text-decoration（文本修饰） text-align（水平对齐方式） text-indent（首行缩进） line-height（行间距）word-break（换行） letter-spacing（字间距） vertical-align（垂直对齐）

### 动画

* transition（过渡） transition-property（设置过渡效果的 CSS 属性的名称） transition-duration（完成过渡效果需要多少秒或毫秒） transition-time-function（规定速度效果的速度曲线） transition-delay（定义过渡效果何时开始）
* @keyframe animation

### 转换

* transform（向元素应用2D或3D转换） transform-origin（改变被转换元素的位置） perspective（为 3D 转换元素定义透视视图） transform-style（被嵌套元素在3D空间中显示） perspective-origin （3D元素的底部位置）
* translate（2D平移） translateX（沿x轴平移） translateY（沿y轴平移） translateZ（沿z轴平移） translate3d（3D平移）rotate（2D 旋转）rotateX（沿x轴旋转） rotateY （沿y轴旋转）rotateZ（沿z轴旋转） rotate 3d（3D旋转）scale（2D 缩放转换）scaleX（设置 X 轴的值来定义缩放转换） scaleY （设置y 轴的值来定义缩放转换） skew（沿着 X 和 Y 轴的 2D 倾斜转换）skewX（沿着 X 轴的 2D 倾斜转换）skewY（沿着 Y 轴的 2D 倾斜转换）matrix（ 2D 转换，使用六个值的矩阵）

# 表格

<table width="" height="" border="" cellspacing="(边框与边框的距离)" align="" bgcolor="">

​	<caption>标题</caption>

​	<thead></thead>

​	<tbody></tbody>

​	<tfoot><tfoot>

​	<tr height="" align="" valign="(垂直方向)" bgcolor="">

​		<th>标题</th>

​		<td></td>

​	<tr>

* table-layout:fixed;
* border-collapse:collapse;
* word-break:break-all;
* colspan合并行单元格
* rowspan和并列单元格

# 媒体查询(响应式布局基本原理)

> 根据当前设备的分辨率来控制某一部分样式是否显示

@media  screen and (max-width:1040px){

​	.box{

​		width:100%;

​	}

}

> 阀值（临界值）min-width、max-width

# 动画

animation-name:动画名; animation-duration:动画时间; animation-timing-function:动画速度; animation-delay:间隔时间; animation-iteration-count:重复次数（infinite无限）; animation-direction:方向（alternate交叉循环）; animation-fill-mode:forwards转完停住（backwards）; animation-play-state:paused（鼠标经过暂停）;