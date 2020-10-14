Transitions
Transition is a CSS animation in its simplest form. It gives us the ability to declare simple animations for events such as :focus, :hover, :active, :target etc.

Syntax wise, it consists of 4 properties: transition-property, transition-duration, transition-timing-function and transition-delay, and the first three are the most commonly used ones.
transition: [transition-property] [transition-duration] [transition-timing-function] [transition-delay]
To make sure our transitions work everywhere, we should use the following vendor prefixes as usual: -webkit-, -moz-, -o-.

Transition property
Simply put, transition property tells the browser what CSS property to animate. You can name one CSS property per transition, or you can use “all”.

Note: Some of the CSS properties can’t be animated, but here’s the list which you can animate:

    background-color, background-position, border-color, border-width, border-spacing, bottom, clip, color, crop, font-size, font-weight, height, left, letter-spacing, line-height, margin, max-height, max-width, min-height, min-width, opacity, outline-color, outline-offset, outline-width, padding, right, text-indent, text-shadow, top, vertical-align, visibility, width, word-spacing, z-index

There’s a quite of lot of them, and in most scenarios you will use only a few CSS properties.

Transition duration
Transition duration tells the browser the duration for which the transition should roll. You can use milliseconds(ms) or seconds(s).

Transition timing function
On to a little more complicated property. Transition timing function tells the browser the style of the animation. The most used properties are: linear, ease-in, ease-out, ease-in-out and cubic-bezier

Transition delay
This tells the browser how long it should wait before it runs the animation. As usual, it accepts milliseconds and seconds, same as transition-duration.

Transition shorthand
transition: left 200ms ease-in-out, top 300ms ease-in-out

Animation
If you want to create more complicated animations, you will likely have to use a CSS property called animation. This property gives us the ability to declare custom animations with as many CSS properties as we want.

To use animation property, we first need to define an animation by name using the @keyframes property, where we define what the object is supposed to look like at what time. 0% is the snapshot when the animation just starts, and 100% is the snapshot when the animation ends. Thus, keyframes give us the ability to declare custom animations on a timeline, going from 0% to 100%.

Suppose we want to define a fade-in animation. We will call it fadeIn:

@keyframes fadeIn{
0%{
opacity: 0;
}

100%{
opacity: 1;
}
}
This way we declared that when we activate the animation, the element should have opacity: 0 (i.e., invisible), and after some time (when it comes to 100%) it will become visible via opacity: 1.

Animation name
Here we pass name of the animation we created using @keyframes; in this case it’s fadeIn.

Animation delay
animation-delay declares the time to wait before the animation is run. It is very similar to the transition-delay.

Animation iteration count
animation-iteration-count declares what should happen with animation after it ends. Usually, it’s used to declare if animation should go infinite times (i.e., just keep looping) after it’s activated.

Animation Shorthand
animation: fadeIn 200ms infinite

A note on compatibility
Again, it's recommended to use vendor prefixes as usual:
-webkit-animation: fadeIn 200ms
-o-animation: fadeIn 200ms
-moz-animation: fadeIn 200ms
animation: fadeIn 200ms
