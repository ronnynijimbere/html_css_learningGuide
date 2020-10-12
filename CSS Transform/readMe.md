The transform property gives us a way to position and alter elements. It comes in two settings: 2-Dimensional and 3-Dimensional. Each of those comes with different settings and properties

Syntax-wise, transform property has multiple sub-properties which declare how the element should be transformed. For instance, in the example above, we used the scale property. But there are a number of these like rotate, translate and skew in addition to scale

2D Transforms
2D transforms work on x-axis and y-axis, while 3D transforms work on x-axis, y-axis, and z-axis.

2D rotate
Takes 1 parameter: the degrees or percentage by which the element should be rotated relative to the x-axis.
transform: rotate(20deg)

2D scale
Takes 1 parameter: the multiple by which the element should be scaled to. scale(2) will make the element twice the original size. scale(0.5) will make it half in size.
transform: scale(0.5)

2D translate
This property is used to translate, or move the element along the X or Y axis. It has multiple sub properties: translateX or translateY
transform: translateX(20px)
transform: translateY(30px)

In addition, you can specify both together with just translate Thus, you can combine the two lines of code above to just:
transform: translate(20px, 30px)

2D skew
This property is used to distort elements on the horizontal axis, vertical axis, or both.
transform: skewX(5deg)
transform: skewY(10deg)

As with translate, you can combine multiple axes with just skew
transform: skew(5deg, 10deg)

Transform origin
Transform origin is the point relative to which the above transforms are applied. The default transform-origin is middle of the element, but you can change that by defining transform-origin yourself. It can take one or two properties, for x-axis or y-axis respectively. These can be percentage, pixels or default values such as top, left, bottom and right).

transform-origin: top left;
transform-origin: 50px 50px;
transform-origin: bottom right 60px;

3D Transforms
3D Transforms are very similar to 2D transforms, except that they take the third z-axis into account as well. Thus, the 2D Transform properties above translate directly to 3D transforms, along with the addition of translateZ and skewZ properties.

Perspective
In order for 3D transforms to work, the elements need a perspective from which the transform takes place. The perspective for each element can be thought of as a vanishing point. 3D transforms are not used very frequently, but if you're curious, you should check out the Perspective documentation at MDN.

Support and Usage
Support-wise, most of the modern browsers support the transform property. It's recommended to use the vendor prefixes on every instance of transform property. So, to make a div 1.5 times the original size, you would write:

div {
-webkit-transform: scale(1.5);
-moz-transform: scale(1.5);
-o-transform: scale(1.5);
transform: scale(1.5);
}

Usage-wise, transform is mainly used in custom animations which are built using @keyframes css property.
