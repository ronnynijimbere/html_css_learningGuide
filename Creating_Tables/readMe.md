Creating Tables
Tables are easy to create in HTML if you know what you’re doing. To create a table, you’ll need the <table> element, the <tr> or table-row element, <td> or table-cell elements and <th> or table-header elements.

Adding Extra Information to Tables
You can use special HTML elements to make a header, footer or a caption for your table.
The <caption> element gives you a table caption.
If you want to create a header and footer, you need to use the <thead>, <tbody>, and <tfoot> elements. Then place your <tr> elements inside each section.

Merging Cells
You can merge cells to create longer ones by using the attributes colspan and rowspan.
To merge cells horizontally, add a colspan attribute with the number of columns you’d like the cell to span. Remember that this cell will take up the space of more than one cell, so adjust the number of cells in the row accordingly.

Styling Tables
Tables have a number of unique properties that can be styled in CSS.
First of all, you can make sure that the table will stretch to fill the entire width of the page by adding 100% width:
Use border-collapse to remove the whitespace in between the borders of the table
For the opposite effect, use border-spacing to increase the amount of whitespace between the borders of the table.
Use table-layout to ensure that all of the cells will stay the same width:
