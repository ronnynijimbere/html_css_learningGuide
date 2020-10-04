How to position elements in CSS

There are two major ways to position elements on a web page — we can pick one method over another based on the page layout and the type of content:

    - The floating technique is used to build the website's layout when naturally flowing content is needed and different elements have to be aligned in response to each other.
    - We can use relative positioning or absolute positioning when the position of elements needs to be more strictly controlled.

How To Use Floats
float is a property that allows you to position elements on a web page next to each other. Float allows elements to interact with each other based on their size and size of their parent elements. It allows the element to be positioned on the left or right or have text wrapped around an image

Restoring the flow of the document
To restore the flow of the document, we apply clear: both to the first element that needs to restore the flow back to normal.

The clearfix technique

The clearfix technique is based on the usage of :before and :after pseudo-elements on the parent element. Using these, we can create hidden elements above and below the parent containing the floats, so that we can Force an Element To Self-Clear its Children. The :before pseudo-element prevents the top margin of child elements from collapsing. The :after pseudo-element prevents the bottom margin of child elements from collapsing and clears the nested floats.

<div class="group">
  <div class="is-floated"></div>
  <div class="is-floated"></div>
  <div class="is-floated"></div>
</div>

.group:after {
content: "";
display: table;
clear: both;
}

You would use this instead of clearing the float with something like <br style="clear: both;" /> at the bottom of the parent (easy to forget, not handleable right in CSS, non-semantic) or using something like overflow: hidden; on the parent (you don't always want to hide overflow).

How To Use the Position Property Effectively

The position property provides more control over an element. It can be used with four values.

1.Static
Elements have the static property by default. Elements will be positioned as coded with default behavior.

2.Relative
With relative positioning, box offset properties can be set. The box offset properties allow an element to be positioned exactly. This property can take the values - top, right, bottom and left. Elements can be set to overlap one another without their positions going in a disarray.

3.Absolute
An element can be set to an absolute position. The element whose absolute position is set will be positioned in relation to the parent element that contains it or the body of the page in case the parent element is not available

4.Fixed
This value allows the element to be placed in a fixed position relative to the browser. The element will always be in that position irrespective of the page being scrolled up or down. This property does not work well with IE6.

How to get a fixed Header or Footer
The position:fixed allows developers to build a fixed header or footer that is static in one part of the page.

How to Manage Stacking Order of Web Page Elements
Elements can be positioned on top of one another. The z-index property allows to manage the order of stacking of elements in a page.
The page elements are positioned upon the z-axis as they appear within the Document Object Model (DOM). Using the z-index property, this order can be changed. Elements can be given z-index values. The element with the highest z-index value will appear on the top regardless of its placement in the DOM. To make it effective, first apply a position value of either relative, absolute, or fixed. Then set the z-index property.
