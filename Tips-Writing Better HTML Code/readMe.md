1. Double-check the document structure

Always include the basic HTML format shown below. If this isn’t done correctly, it could cause errors for your web page.

<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <title>Document</title>
    </head>
    <body></body>
</html>

2. Use HTML elements the way they were intended
   Each HTML element was designed for a certain purpose, so don’t use them for other purposes. Good code is simple and doesn’t have any weird hacks.
   If you aren’t sure how to use an HTML element, you can learn more about it at MDN Library Just search for the element name.

3. Keep your code consistent
   Decide the way you’ll write your code and keep it consistent throughout the document.
   For example, it’s common to use lowercase letters for all HTML code, indent child elements, and always use double quotes ("") instead of single quotes ('').
   This will make your code more legible for you and anyone else who may work on it in the future.

4. Keep CSS out of your HTML
   It’s important to keep HTML and CSS separate, because they’re used for different purposes.
   If you include CSS code inside of your HTML document, it will be more complicated to update the style of your web page. If you keep all your styles in one CSS file, you can update it quickly without affecting your HTML code.
   It’s best to put all of your HTML code in HTML files, and make a separate CSS file for the styles.

5. Remove code errors
   You can check your HTML in the The W3C Markup Validation Service that checks your code for errors and mistakes. Just copy and paste your entire HTML document into the text box and press “Check.”
   It’s best to validate your code when you’re finished writing it, and fix all of the errors.
   If you don’t know what the errors mean, you can search for them on Google or W3Schools.

6. Add alternative text to images
   Alternative text is the alt attribute on an img element. Alt text displays when the image doesn’t load properly. This lets the user know what the image was for, or what the image says.
   This is really important for two reasons: one, if the image has important information, it guarantees that the information is conveyed; and two, the text is indexed by Google and shows up in Google searches to help people find your image and web site.
   If the image is only decorative and doesn’t have important information, you can leave the alt attribute blank, like below:

<img src="myimage.jpg" alt="">

7. Give good names to classes and IDs
   Classes and IDs are used to identify elements in your HTML that you want to style with CSS (or manipulate with Javascript).
   However, it’s important to name them correctly: after their function, not their form.
   For example, if you are placing a red alert box at the top of your webpage, you shouldn’t give it a class name of “red-box.”
   Why? Because the design of your webpage may change, and you may turn it into a yellow alert box. Once that happens, your class name doesn’t make sense anymore.
   Instead, give your alert box a class name after its function—like “alert-box.” Then you can change the style as much as you want and the class name will still apply.
   It works the same for position. Don’t give your left sidebar a class name of “left-box,” because you may move it to the right side in the future. Name it after its function.

8. Don’t use too many divs
   New web developers tend to use a lot of divs to create their web pages. You might be tempted to do this, too.
   However, this is usually unnecessary and adds a lot of extra code that weighs down your web page.
   Instead of using a lot of divs, use <main>, <article>, <section>, <h1> or any other element that’s appropriate for the content inside. Then apply your styles to these elements directly instead of adding an extra div.

9. Reusing layouts
   Once you create a good layout, reuse it in each page to save yourself time and effort.
   Make it general enough that it works for each page, and then change up the content inside to make your web pages.
   Not only is this easier, but it makes sure that all of your pages look alike, providing a consistent experience for the user.

10. Keep editing and simplifying your code
    Good coders do something called “refactoring.”
    Every day, after writing lots of code, they go back and analyze everything they wrote, looking for parts that they can simplify or make more efficient.
    This act of “refactoring” is what makes truly good. You can get rid of duplicate elements, remove unnecessary HTML elements, or restructure a part of your web page to make it load faster.
    Good writers would never publish their work after the first draft. Neither should you.
