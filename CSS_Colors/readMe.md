CSS Colors
we will learn how to specify color values in CSS, and develop an understanding of the
CSS color models like rgb, rgba, hsl and hex color codes

Once you know how to specify the colors, the same color values can be used everywhere in CSS,
whether you are specifying text color, background color, or whatever else.

The simplest, oldest way to specify color in CSS is to use the color keywords.
p {
background-color: blue;
}

RGB

The second way to specify color values we'll talk about is the RGB, or Red Green and Blue color system. These values are a bit more complex and less easy to understand, but they are a lot more versatile than keywords we looked at the last section. You can use RGB values to represent any color you want to use in your color scheme.
An RGB value is a function — rgb() — which is given three parameters that represent the intensity of the red, green and blue channel values of the colors. Each parameter is an integer between 0 and 255.

.colors {
background-color: rgb(255, 255, 255);
}

HSL

The next color system we'll talk about is the HSL model, which was implemented after a lot of interest from designers — instead of red, green and blue values, the hsl() function accepts hue, saturation, and lightness values. Like red, green and blue, these also help us distinguish between colors, but in a different way. Here's what they mean:

    hue: the base shade of the color. This takes a value between 0 and 360, presenting the angles around a color wheel.
    saturation: how saturated is the color? This takes a value from 0-100%, where 0 is no color (it will appear as a shade of grey) and 100% is full color saturation.
    lightness: how light or bright is the color? This takes a value from 0-100%, where 0 is no light (it will appear completely black) and 100% is full light (it will appear completely white)

RGBA and HSLA

RGB and HSL both have corresponding modes — RGBA and HSLA — that allow you to set not only what color you want to display, but also what transparency you want that color to have. Their corresponding functions take the same parameters, plus a fourth value in the range 0–1 — which sets the transparency, or alpha channel. 0 is completely transparent, and 1 is completely opaque.

Hexadecimal values

The next ubiquitous color system is hexadecimal values, or hex codes. Each hex value consists of a hash/pound symbol (#) followed by six hexadecimal digits, each of which can take a value between 0 and f (which represents 15) — so one of 0123456789abcdef. Out of the six digits, the first two represent the red channel, the next two represent the green channel and the last two represent the blue channel.

Opacity

There is another way to specify transparency via CSS — the opacity property. Instead of setting the transparency of a particular color, this sets the transparency of all selected elements and their children. Again, let's study an example so we can see the difference.

Note the difference — the first box that uses the RGBA color only has a semi-transparent background, whereas everything in the second box is transparent, including the text. You'll want to think carefully about when to use each — for example RGBA is useful when you want to create an overlaid image caption where the image shows through the caption box but the text is still readable. Opacity, on the other hand, is useful when you want to create an animation effect where a whole UI element goes from completely visible to hidden.
