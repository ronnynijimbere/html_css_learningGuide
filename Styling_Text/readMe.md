Changing Font

You can specify the font with the font-family property.
the web developer specifies Helvetica as the font. But if the Helvetica isn’t available, Arial will be displayed.

Changing Size
You can change font size with the font-size property.
You can also use % to change text size. In this case, the size of an element will be a % of its parent.
html {
font-size: 16px;
}

body {
font-size: 87.5%;
}

h1 {
font-size: 150%;
}

In this case, the font size of the HTML document is 16px, and the body is set at 87.5% of 16px, which is 14px.
The h1 element is inside the body, which means it’s 150% of 14px, not 16px. 150% of 14px is 21px, so the h1 element is 21px.
This is helpful for mobile websites, where the font size might change depending on the device.
You can also specify font size with a unit called em. This works like percents, but is easier to calculate and read.
A font size of 1em is the same as 100%. If you rewrite the above example using ems, it looks like this:
Rem works like em, but is based on the html font size, not the parent’s font size.

Changing Style
The font-style property allows you to make your text normal, italic, or oblique.

Changing Weight
As mentioned in the previous section, font-style isn’t usually used to make text bold. Instead, developers use a property called font-weight. Its most common values are normal and bold.
If your font has many weights, you can use numbers to specify which weight you’d like to use. A normal font is 400, while a bold font is 700. A semi-bold font might have a weight of 600.

Changing Line-Height
Each line of text on a web page has a certain height, which creates space between each line of text. If there were no line-height, each line would be squished together, and it would be very hard to read.

Changing Alignment
You can use the text-align property align the text to the left, right, or center. (You can also justify text, although it isn’t very popular.)

Underlining Text
You can add or remove an underline using the text-decoration property. Usually you don’t want to add an underline to text unless it’s a link. But you may want to remove the underline from a link, which is a popular style.

Adding a Shadow
You can add a shadow to your text using the text-shadow property. This is only recommended for titles or short text. Adding a shadow to paragraphs of text would only make it difficult to read.
Text-shadow has four values: the x-offset, the y-offset, the blur radius, and the color. The color is usually written in RGBA so the shadow is semi-transparent.

Changing Capitalization

You can transform your text into all caps, lowercase, or capitalize each word using the text-transform property.

Spacing Out the Text
The letter-spacing property allows you to space out the letters of a word. You can use pixels or ems (based on the size of the text) to do this.
