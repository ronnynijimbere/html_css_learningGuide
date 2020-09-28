1. Use comments to break up the document
   Once you have a lot of styles in a CSS document, it becomes a huge mess of class names and semicolons that is nearly impossible to read.
   To make it easier to go through your CSS document later, you can break up the document into sections or categories, like Base Styles, Text Styles, Backgrounds, etc.
   At the top of each section in your CSS document, you can add a CSS comment to write the title of the section. CSS comments start with /_ and end with _/.

2. Each style gets one line
   To keep the document easy to read, each style should be on a new line.
   Also, make sure to keep all spaces consistent, too. This is a good format to follow.

.style {
property: value;
property: value;
}
Whatever format you choose, make sure to stay consistent throughout the whole document

3. Keep class name format consistent
   Some people prefer to write their class names in camel case (all words squished together, and all words except the first are capitalized).

A class name in camel case looks like this:

<div class="camelCase"></div>

Other people prefer snake case (all words are lowercase and separated by underscores).

A class name in snake case looks like this:

<div class="snake_case"></div>

Other people hyphenate their words like this:

<div class="hyphenated-class"></div>

Whichever you choose, keep it consistent throughout the document.
(For another popular method among more advanced coders, check out the BEM — Block Element Modifier methodology.)

4. Don’t nest lots of selectors
   You learned previously that the more selectors you include, the stronger the style gets.
   A style like this...

#main div p .my-link span {
/_ styles go here _/
}

...is way stronger than this:

.my-link span {
/_ styles go here _/
}
Don’t add lots of selectors unless you really need to. It’s usually enough to use just one class name to define a style.

5. Create classes instead of styling HTML elements directly
   Don’t do this:
   .blog-post h1 {
   font-size: 22px;
   font-family: Helvetica;
   }

Why is this bad? Because you aren’t directly styling the <h1> itself, but all <h1>s that are inside the blog post.
What happens when the <h1> moves outside of the blog post? What happens when you decide to use an <h2> instead of an <h1>? It will lose all styling.
When you restructure your document or try to use the style in another place, it will all fall apart.

To avoid this, simply add a class to the <h1> directly.

<h1 class="blog-post-title">My Title</h1>

CSS:
.blog-post-title {
font-size: 22px;
font-family: Helvetica;
}
Now you can move the title anywhere and even change the element to <h2> or something else, and it will always have the correct style.

6. Keep CSS to a minimum
   You learned about refactoring in the last lesson. You can (and should) refactor any code, including CSS.
   You’ll often use the same styles many times in an HTML document. In that case, try to combine the styles in one class name or group the selectors together to simplify your document.

For example, turn this…

h1 {
color: purple;
font-weight: bold;
}

h2 {
color: purple;
font-weight: bold;
}

...into this:

.emphasized-title {
color: purple;
font-weight: bold;
}

Or list multiple selectors using a comma to separate them.

Turn this…

.blog-post-title {
font-weight: bold;
font-family: Helvetica;
font-size: 22px;
color: #333;
}

.menu-title {
font-weight: bold;
font-family: Helvetica;
font-size: 16px;
color: #333;
}

...into this:

.blog-post-title,

.menu-title {
font-weight: bold;
font-family: Helvetica;
color: #333;
}

.blog-post-title {
font-size: 22px;
}

.menu-title {
font-size: 16px;
}

Notice how the same styles are grouped together, while the different styles are left separate.

Using a comma between class names means AND, so the above means “Elements with a class name of ‘blog-post-title’ AND elements with a class name of ‘menu-title.’

7. Shorten HEX colors
   To save space, you can shorten HEX colors into 3 digits.
   This works if you have a color with the same number repeated 6 times, like #cccccc.
   Just write it as #ccc instead. It means the same thing.

8. Don’t add units when the value is 0
   Whenever you have a property with a value of 0, drop the unit (px, %, em, rem, etc.).
   If the margin-left is 0 pixels, just write 0:

.no-margin {
margin-left: 0;
}

9. Separate base styles from their variations
   Good coders create a base style and then add extra classes for new variations to the style.
   For example, you may want to create a set of buttons for your web page.
   Most web pages have different colored buttons for different functions. For example, you may have a red submit button, a gray cancel button, and a yellow help button.
   To start, make a base button class with all of the styles that are common to each button.

.button {
border-radius: 20px;
margin-top: 5px;
margin-right: 25px;
margin-bottom: 5px;
margin-left: 25px;
font-size: 18px;
}

Then create separate classes for each variation:

.button--submit {
color: #fff;
background-color: red;
}

.button--cancel {
color: #333;
background-color: #ccc;
}

.button--help {
color: #333;
background-color: yellow;
}

Your HTML will look like this:
<button class="button button--submit">Submit</button>
<button class="button button--cancel">Cancel</button>

This makes it easier to maintain your code. Just edit the base style to quickly update all of the buttons, or make tweaks to a specific type of button without affecting the others.

10. Always keep learning
    This is not specific to CSS, but a good coder always makes time to learn new things.
    If you never change your coding style, your work will quickly become outdated!
    Follow web development blogs or Twitter accounts, and take a closer look at the HTML and CSS of web pages you personally like.
    Every day, you can discover new techniques, tricks, and technologies.
