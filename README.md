弹性布局
==============

[参考链接软](http://www.ruanyifeng.com/blog/2015/07/flex-grammar.html "Markdown")


任意一个元素可以指定为flex布局，这元素称为容器，子元素称为项目

容器的属性有
--------------

>1.`flex-direction`: row | row-reverse | column | column-reverse 主轴的方向（项目的排列方向）

>2.`flex-wrap`: nowrap | wrap | wrap-reverse; 默认情况下，项目都排在一条线（又称"轴线"）上。flex-wrap属性定义，如果一条轴线排不下，如何换行。

>3.`flex-flow`:  <flex-direction> || <flex-wrap>;flex-flow属性是flex-direction属性和flex-wrap属性的简写形式，默认值为row nowrap

>4.`justify-content`: flex-start | flex-end | center | space-between | space-around; 在主轴上的方向

>5.`align-items`: flex-start | flex-end | center | baseline | stretch; 在交叉轴上的方向。默认值stretch

>6.`align-content`: flex-start | flex-end | center | space-between | space-around | stretch;多根轴线的对齐方式。如果项目只有一根轴线，该属性不起作用。

项目的属性
-----------------

>1.`order`: 0(默认);定义项目的排列顺序。越小，越靠前。

>2.`flex-grow`: <number>; /* default 0 */属性定义项目的放大比例，默认为0，即如果存在剩余空间，也不放大。如果所有项目的flex-grow属性都为1，则它们将等分剩余空间（如果有的话）。如果一个项目的flex-grow属性为2，其他项目都为1，则前者占据的剩余空间将比其他项多一倍。

>3.`flex-shrink`: <number>; /* default 1 */如果所有项目的flex-shrink属性都为1，当空间不足时，都将等比例缩小。如果一个项目的flex-shrink属性为0，其他项目都为1，则空间不足时，前者不缩小。

>4.`flex-basis`: <length> | auto; /* default auto */ 属性定义了在分配多余空间之前，项目占据的主轴空间（main size）。浏览器根据这个属性，计算主轴是否有多余空间。它的默认值为auto，即项目的本来大小。

>5.`flex`: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ] auto(1 1 auto) none(0 0 auto)缩写

>6.`align-self`: auto | flex-start | flex-end | center | baseline | stretch;align-self属性允许单个项目有与其他项目不一样的对齐方式，可覆盖align-items属性。默认值为auto，表示继承父元素的align-items属性，如果没有父元素，则等同于stretch。

