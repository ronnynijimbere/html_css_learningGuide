Form Basics
All forms in HTML are surrounded by the <form> tag. This defines the beginning and end of the form.
Forms take two attributes: action and method. The action attribute links to a PHP file that tells the server what to do with the form. The method is either GET or POST and tells the browser how to send the form data to the server. For practice with HTML, you can leave these blank.

Adding Text Fields

The most common type of form input is the plain text field. This is an <input> element with a type attribute that has a value of text. An input element is self-closing, so it doesn’t need a closing tag.

Another type of text field is a <textarea> element. This is a resizable text box that gives the user more space to type. The textarea element takes two attributes, rows and cols, that determine the height and width of the text box.

Multiple-Choice Inputs

You can create radio buttons, checkboxes, or drop-downs that allow a user to select one or more choices from an existing list of options.

To add a set of radio buttons, you use the <input> element with a type of radio. You must also define the name and value properties.

To make a group of radio buttons, give them all the same name. You can write anything in the value property, but it will be sent to the server as the answer that was chosen.

The checkbox input is similar to the radio input, except that it has a type of checkbox instead of radio. Use checkboxes when multiple options can be selected. Use radio buttons when only one option in the list should be selected.

To create a drop-down menu, you will use the <select> element. To add an item to the drop-down menu, add an <option> element directly inside the <select>. Each <option> should have a value property, too.
By default, the first <option> element will be automatically selected when the page loads.
If you’d like to change the default option, add the selected attribute (with no value) to the <option> element.
If you want to make it possible for the user to select more than one option in a dropdown, simply add the multiple attribute (with no value) to the <select> element.

Adding Buttons
Adding buttons to forms is also quite easy. There are two ways to add buttons.
The first is by adding an input field with a type of submit, reset, or button. Each of these takes a value attribute that specifies the text that will display on the button.
A submit button submits the form when you press it. A reset button clears out a form and deletes all of the input when you press it.
These buttons are useful, but you can’t add any icons or images inside of them. They can only text text from the value attribute.

This is where the <button> element, a more popular option for form buttons, comes in handy.

Buttons have the same types as inputs, but they can have html, text, images, and icons inside of them.

Adding File Inputs
Another popular type of input is a file upload button. This button opens a dialog window where the user can choose a file to upload. When he or she clicks the submit button, the file will be sent to your server.
You can also add the multiple attribute to allow users to upload more than one file at a time.

Adding Hidden Inputs
Hidden inputs are slightly confusing, because they’re invisible to the user. These are fairly advanced inputs and are used to pass secret information to the server that you don’t want the user to see. The secret information is stored in the name and value attributes. You will probably not use these as a beginner, but it’s important to know that they exist.

Adding Form Labels

Of course, simply adding form inputs to your page won’t help anyone! You’ll need to include an easy-to-read label on each input that tells the user what to input.

A label element is fairly simple, and can take a for attribute whose value is the ID of an input field

Grouping Form Inputs
You can group inputs together with the <fieldset> element. This element helps to break up a long form into more manageable chunks. To add a title to your fieldset, add the <legend> element.

Adding Placeholder Text
For any text-based input, you can add placeholder text to give the user hints about what they should write. You can add this by using the placeholder attribute.

Making an Input Required
You can force the user to fill out parts of your form by making some of the inputs required.
