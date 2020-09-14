Positioning Elements

In this section, you’ll learn how to move an HTML element to a specific location on the page.

For example, you can move a link 10 pixels from the top border of the page and 10 pixels from the left border of the page. This gives you more control than simply using floats or inline-block.

Each HTML element has a property called position and a default value of static. This means that the element shows up where it’s written in the HTML and scrolls along with the document.

If you change the position property, you can unlock more tools to position the element wherever you’d like.

1.Relative Positioning
The first type of positioning is relative positioning. This is unlocked when you set the position property to relative.
eg
.test {
position: relative;
}
A relatively-positioned element can be moved as far as you’d like away from its original position. You can use the properties top, right, bottom, and left to specify how far you’d like to move the element. (Remember, the starting point is its original position.)

2.Absolute Positioning
The second type of positioning is called absolute positioning. This is unlocked when you set the position property to absolute.
An absolutely-positioned element can be positioned anywhere in relation to its closest parent with non-static position. What does that mean?
Since all HTML elements are static by default, an absolutely positioned element will (by default) be positioned relative to the entire page (the body element).

By default this element will be located 100px from the top of the body (the top of the screen), and 100px from the right side of the body (the right side of the screen). You can do the same thing with the left and bottom properties.

However, if this element is inside another box with either relative or absolute position, it will be positioned relative to its parent instead.

3.Fixed Position

The third type of positioning is called fixed positioning. This is unlocked by setting the position property to fixed.
A fixed-position element is placed in relation to the edges of your screen.
This element will be positioned at the bottom-right side of the screen. It will stay “fixed” in the bottom of your screen as you scroll. This type of positioning is really handy for a link or image that you want to keep visible as you scroll down the page.

Using Negative Values
You can also use negative values to move elements with relative, absolute, or fixed position. Let’s see the absolute-positioned element from the previous example, this time with negative values.
