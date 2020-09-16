Making lists in HTML is easy if you know how to use the <ol> and <ul> elements. These are two basic types of lists called ordered lists and unordered lists. Ordered lists are numbered lists, while unordered lists are bullet-point lists that don’t follow a certain order (hence the names).

Making Unordered Lists
This is the most common type of list used on the web. This is used for bullet-point lists, lists of links, navigation menus, and much more.
To make an unordered list, you will use the list element <ul> and the list-item element <li>.
By nesting <li> elements inside of a <ul> element, you can make a simple list.

Please note that only <li> elements can be placed directly inside of a <ul> element. Please do not place a <p> or <a> or any other element directly inside a <ul>, However, you can place any content you’d like (<a>, <p>, <div>, etc.) inside an <li> element

You can use attributes to manipulate your ordered lists in many ways.
To start your list from a number other than one, use the start attribute.
To reverse the numbering on a list, use the reversed attribute. This one doesn’t need a value.

Making Description Lists
Another type of list found in HTML is called a description list. This element makes a list of terms and their definitions, much like a dictionary or glossary. This list follows a specific structure: the outer layer is a <dl> (description list), and inside is placed a <dt> (description title) and a <dd> (description data).
As you see above, you can list <dt> and <dd> elements in order inside the <dl> tag. You cannot place anything but <dt> and <dd> directly inside <dl>, but you can place other elements inside of <dt> and <dd>.

Lists Inside Lists
So far, you have learned that you can place other elements inside list items, or description list titles or data. This means that you can nest lists inside of other lists.
For example, to add a secondary bullet-point list inside of an existing unordered list

Styling Lists
You can change the bullet point or numbering style of ordered and unordered lists, using the list-style-type property in CSS.
The default list-style-type for an ordered list is decimal, but you can change it to other numbering styles like upper-roman (uppercase roman numerals) or lower-roman (lowercase roman numerals).

Another way to style an unordered list is to remove the bullet points completely and list them horizontally across the page. You can do this by removing the list-style-type, removing margins and padding, and making the list-item elements inline-block.
