# Regex tutorial
Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern .

One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in (almost) all programming languages ​​(JavaScript, Java, VB, C #, C / C++, Python, Perl, Ruby, Delphi, R, Tcl, and many others) with the slightest distinctions about the support of the most advanced features and syntax versions supported by the engines).

#### Anchors — ^ and $

`^The        matches any string that starts with The 
end$        matches a string that ends with end
^The end$   exact string match (starts and ends with The end)
roar        matches any string that has the text roar in it `


#### OR operator — | or []

`a(b|c)     matches a string that has a followed by b or c (and captures b or c) 
a[bc]      same as previous, but without capturing b or c`

## Flags 

We are learning how to construct a regex but forgetting a fundamental concept: flags.

g   (global) does not return after the first match, restarting the subsequent searches from the end of the previous match

m   (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string

i   (insensitive) makes the whole expression case-insensitive (for instance /aBc/i would match AbC)

***Remember that*** inside bracket expressions all special characters (including the backslash \) lose their special powers: thus we will not apply the “escape rule”. 

# Guide to Grid 

CSS Grid Layout is the most powerful layout system available in CSS. It is a 2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system. You work with Grid Layout by applying CSS rules both to a parent element (which becomes the Grid Container) and to that element’s children (which become Grid Items).


#### Grid Container
The element on which display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container.


`<div class="container">
  <div class="item item-1"> </div>
  <div class="item item-2"> </div>
  <div class="item item-3"> </div>
</div>`



#### Grid Item
The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.


`<div class="container">
  <div class="item"> </div>
  <div class="item">
    <p class="sub-item"> </p>
  </div>`



The most powerfull line in grid 
Fluid width columns that break into more or less columns as space is available, with no media queries!

`.grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  /* This is better for small screens, once min() is better supported */
  /* grid-template-columns: repeat(auto-fill, minmax(min(200px, 100%), 1fr)); */
  grid-gap: 1rem;
  /* This is the standardized property now, but has slightly less support */
  /* gap: 1rem */
}`


##### grid-template-areas

Defines a grid template by referencing the names of the grid areas which are specified with the grid-area property
  
##### justify-self

Aligns a grid item inside a cell along the inline (row) axis (as opposed to align-self which aligns along the block (column) axis). This value applies to a grid item inside a single cell.

##### place-self

place-self sets both the align-self and justify-self properties in a single declaration.

##### align-items

Aligns grid items along the block (column) axis (as opposed to justify-items which aligns along the inline (row) axis). This value applies to all grid items inside the container.


# Common Responsive Layouts with CSS Grid 

The `repeat()` function takes two arguments, the first will define the number of column tracks and the second, what width the tracks should be.


Often when we put images in a responsive grid layout like this we come across the problem of the images stretching out of proportion. Using

`object-fit: cover;`

















