== 
== grid-template-columns, grid-template-rows
==

"grid-template-columns" is a CSS property used in CSS Grid Layout. It defines the columns of a grid container. You can specify the size of each column in the grid with this property. Here are some key points about grid-template-columns:

Fixed Size Columns: You can set fixed sizes for your columns. For example, grid-template-columns: 100px 200px 300px; would create three columns with widths of 100px, 200px, and 300px, respectively.

Fractional Units (fr): This unit allows you to divide the grid into proportionally sized columns. For instance, grid-template-columns: 1fr 2fr 1fr; divides the grid into three columns, where the middle column is twice as wide as the others.

Repeat Function: The repeat() function can simplify your code. For example, grid-template-columns: repeat(3, 1fr); creates three columns, each with equal width.

Auto-fill / Auto-fit: These keywords, used with repeat(), can create a flexible number of columns based on the container's width. auto-fill fills the row with as many columns as it can fit, while auto-fit collapses empty columns.

Using minmax(): The minmax() function is used inside grid-template-columns to specify a minimum and maximum size for your columns. For example, grid-template-columns: repeat(3, minmax(100px, 1fr)); creates three columns, each with a minimum width of 100px and a maximum width that fills the remaining space.

Responsive Grids: By combining these features with media queries, you can create responsive grid layouts that adjust to different screen sizes.

Example:

.grid-container {
    display: grid;
    grid-template-columns: 100px 200px 100px; /* 3 columns */
    grid-template-rows: 50px 100px; /* 2 rows */
}

<div class="grid-container">
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
    <div>Item 5</div>
    <div>Item 6</div>
</div>

Display: Matrix: 2 x 3 

==
== @media 
== 
/* Default styles for all devices */
body {
    background-color: lightblue;
}

/* Styles for screens wider than 600px */
@media screen and (min-width: 600px) {
    body {
        background-color: pink;
    }
}

/* Styles for landscape orientation */
@media screen and (orientation: landscape) {
    body {
        background-color: lightgreen;
    }
}
