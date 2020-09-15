Adding a Background Color
You can add a background color to any element by using the background-color property.
div {
background-color: #16a085;
padding: 15px;
}

Adding a Background Image
You can use an image as a background by using the background-image property. To use this
property, you must specify the path to the image you want to use.
We can also use a property called background-repeat to specify whether the background image
should repeat across the element or not.
Use repeat to repeat the background in all directions, repeat-x to repeat it horizontally,
repeat-y to repeat it vertically, and no-repeat to display the image only once

Next, you can specify a background-position to specify where the background image should display.
Background-position takes two values: the x-position (or horizontal position) and the y-position
(or vertical position). You can write these in pixels, percents, ems, rems, or keywords like top or center

There is one more helpful property called background-size that you can use to style your background.
Instead of repeating the background image, you may want the background image to scale up to fit the size of the element.
This makes the background-image “cover” the entire element. Parts of the background image may be cut off, but it will completely cover the element, leaving no whitespace.

You can also have the background image fit neatly inside the element without losing any part of the image. This means that it will scale up to as big as it can get without going over the boundary of the element. This is called “contain.” It will leave some whitespace around the image if it’s not exactly the same size as the element.

Adding a Gradient
Besides flat colors and images, you can add a gradient background to your elements.
