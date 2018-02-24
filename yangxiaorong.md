# WUIW1711-02-24

# 1.html

#  

> > *后根文字为列表标签、#后跟文字一级标签。##二级标签，以此类推、>是注释、
> >
> > 行标签：不会独占一行，不能设置宽高，a span i  em  b  strong  time address progress 
> >
> > 块标签：独占一行，可以设置宽高 div  h1-h6 pre ul li ol dl dt dd header footer section main video audio 
> >
> > 行内块级标签；不会独占一行，可以设置宽高 img （src alt width height border)   input textatea select  option fieldest

## 实体：

​      &nbsp ; &lt ;  &gt ;  &quot ; &amp ;

##  

### 表单

- form(action        method  （get/post  （表单的传输方式）））

  ​

- 表单控件

  - input(表单控件)(text(文本框)	password(密码框)	radio(单选按钮)	checkbox(多选按钮)	file(文件上传框)	hidden(隐藏域)	submit(提交按钮) 		reset(重置按钮) 	button(普通按钮))（email(用于应该包含电子邮件地址的输入字段)	 url（用于应该包含 URL 地址的输入字段）	date(用于应该包含日期的输入字段)	week(用于应该包含日期的输入字段)	month(用于应该包含日期的输入字段)	time（允许用户选择时间（无时区））	datetime-local(允许用户选择日期和时间（有时区）)	number（ 用于应该包含数字值的输入字段）	range(用于应该包含一定范围内的值的输入字段)	search(用于搜索字段（搜索字段的表现类似常规文本字段）)	color(用于应该包含颜色的输入字段））
    - 属性（type(类型)	name(名称)	value(文本框的初始值)		readOnly(规定输入字段为只读)	disable(当 input 元素加载时禁用此元素）	checked	(首次加载时应当被选中)	selected(下拉框) 	maxlength(最多输入的字符数)		required	(指示输入字段的值是必需的)	placeholder(帮助用户填写输入字段的提示)）

## 引用方式

- 行内样式 style="width:100px;  height:100px;"

- 嵌入样式<style > .one{}

- 外部样式<link rel='stylesheet' href="">

- 引入样式@import  url("demo.css")或者 @import  "demo.css"

  ## 选择器

  - 标签选择器  div  body    a

  - 类名选择器    .one

  - id选择器  #one

  - 后代选择器  ul li  .one .two

  - 群组选择器  .one,.two

  - 交叉选择器  ul.one  .one.two

  - ui伪类选择器  :hover :link   :active   :visited

  - 子选择器 div >a(表示选择的是前一个元素下的子元素)

  - 同级选择器：div+p(这个表示是在p标签前必须紧挨着div) ;  div~p(这个表示是在p标签前有div标签)

    ：nth-child(2) 如果前面跟值就是所选元素下的第二个元素，如果没有就是整个布局下第二个元素

     :first-child() 如果前面跟值就是所选元素下的第一个元素，如果没有就是整个布局下第一个元素

     :last-child() 如果前面跟值就是所选元素下的第一个元素，如果没有就是整个布局下第一个元素

     :nth-last-child() 

    :only-child整个布局下仅有一个元素的盒子设置属性

    ：nth-of-type(2)  :first-of-type()  :last-of-type()  :nth-last-of-type() :only-of-type

  - 属性选择器 [data ][ data=aa][data=aa][data=aa] [data^=aa][data$=aa][data*=aa]

  - :before  :after

  - :checked    

  - target  :root

    ## 属性

    ### 布局

    - width 宽、 height 高、  ,margin 外边距、   padding 内填充、  float 浮动、	position 位置、  box-sizing以特定的方式定义匹配某个区域的特定元素、diaplay  left right bottom  top    z-index 

### 样式

- background （背景）     background-image （背景图片）    background-color  （背景颜色）     background-repeat  （背景是否重复）     background-position  （背景位置）     background-attachment  （背景滚动模式）    background-clip （背景裁减）     background-origin  （背景开始位置）     background-size （背景尺寸） 

- border （边框） border-width （边框宽度）   border-style（边框样式）   border-color（边框颜色）        border-image（边框图片）  border-radius（（边框四个角的设置、最多设置八个值，/目的是x轴y轴分别设置)

- box-shadow（盒子阴影设置）     outline:1px solid red;(边框外轮廓线，不占位置)    outline-offset：20px;(轮廓的偏移量) 

- background:radial-gradient(circle,red 0,blue 100%, transparent 0);    background-position:left  top,right bottom;(设置镜性渐变、位置颜色）

  ### 文字

  word-break(文字换行)

  vertical-align(文字垂直居中)

  ### 动画

  - transition   transition-property(定义过渡属性)、transition-duration(过渡持续时间)、transition-timing-function (过渡函数) transition-delay(过度延迟时间)

    animation-name: rotate;（定义动画名字）

    animation-duration: 5s;（动画转动时间）

    animation-timing-function: linear;（动画线性旋转）

    animation-delay: 2s;（延迟时间）

    animation-iteration-count: infinite;（一致重复动画）

    animation-direction: alternate;/*正着转一次。反着转一次*/

    animation-fill-mode: backwards; /*停留在开始方向*/

    animation-fill-mode: forwards;/*停留在结束方向*/ 

  @keyframe     animation（定义动画）

### 转换

- transform  transform-origin  perspective （视点）  transform-style  perspective-origin（视点开始位置）

- teanslate  translateX translateY  translateZ translate3d()   （分别沿xyz轴移动）

- rotate()   rotateX()  rotateY()   rotateZ()   rotate3d()   （分别以xyz轴旋转）

- scale()  scaleX( ) scaleY()  （分别以xyz轴缩放）

- skew()    skewX()    skewY()   (倾斜偏移位置)

- matrix()   （矩阵）

  ### 表单拆分组合：

  rowspan:列合并

  cowspan:行合并

  拆分：

  假如想给某一行某一格拆分直接在这一格中加一个table，自己设置大小等