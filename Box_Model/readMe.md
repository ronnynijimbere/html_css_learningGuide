What’s the Box Model?

The Box Model is the invisible box that outlines each element on a web page. Each box has a height and width, borders, margins, and padding. You can change these properties to create different effects.

Every element is a rectangle, stacked up on the page. Even round elements have an invisible rectangle around them.

Once you understand that each element is a box, you can learn to create complex styles and layouts on your web page. Let’s look at the properties of boxes.

The Display Property
One of the most important properties is the display property. This property determines what type of box an element is.
Some elements are block elements by default. These elements take up all the available width around them. They can’t sit next to another element, so they all take up their own line.

Most elements are block elements. These include headings, paragraphs, sections, divs, and images.

Inline elements include text, buttons, anchor tags, links, and span elements. You can’t change the height or width of an inline element, just like you can’t change the height or width of a printed word. You can, however, add margins, padding, and borders, which we’ll look at later.

There is one more display type that will come in handy when making websites. This third type is called inline-block, and it’s the perfect blend of both block and inline. You can change the height and width of an inline-block element, but it will only take up its own space, allowing other elements to sit next to it.

The final option for the display property is to hide the element completely by setting it to none. This will hide the element and delete the space that it takes up. Everything inside the element will also disappear. (It’s still there in the code, but it’s hidden.)

===============================================================
Adding Borders
All boxes have invisible borders that line the edges of an element. Even round elements have rectangular borders.

# You can change the appearance of any element’s border by manipulating the border property.

Adding Margins and Padding
Margins and padding add space within and between elements.
Margins add space outside of an element’s borders. This creates space between elements. (For example, adding space between two paragraphs.)

You can add a margin to all sides equally, or set different margins on each side. The following example will add a 12px margin on all sides of the element.

Padding adds extra space between the borders of an element and its contents. For example, if you create a text box with a black border, you can add padding to keep the text from touching the border.

Calculating the Width of a Box
If you set the width of a box to 400px, then add 20px of padding, 20px of margin and a 1px border to all sides, the box’s width will be 482px, not 400px.

Why? Because the extra space and borders on the left and right of the box are added to the width.

It's important to keep the margin, padding, and border in mind when you write your code.

We mentioned that margin and padding add to the width of an element. But sometimes you’ll want to keep a box at a certain width no matter the margin, padding, and border.
