### html(Hyper Text markup language 超文本标记语言)

#### 标签分类：行标签、块标签、行内块级标签

###### 1、行内元素特点：不会独占一行，不能设置宽高

###### 常见的行内元素有：<a>、<span>、<i>、<strong>、<b>、<cite>、<em>、<code>、<samp>、<var>、<site>、

###### <code>、<del>、<ins>、<a>、<time>、<address>、<progress>、<meter>、

###### 2、块级元素特点：独占一行

###### 常见的元素有：div、h1-h6、p、form、header、main、footer、ul、ol、li、dl、dt、dd、video、audio、input、textarea、select、object、option、filedset

###### 3、行内块元素：可设置宽高，不会独占一行

###### 常见的行内块元素有:img、

###### 4、常见的空元素：<br>、<hr>、<img>、<input>、<link>、<meta>、<progress>、<meter>、

### 常见的实体符号：

###### &nbsp; &nbsp; 空格："&nbsp"

######     大于号：&gt；

######     小于号：&lt；

######      引号：&quot；

######      和号：&amp；

######       注册商标：&reg；

######       商标：&trade；

######       乘号 ：&times；

######        除号：&divide；

### 表单

###### form：    提交方式： method：post /get     post较安全

###### action：指定表单的提交地址

###### input的type属性值有：text(文本框)、password(密码框)、radio(文本框)、checkbox(密码框)、file(文本框)、hidden(密码框)、

###### submit(文本框)、reset(密码框)、button(文本框)、email(密码框)、date(文本框)、week(密码框)、month(文本框)、time(密码框)、datetime-local(文本框)、number(密码框)、range(文本框)、search(密码框)、color(文本框)、

###### name:用于后台，一般必须有

###### value：默认值

###### readonly：只读

###### disable：禁用

###### checked

###### selected 

###### maxlength

### CSS的引用方式：

#### 1.行内样式

###### style=“width：20px; height:30px;”

#### 2.嵌入样式：

<style>

###### .one{

###### background-color:red;

###### }

###### </style>

#### 3.外部样式：

###### <link rel=" style/sheet" href="">

#### 4.引入样式：

###### @import( );

### 布局

###### 常见的用于布局的css属性有：width、height、padding、margin、float、position、left、top、bottom、right、

###### display、z-index、box-sizing...

### CSS选择器：

###### 标签选择器    body    div   a

###### 类名选择器    .one

###### id选择器    #one

###### 后代选择器   ul li    .one  .two          选中.one 里的所有.two(儿子、孙子等等都会选中）

###### 子元素选择器  div>p       .one>.two       只选中父元素是div里的p元素（只会选中儿子）

###### 群组选择器  .one,.two

###### 交叉选择器  ul.one     .one.two       p.p1         选中这种元素<p class="p1">f</p>

###### UI伪类选择器：    :hover    选择鼠标在链接上面时

######  				 :linked   选择所有未访问的链接

###### 				 :active    选择激活时的链接样式

###### 				 :visited   选择所有访问过的链接

###### 同级选择器   div+p      (选择所有紧接着div之后的p元素)    

######  div~p          (div与p有相同的父元素，选择所有同级的div之后的p元素)

###### :nth-child()     eg：    p:nth-child(2)		选中每个p元素是其父元素的第二个子元素

###### :first-child      eg:       p:first-child             选中“只有当p元素是其父元素的第一个子集”

###### :last-child  						  选中“只有当p元素是其父元素的最后一个子集”

######  :nth-last-child(倒数)     		    选中“只有当p元素是其父元素的第一个子集”（倒着数的第几个）

###### :only-child(是唯一的子元素)             选中每个p元素是其父元素的唯一子元素

###### :nth-of-type()          eg：  p:nth-of-type(2)		选中每个p元素是其父元素的第二个p元素

###### :first-of-type      eg:       p:first-child             选中“只有当p元素是其父元素的第一个p元素”

###### :last-of-type  						  选中“只有当p元素是其父元素的最后一个p元素”

######  :nth-last-of-type(倒数)     		    选中“只有当p元素是其父元素的第一个p元素”（倒着数的第几个）

###### :only-child(是唯一的子元素)             选中每个p元素是其父元素的唯一p元素

###### :nth-child(2n)    				规定属于其父元素的第2n个子元素

######  :nth-child(2n-1) 				规定属于其父元素的第2n-1个子元素

###### 属性选择器    [data][data=aa]   [data^=aa][data$=aa]   [data*=aa]

###### :before          eg：    p:before {

###### 					content:"this is mine:";

###### 				   }                                  在每个p元素之前插入内容  ;使用content 属性来指定插入的内容 

###### :after               在每个p元素之后插入内容  ;使用content 属性来指定插入的内容 

###### :checked           选择每个选择的输入元素（仅适用于单选按钮radio和复选框checkbox）

###### ::selected          匹配元素中被用户选中或处于高亮状态的部分    

###### :target             设置当前活动的target元素的样式       （例如：当a元素被选中时，可以用它更改选中时所需的样式）

###### :root                设置文档的根元素（在html中，根元素始终是html元素）

### 样式

###### background   border   background-image/color/repeat/position/attachment(fixed)  设置背景图片是随着页面滚动而滚动，还是固定不动的

###### border-width/color/style

###### background-clip/origin/size(cover/contain)

###### border-image-size/

###### border-radius(可设n个值)(10px/20px)--椭圆形的圆角

###### box-shadow(0 0 0 2px #333,0 0 0 2px #333,0 0 0 2px #333)----

###### outline: 1px  solid red;

###### outline-offset: 20px;

###### backgound:可以设置多个背景。

### 渐变

###### linear-gradient()  线性渐变              repeating-linear-gradient() 重复线性渐变     

######  radial-gradient()  径向渐变             repeating-radial-gradient()  重复径向家变

### 文字

###### font-family/size/color/weight/style               color/text-decoration/line-height/text-indent/word-break  /letter-spacing/vertical-align

### 动画

1、transition        transition-property/transition-duration（默认时间为0，所以必须指定时间）/transition-timing-function--函数/transition-delay()

2、@keyframe          animation：animation-name/animation-duration/animation-timing-function/animation-direction/animation-delay/animation-itaration-count(设置动画播放次数)/animation-fill-mode(设置动画当动画停止时，要应用的样式，是保持运动的最后一秒的状态还是回到最初状态)

### 转换

transform    transform-origin   perspective  perspective-origin(转换的基本点)

平移：translateX  /translateY  /translateZ   /translate3d()

旋转：rotate()   rotateX()   rotateY()  rotate3d()

放大、缩小：scale()   scaleX()   scaleY()

斜切：skew()   skewX()     skewY()

matrix()--矩阵

### 应用于表格的特定的两个CSS样式

border-collapse:collapse;         把表格内的两条线合并成1条

table-layout：fixed；         设置表格的布局方式

