# transform 
>CSS Transform属性允许你旋转，缩放，倾斜或平移给定元素。这是通过修改CSS视觉格式化模型的坐标空间来实现的。  
##  四个常用功能
*  位移 translate
*  缩放 scale
*  旋转 rotate
*  倾斜 skew  
  
>注意: 一般都需要搭配transition(过渡)使用  
     inline元素不支持transform,需转变为block.
1. translate
* translateX(length+px(长度) - percentage(百分比))
* translateY(length+px(长度) - percentage(百分比))
* translate( X,Y  )
* translateZ(length),父容器 perspective:;  
  
注意:translate(-50%,-50%)可以做到绝对定位元素居中
2. scale
* scaleX(number)
* scaleY(number)
* scale(x,y)
注意:不常用,容易变形模糊
3. rotate
默认是:rotateZ 垂直平面旋转
4. skew
* skewX(angle)
* skewY(angle)
4. 组合使用
* transform:scale(0.5) translate(100px,200px);
* transform:none;取消所有.
# transition
> 作用是补充中间帧  
> 过渡可以为一个元素在不同状态之间切换的时候定义不同的过渡效果。比如在不同的伪元素之间切换，像是 :hover，:active 或者通过 JavaScript 实现的状态变化。

## 语法
* transition:属性名 时长 过渡方式 延迟--transition:left 1.5s linear 1s;
* 可以用逗号分隔两个不同属性--transition:left 1.5s,height 2s;
* 可以用all代表所有属性--transition:all .5s;
* 过渡方式:linear  | ease | ease-in | ease-out | ease-in-out | step-start | step-end |
###  注意:不是所有属性都能过渡
* 1. display:none => block 直接消失,无法过渡
* 2. 一般可以用visibility:hidden => visible
* 3. background属性可以过渡
* 4. opacity可以过渡