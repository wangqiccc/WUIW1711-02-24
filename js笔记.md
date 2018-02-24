#### 1、webstorm,相当于sublim，功能更强大，文件后缀名为.md，

#### 2、html:Hyper Text Mark Language的简称，即超文本标记语言

#### 3、行标签：

​		本身不会独占一行、不能设置宽高，eg:a （href\title\target）、span、i、em、b、strong、form

   		  H5中新增的：addrss、 progress

#### 4、块标签:

​			独占一行，可以设置大小;eg:div、h1-h6、 p、 pre、 ul、 il、 ol、 dl、 dt、 dd、

​      			H5中新增的：footer、 section、 main、 video 、audio

#### 5、行内块级标签：

​				不会独占一行，可以设置大小；img(src alt width height border)、input、textarea、 select  

​				H5新增的：email url date week month time datetime-local number range search color

​				属性:(type name v alue readonly disable checked selected maxlength);验证(required placeholder)

#### 6、引用方式：

​			行内样式 style="width:100px;height:100px;"

​                          嵌入样式 <style>.h1{width:100px;height:100px;}</style>

#### 			外部样式 <link rel='stylesheet' href="">

​			引入样式 @import url("demo.css");  @import "demo.css"

#### 7、选择器：  

​			标签选择器   div body  a

​			类名选择器   .one

​			id选择器        #one

​			后代选择器    .one  .h1

​			群组选择器    .one,.two

​			交叉选择器    ul.one    .one.two		

​			UI伪类选择器  :link     :hover鼠标选中的效果   :active鼠标按下的效果；:visited访问过；

​			子选择器        div>a   .one>.two    意思是选中前一个元素的子

​			同级选择器    div+p ;p紧挨着div       div~p;p前边有div即可

​			：nth-child()            :first-child   :last-child  :nth-last-child(倒数的个数) -（倒数第几个）  only-child 父元素中唯一的子元素

​			：nth-of-type()        : first-of-type    ：last-of-type   ：nth-of-type      only-of-type同类型中的唯一一个此类元素

​			属性选择器    [data]

​						[data==aa]

​						[data^=aa]

​						[data4=aa]

​						[data*=aa]

​			:before     :after

​			:checked    某一个被选中的选项

​			：target     :root

#### 8、属性：

​		布局 ：宽：width；高：height  外边距：margin  内边距：padding  浮动：float  定位：position  左边距离：left  上边距离：top 右边距离：right 下边距离：bottom 层级:z-index  内容绘制区域:box-sizing   排列方式：display  

​		样式(背景和边框)： 背景：background    背景图片：background-image   背景颜色：background-color 背景平铺：background-repeat  背景位置：background-position  

​           背景图是否跟着内容滚动：background-attachment   

​	   边框： border  

​           边框的宽：border-width  

​	   边框的样式：border-style   

​           边框的颜色：border-color     

​           背景裁剪区域：background-clip  

​           背景起始位置：background-origin    				

​            背景的大小：background-size   

​            设置圆角矩形：border-radius  

​            阴影：box-shadow 

​            轮廓线：outline,（不占位位置。只是效果 ）

​            轮廓线偏移：outline-offset

​             边框设置背景图片：border-image...



border-radius:10px/20px;    10px 20px;     10px 20px 30px 40px/20px 30px 40px 50px;

outline-offset:20px; 即为向外扩展20px;

#### 9、渐变： 

​		线性渐变： linear-gradient()  

​                线性渐变中重复渐变：repeating-linear-gradient()     

​                径向渐变：radial-gradient()    

​                径向渐变中重复渐变：repeating-radial-gradient()

#### 10、文字处理样式：

​		字体类型：font-family；

​                字体大小：font-size;

​                字体粗细：font-weight;  

​                字体样式：font-style; 

​                文本装饰：text-decoration; 

​               文本水平居中： text-align;  

​                文本首行缩进：text-indent;

​                文本垂直居中： line-height;

​                 强制换行： word-break; 

​                字间距： lettter-spacing;  

​                垂直对齐：vertical-align;

#### 11、动画的实现：

​				1)、过渡的属性 ： transition  transtion-property ；

​				       持续的时间：transition-duration；

​                                       过渡效果的时间曲线：transtion-timing-function        

​                                       动画延迟的时间：transtion-delay

​                                2）、@keyframe     animation

#### 12、转换：

​		转换：transform    

​                转换元素的位置：transform-origin     

​               元素被查看位置的角度：perspective   

​		元素的基数位置：perspective-origin

​                转换的子元素保留 3D 转换：transform-style  

​		平移：translate   

​                X位置平移：translate X    

​                Y方向平移：translate Y  

​                Z方向平移：translate Z   

​               3个方向平移： translate 3d()

​              旋转： rotate()   

​              X方向旋转：rotateX()    

​              Y方向旋转：rotateY()    

​              Z方向旋转：rotateZ()     

​              3D旋转：rotate3d()

​	     放大/缩小：scale()    

​             X方向放大/缩小：scaleX()    

​             Y方向放大/缩小：scaleY()   

​	     斜切：skew()      

​            X方向斜切：skewX()     

​            Y方向斜切： skew Y()

​	    矩阵转换：matrix()  

#### 13、表格

14、Bootstrap

