# CSS Transforms, Transitions, and Animations

ways to size, position, and change elements. All of these new techniques are made possible by the transform property. the transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

1. The rotate
      value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. The default point of rotation is the center of the element, 50% 50%, both horizontally and vertically. Later we will discuss how you can change this default point of rotation.

       .box-1 {

         transform: rotate(20deg);
    }
       .box-2 {
        transform: rotate(-55deg);
     }  

2. Scale
Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1, therefore any value between .99 and .01 makes an element appear smaller while any value greater than or equal to 1.01 makes an element appear larger.

3. Translate
The translate value works a bit like that of relative positioning, pushing and pulling an element in different directions without interrupting the normal flow of the document. Using the translateX value will change the position of an element on the horizontal axis while using the translateY value will change the position of an element on the vertical axis.

As with the scale value, to set both the x and y axis values at once, use the translate value and declare the x axis value first, followed by a comma, and then the y axis value.

Transitions
As mentioned, for a transition to take place, an element must have a change in state, and different styles must be identified for each state. The easiest way for determining styles for different states is by using the :hover, :focus, :active, and :target pseudo-classes.

There are four transition related properties in total, including transition-property, transition-duration, transition-timing-function, and transition-delay. Not all of these are required to build a transition, with the first three are the most popular.

       .box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
       }
      .box:hover {
  background: #ff7b29;
       }

Transitional Properties
It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. The display property, for example, may not be transitioned as it does not have any midpoint. A handful of the more popular transitional properties include the following.

`background-colorbackground-positionborder-colorborder-widthborder-spacingbottomclipcolorcropfont-sizefont-weightheightleftletter-spacingline-heightmarginmax-heightmax-widthmin-heightmin-widthopacityoutline-coloroutline-offsetoutline-widthpaddingrighttext-indenttext-shadowtopvertical-alignvisibilitywidthword-spacingz-index`

Transition Duration
The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values may also come in fractional measurements, .2s for example.

for more animated elements visit [this site](https://codepen.io/retyui/pen/ByoaXV)
