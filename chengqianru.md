# 总结

## 1.html  :  Hyper Text markup language          超文本标记语言

## 2.标记/标签

#### 1）行标签  

​     不会独占一行，不能设置宽高     ( a、span)

​     a------href 、 title、 target                     span       

​     斜体：i 、em b strong      time   address     

​     进度:progress

#### 2）块标签                  

​    独占一行             

  (div 、h1-h6、 p、 pre 、ul、 li 、ol 、dl 、dt 、dd      header   footer   section  main   播放视频:video  播放音频:audio       form)

#### 3）行内块元素              

​     不会独占一行，可以设置宽高

img (src    alt)                           width 、 height  、border、 input、 textarea  、select   、 option  、fieldset  

## 3.实体

&nbsp;&lt      &gt    &quot     &amp   &nbsp

## 4.表单

#### 1）form  (指定数据的处理文件：action    指定数据提交方式：method)

#### 2）表单控件

input

控件类型(文本字段：text    密码：password    单选按钮：radio   复选框：checkbox    文件域：file    隐藏域：hidden    提交按钮：submit    重置: reset     按钮：button   )

h5新增 ——电子邮件:email     地址:url      日期：date    month    time    week      定义选取时间、日 月、年的输入域(本地时间)：datetime-local       数字：number   定义包含一定范围内数字值的输入域：range       搜索域：search     调色板：color

#### 3）属性

type   name     value     只读-只能看，不能改：readOnly 、disable      checked     selected    maxlength     required       默认文字placeholder

 readOnly与 disabled 的区别

​    1、readOnly 只能看，不能改，但是可以被提交给服务器

​    2、disabled 只能看，不能改，但是不能提交给服务器

## 5.引用方式

#### 1）行内样式                      style="width   height " 

#### 2)  嵌入样式                      <style></style>

#### 3）外部样式                      <link rel='stylesheet'  href="">   

#### 4）引入样式                      @import url("demo.css");         @impor  "demo.css";

### 选择器

####        1）标签选择器                     div      body      a

####  2）类名选择器                     .one

####         3）id 选择器                        #one

####         4）后代选择器                     ul li                            .one    .two

####         5)  群组选择器                      .one,.two

#### 	6)  交叉选择器			ul.one                      .one .two

#### 	7)  UI伪类选择器             	:hover           :active        :visited

#### 	8)  子选择器     			div>a             .one >.two               选择前一个

#### 	9)  同级选择器    			div+p        div-p

#### 	10)  实现条纹效果 :nth-child                   最近执行效果:first-child                      :last-child                            :nth-last-child                     :only-child

​	标签:nth-of-type( )                  :first-of-type                  :last-of-type                     :nth-last-of-type                         :only-of-type 

​        偶数行  :nth-child  （2n）             奇数行 :nth-child  （2n-1）

#### 	11) 属性选择器                     

  [data] 

  [data=aa]        

  [data^=aa]

 [data$=aa]    

  [data*=aa]

：before                    :after                      :checked

锚链接跳转地址       :target                             :root

## 6.属性

### 布局

width   height        margin     padding            float              position              box-sizing              display          left    right     top    bottom     

z-index

### 样式

background           background -img           background -color           background -repeat              background -position

   固定背景位置 ：background -attachment          规定背景的绘制区域：background -clip     background -origin    background -size

border              border-width      border-style       border-color     border-clip     border-origin       border-size       border-image

 border-radius         border-shadow         

多边框 border-shadow：0 0 0 0 2px  #000；0 0 0 0 3px blue；0 0 0 0 2px  pink;



		/背景颜色/
		background-color: red;
		/*背景图*/
		background-image: url('imgs/b.3.jpg');
		/*设置背景图平铺与否
		background-repeat: no-repeat;
		/*背景图大小(长度/百分比/contain）*/
		background-size: 100% 100%;
		background-size: 400px 400px;
		/*(正好包含在内，不变形。等比例出现，覆盖会不完整)*/
		background-size: contain;
		/*覆盖整个盒子，但是会出现图片不完整的现象*/
		background-size: cover;  
		/*图片位置的设置*/
		background-position: left center;
		background-position: 10px 50px;    /*x轴  y轴*/
		/*图片放到那个地方,图片裁剪区域。默认是border区域*/
		background-clip: border-box; 
		background-clip: content-box;
		background-clip: border-box;
		/*设置图片绘制的起始位置,默认是padding区域*/
		background-origin: border-box;
		/*设置背景图是否与内容图滚动而滚动*/
	    background-attachment: fixed;
#### 轮廓线

outline           轮廓线偏移   outline-offset，不占位置

#### 渐变

linear-gradient( )                    重复线性渐变：repeating-linear-gradient( )        radial-gradient (  )        repeating-radial-gradient( )



	    /文本背景颜色在背景图上，图片作为边框/
	    background: linear-gradient(#fff,#fff) padding-box,url('4.jpg') border-box;   /*从边框区域绘制*/ 

		/渐变文字/
		background: linear-gradient(to right,pink,yellow);

#### 文字

font-family      font-size     font-weight    font-style     text-decoration      text-align       text-indent     line-height       word-break

letter-spacing字间距     vertical-align垂直对齐

#### 动画

transition             transition-property 过度属性             transition-duration过度时间                     transition-timing-function过度动画函数

  transition-delay 动画延迟

@keyframe 

	@keyframes rotate {
		0%{
			transform: rotate(0deg);
		}
		100%{
			transform: rotate(180deg);
		}
	}          
animation

			/动画名称/
			animation-name: rotate;
			/*动画过度时间*/
			animation-duration: 5s;
			/*动画匀速执行旋转*/
			animation-timing-function: linear;
			/*动画延迟*/
			animation-delay: 2s;
			/*动画执行次数，2次*/
			animation-iteration-count: 2;
			/*动画执行次数，无数次*/
			animation-iteration-count: infinite;
			/*正反交替转*/
			animation-direction: alternate;
			/*旋转一定角度停止*/
			animation-fill-mode: forwards;
#### 转换

transform                     设置元素的基点转换位置： transform-origin          设置景深以及位置：perspective              让转换的子元素保留3D转换：transform-style             

 设置 3D 元素的基点位置：perspective-origin



	/*2d转换  旋转  平移 斜切  放大缩小（正的是放大，负的是缩小）*/
	transform: rotate(45deg) translate(0,200px) skewX(30deg) scale(1, 1);
	transform: rotate(45deg);



		/设置景深以及位置1000-2000,距离盒子的距离/
		perspective: 1000px;
		perspective-origin: left top;
位移translate                translateX			translateY		   translateZ		            translate3d( ) 		

旋转rotate( )			rotateX( )		        rotateY( )		   rotateZ( )		            rotate3d ( )	

放大缩小scale( )		scaleX( )			        scaleY( )			

斜切skew( )			skewX( )		                skewY( ) 			

)矩阵matrix( )