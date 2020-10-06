Common Selectors
Type selector identifies an element based on its type — i.e., how it is declared within the HTML:
body {
width: 100%;
}

Class selector identifies an element based on its class attribute value:
.wide-button {
width: 120px;
}

ID selector identifies an element based on its ID attribute value. It can be used once per page:
#homepage-hero-image{
width: auto
}

Child Selectors
Child selectors enable selecting of child elements of an element. Child selectors can be of two types: Descendant Selector and Direct Child Selector:

Descendant Selector
This selects all child elements (not just direct children) that are descendants at different levels of the parent element. For example,

p strong {
font-weight: 400;
}
This will apply the rule: "set font-weight to 400" to all strong elements that are descendants of any p element.

Direct Child Selector
If the styling has to be applied only to direct children of a parent element, then the direct child selector should be used. The direct child selector is indicated by placing a greater than sign (>), between the parent element and the child element within the selector

Sibling Selectors
Sibling elements are elements that have a common parent. Sibling elements can be selected using General Sibling selectors or Adjacent Sibling selectors:

General Sibling Selector
It lets you select elements that have a common parent. Sibling elements are created using the tilde character (~) between them within a selector. It matches the second element only if it follows the first element (though not necessarily immediately), and both are children of the same parent

Adjacent Sibling Selector
The adjacent sibling selector is used when an element directly following after another sibling element is to be selected. A plus character (+) between the two elements is used to identify adjacent siblings. The first element identifies what the second element shall follow. The elements must share the same parent. Using the same example as before:

p + h1 {
color: blue;
}

Attribute Present Selector

This identifies an element based on whether an attribute is included or not. Include the attribute in square brackets to select an element if the attribute is present.

Attribute Equals Selector
To identify an element with specific values, the Attribute Equals Selector can be used. Add the attribute and desired value in the square brackets separated with an = to select elements based on this logic. So,

a[target="_blank"] {
background-color: yellow;  
}

Attribute Contains Selector
To select an element based on part of an attribute value, use the asterisk character (\*) before the =. It should be added just after the attribute name within the square brackets.

a[target*="bla"] {
background-color: yellow;  
}

Attribute Begins With Selector
You can select an element based on what an attribute value begins with using a circumflex accent (^) with the attribute name within square brackets. It should be placed before the '=' sign.

a[target^="_bla"] {
background-color: yellow;  
}

Attribute Ends With Selector
You can use the dollar sign (\$) within the square brackets of a selector between the attribute name and equals sign to find for elements that have attributes that end with a certain value.

a[target$="lank"] {
background-color: yellow;  
}

Pseudo-classes
Pseudo classes are classes that are dynamically populated due to user actions or document structure.

Link Pseudo-classes
The :link pseudo-class is used to style an anchor element which has not been visited. The :visited pseudo-class styles links that a user has already visited based on their browsing history.Pseudo classes are classes that are dynamically populated due to user actions or document structure.

User Action Pseudo-classes
These pseudo-classes can be dynamically applied to an element based on action of user.

a:hover {…} is applied to an element when a user moves the cursor over the element.
a:active {…} is applied to an element when a user acts on an element like a click or a selection.
a:focus {…} is applied to an element when the element is currently selected to receive input from input devices.

User Interface State Pseudo-classes
These classes are generated based on state of UI elements.
input:enabled {…} selects the input elements that are enabled by default.
input:disabled {…} selects input elements that are disabled.
input:checked {…} selects checkboxes or radio buttons that are selected.
input:indeterminate {…} selects checkboxes and radio buttons that are neither selected nor unselected.

Structural & Position Pseudo-classes
These pseudo classes are based on where the elements are positioned in the document tree.

The :first-child pseudo-class is used to select an element that is the first child within its parent.
The :last-child pseudo-class is used to select an element that is the last element within its parent.
The :only-child pseudo-class is to select an element that is the only child element within a parent.

:first-of-type will select the first element of its type within a parent.
:last-of-type will select the last element of its type within a parent.
:only-of-type will select the element that is only of the type within a parent.
:nth-child(n) & :nth-last-child(n)

Pseudo-elements

Pseudo-elements are used to style specific parts of an element. They are not part of the document tree. They can be used to style the first letter or part of an element.

Textual Pseudo-elements

:first-letter selects the first letter of text within an element.

:first-line selects the first line of text within an element.
Generated Content Pseudo-elements

:before creates a pseudo-element before, or in front of the selected element

:after creates a pseudo-element after, or behind the selected element.

You will actually find yourself using :before and :after very often — much more frequently than other pseudo elements.
Fragment Pseudo-element

::selection selects part of the document that has been selected, or highlighted, by a users’ actions. The selection can be stylized using the color, background, background-color, and text-shadow properties. If you select something on Commonlounge, the selection color is a lighter shade of blue. This is achieved by the following:

.post{
::selection {
background: aliceblue;
}
}
