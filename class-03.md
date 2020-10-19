# Templating with MUSTACHE 
Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.

**Mustache**
As the name suggests, it was named mustache because the syntax resembles a Mustache. 

It is often referred to as ***logic-less*** because there are no if statements, else clauses, or for loops. Instead, there are only tags.


#### Mustache-Express
With Yarn:

`$ yarn add mustache-express`

OR with NPM:

`$ npm install mustache --save`


# Flexbox
Last Updated


The Flexbox Layout (Flexible Box) module aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic (thus the word “flex”).

The main idea behind the flex layout is to give the container the ability to alter its items’ width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes). A flex container expands items to fill available free space or shrinks them to prevent overflow.

### Basics and Terminology 

Since flexbox is a whole module and not a single property, it involves a lot of things including its whole set of properties. Some of them are meant to be set on the container (parent element, known as “flex container”) whereas the others are meant to be set on the children (said “flex items”).


#### display
This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.

`.container {
  display: flex; /* or inline-flex */
}`


#### flex-direction 
This establishes the main-axis, thus defining the direction flex items are placed in the flex container.

`.container {
  flex-direction: row | row-reverse | column | column-reverse;
}`


#### flex-wrap

two rows of boxes, the first wrapping down onto the second
By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.

`.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}`


#### flex-flow

This is a shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.

`.container {
  flex-flow: column wrap;
}`




