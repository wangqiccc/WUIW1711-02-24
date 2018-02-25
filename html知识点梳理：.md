装webstorm/phpstorm



# html知识点梳理：

## 一、html是什么：

Hyper Text	markup Language	超文本标记语言

## 二、标记/标签

行标签：不能独占一行，不能设置宽高。常见的有：a、span、i、em、b、strong、time，H5新增的有：address、progress

块标签:独占一行。常见的有： div、h|p、pre、ul、li、ol、dl、dt、dd、header，H5新增的有：footer、section、main、video、audio

行内块级标签（img、form）：不会独占一行，也可以设置宽高

## 三、实体（html不识别多个空格以及换行）

## 四、表单

form(action method)

### 1.表单控件：

​			input(类型：text password  radio  check box  file  hidden  submit  reset  button)	

​			H5新增的控件类型 ：email url date week month time datetime-local number range search color

### 2.属性：

​			（type name value readOnly disable checked selected maxlength required placeholder ）

## 五、CSS的引用方式

### 1.行内样式

  在style中书写<style="weight:100px;">

### 2.嵌入样式

 <style> .one{weight:100px;}</style>

### 3.外部样式

<link rel='stylesheet' href="">

### 4.引入样式

@import"index.css"   @import url("index.css");

## 六、CSS的选择器

​	1.标签选择器(清除默认样式) div body a

​	2.类名选择器   .one

​	3.id选择器    #one

​	4.后代选择器   ul li 				.one  .two

​	5.群组选择器  .one,.two

​	6.交叉选择器 （无固定格式，将两个合在一起） ul.one  .one.two

​	7.伪类选择器：:link   :hover（鼠标移入效果）  :active（鼠标按下效果）  :visited（访问过的效果）

​	8.子选择器： div>a  .one>.two

​	9.同级选择器 div+p  div~p

​	10. :nth-child():  	first-child :last-child :nth-last-child() :only-child

​	       :nth-of-type(): 	first-of-type  :last-of-type   :nth-last-of-type()  	

​	       :only-of-type（同类型中唯一的）

​	11.属性选择器[date]

​	  [][]	 [date=aa],[date^=aa] ,[date$=aa], [date*=aa]

​	12.:before  :after

​	13.:checked	某一个被选中的选项

​	14.:target  :root

## 七、CSS属性

### 	1.CSS布局

​		wight(宽)	 height（高）	 margin（外边距）	 padding（内边距）	 float（浮动） 	position（定位）		box-	

​		sizing:border-box;（移动端）	diplay(转换)：left   right   top  bottom   z-index

### 	2.CSS样式

#### 	背景background   

​		    背景图background-image	background-repeat是否重复 background-position背景位置  background-attachment背景图是否跟	

​		    着内容滚动  background-clip  裁剪绘制区的背景															      					

​	   	    background-origin   背景起始位置

​		    背景颜色background-color

#### 	边框border

​		    border-weight（边框宽度） border-style（边框样式） border-color（边框颜色） border-image（图像边框）

​		    border-radius （圆角边框）

#### 	阴影box-shadow 	

#### 	轮廓线

​		     outline	在边框即盒子外边，且不占位置	   outline-offset 轮廓线偏移

#### 	渐变（重点）

​		   线性渐变 linear-gradient();

 		  线性渐变中的重复渐变repeating-linear-gradient();    

​	          径向渐变radial-gradient();     

​		  径向渐变中的重复渐变repeating-radial-gradient();    

#### 	文字

​		 font-family（字体类型）

​		 font-size（字体大小）

​		 color（字体颜色）

​		 font-weight（字体粗细）

​		 font-style（字体样式）

​		 text-decoration（文本装饰）

​		 text-align（文本水平居中） 

​		 text-indent（首行缩进）

​		 line-height（垂直居中）

​		 word-break（强制换行）

​		  letter-spacing（字间距）   

​		 vertical-align（垂直对齐）

#### 	动画（重点）transition

​		第一种设置动画

```
		box-shadow:inset  0 10px 20px 5px blue;
		/*2D转换：旋转、平移、斜切、放大缩小*/
		transform:rotate(45deg) translate(0, 100px)skew(0, 30deg) scale(1h,3);
		然后设置动画过渡
		transition: all 10s linear;
```



​	        第二种自定义动画

```
@keyframes donghua{
	0%{
		transform:rotate(0deg);
	}
	100%{
		transform:rotate(360deg);
	}
}
div{
			/*动画名称*/
			animation-name: donghua;
			/*动画时间*/
			animation-duration:5s;
			/*动画速度*/
			animation-timing-function: linear;
			/*动画开始时间*/
			animation-delay:2s;
			/*动画的播放次数*/
			animation-iteration-count:infinite;
			/*下次是否逆向播放*/
			animation-direction:alternate;
			/*动画停留状态*/
			animation-fill-mode:forwards;  
		}
		.div:hover{
			/*当鼠标移入时停止播放*/
			animation-play-state:paused;
		}
```



#### 	转换 transform 

​			转换元素位置transform-origin

​			查看元素时的角度 perspective 

​			转换的子元素保留 3D 转换transform-style 

​			元素的基数位置 perspective-origin

​			平移translate   translateX   translateY   translateZ   translate3d

​			旋转 rotate()    rotateX()    rotateY()    rotateZ()    rotate3d()

​			放大缩小scale()   scaleX()   scaleY()

​			斜切skew()   skewX()   skewY()

​			矩阵matrix()

## 八、表格

 border-collapse:collapse;合并边界

text-align: left  right  center;文本水平对齐

vertical-align:top  bottom center;文本垂直对齐







# 新知识

## 响应式布局

响应式布局设计，是指将桌面设备上的网页内容在移动设备上进行优化排版，使用户能够在移动设备上更方便地阅读并操作。

流布局