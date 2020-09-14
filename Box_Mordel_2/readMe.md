Creating a Layout with Floats

There are two ways to create a basic layout by moving elements around the page. One is by floating elements in the page.

To float an element means that you remove it from the flow of the document and let it rest above everything. If you float two block elements you can stack them side by side.

To float an element, give it a float property with a value of either left or right and a width.

The footer is hiding behind the main and aside elements.

This is because when you float elements, they lift up above the other elements and no longer take up any space.

When this happens, you must add something called a clearfix to the element that is surrounding the floating elements.

In this case, the element that contains the main and aside elements is a div with the class name main-content. We need to apply a clearfix to this element to make the footer go to its normal place.

Creating a Layout with Inline-Block
Floating elements often cause problems for a layout. That’s why many people create layouts using inline-block instead.
The aside doesn’t fit next to the main and is falling into the next line:

This is caused by a small space between the two elements in our HTML document.

Since the main and aside elements are on separate lines in the HTML, there is a single space character between them. And since the elements are at 70% and 30% width, there’s no room for any other space between them.

When the tiny space shows up between the main and the aside, the remaining space becomes too small, and the aside falls to the next line. We need to remove the space to fix the layout.

The simplest way to remove this space is to add an empty comment between the elements.

Note: You may notice that the two inline-block elements are not the same size and are aligned at the bottom. Most layouts are aligned at the top, so we will add a property called vertical-align to our CSS.

Vertical-align specifies whether an inline-block element will align at the top, bottom, or middle of its neighboring elements. We can add a vertical-align property with a value of top to fix the layout.
