//定义响应式样式
@media only screen and (min-width:640px) and (max-width:980px){    }

// -moz-, -webkit-
@keyframes animation_name{
    0% {}
    50% {}
    100% {}
}

.class_name{animation:animation_name 1s ease-in 3s backwards;}

    <' animation-name '>： 检索或设置对象所应用的动画名称 
    <' animation-duration '>： 检索或设置对象动画的持续时间 
    <' animation-timing-function '>： 检索或设置对象动画的过渡类型 
    <' animation-delay '>： 检索或设置对象动画延迟的时间 
    <' animation-iteration-count '>： 检索或设置对象动画的循环次数 
    <' animation-direction '>： 检索或设置对象动画在循环中是否反向运动 
    <' animation-fill-mode '>： 检索或设置对象动画时间之外的状态 
    <' animation-play-state '>： 检索或设置对象动画的状态。w3c正考虑是否将该属性移除，因为动画的状态可以通过其它的方式实现，比如重设样式 

.class_name{
    background:linear-gradient([ [ <angle> | to <side-or-corner> ] ,]? <color-stop>[, <color-stop>]+);
}

语法：
<linear-gradient> = linear-gradient([ [ <angle> | to <side-or-corner> ] ,]? <color-stop>[, <color-stop>]+)
<side-or-corner> = [left | right] || [top | bottom]
<color-stop> = <color> [ <length> | <percentage> ]?
取值：
下述值用来表示渐变的方向，可以使用角度或者关键字来设置：
<angle>： 用角度值指定渐变的方向（或角度）。 
to left： 设置渐变为从右到左。相当于: 270deg 
to right： 设置渐变从左到右。相当于: 90deg 
to top： 设置渐变从下到上。相当于: 0deg 
to bottom： 设置渐变从上到下。相当于: 180deg。这是默认值，等同于留空不写。 <color-stop> 用于指定渐变的起止颜色：
<color>： 指定颜色。 
<length>： 用长度值指定起止色位置。不允许负值 
<percentage>： 用百分比指定起止色位置。 



语法：
<radial-gradient> = radial-gradient([ [ <shape> || <size> ] [ at <position> ]? , | at <position>, ]?<color-stop>[ , <color-stop> ]+)
<position> = [ <length>① | <percentage>① | left | center① | right ]? [ <length>② | <percentage>② | top | center② | bottom ]?
<shape> = circle | ellipse
<size> = <extent-keyword> | [ <circle-size> || <ellipse-size> ]
<extent-keyword> = closest-side | closest-corner | farthest-side | farthest-corner
<circle-size> = <length>
<ellipse-size> = [ <length> | <percentage> ]{2}
<shape-size> = <length> | <percentage>
<color-stop> = <color> [ <length> | <percentage> ]?
取值：
<position> 确定圆心的位置。如果提供2个参数，第一个表示横坐标，第二个表示纵坐标；如果只提供一个，第二值默认为50%，即center
    <percentage>①： 用百分比指定径向渐变圆心的横坐标值。可以为负值。 
    <length>①： 用长度值指定径向渐变圆心的横坐标值。可以为负值。 
    left： 设置左边为径向渐变圆心的横坐标值。 
    center①： 设置中间为径向渐变圆心的横坐标值。 
    right： 设置右边为径向渐变圆心的横坐标值。 
    <percentage>②： 用百分比指定径向渐变圆心的纵坐标值。可以为负值。 
    <length>②： 用长度值指定径向渐变圆心的纵坐标值。可以为负值。 
    top： 设置顶部为径向渐变圆心的纵坐标值。 
    center②： 设置中间为径向渐变圆心的纵坐标值。 
    bottom： 设置底部为径向渐变圆心的纵坐标值。 

<shape> 确定圆的类型
    circle： 指定圆形的径向渐变 
    ellipse： 指定椭圆形的径向渐变。 
<extent-keyword> circle | ellipse 都接受该值作为 size
    closest-side： 指定径向渐变的半径长度为从圆心到离圆心最近的边 
    closest-corner： 指定径向渐变的半径长度为从圆心到离圆心最近的角 
    farthest-side： 指定径向渐变的半径长度为从圆心到离圆心最远的边 
    farthest-corner： 指定径向渐变的半径长度为从圆心到离圆心最远的角 
<circle-size> circle 接受该值作为 size
    <length>： 用长度值指定正圆径向渐变的半径长度。不允许负值。 
<ellipse-size> ellipse 接受该值作为 size
    <length>： 用长度值指定椭圆径向渐变的横向或纵向半径长度。不允许负值。 
    <percentage>： 用百分比指定椭圆径向渐变的横向或纵向半径长度。不允许负值。 
<color-stop> 用于指定渐变的起止颜色：
    <color>： 指定颜色。 
    <length>： 用长度值指定起止色位置。不允许负值 
    <percentage>： 用百分比指定起止色位置。不允许负值 

