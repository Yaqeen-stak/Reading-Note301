# Responsive Web Design "RWD"
 TO build websites suitable for all users.
Or its building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. 

### Responsive vs. Adaptive vs. Mobile 
 Responsive generally *means* to react quickly and positively to any change 
 Adaptive *means* to be easily modified for a new purpose or situation, such as change.

 **Responsive web design is broken down into three main components:**
 * flexible layouts
 * media queries 
 * flexible media

`target ÷ context = result`

#### Initializing Media Queries:

In HTML :
`<link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">`

In CSS :
`@media all and (max-width: 1024px) {...}`
OR 
`@import url(styles.css) all and (max-width: 1024px) {...}`

#### Logical Operators in Media Queries:
There are three different logical operators available for use within media queries, including `and` , `not`, and `only`.

***When using the `not` and `only` logical operators the media type may be left off. In this case the media type is defaulted to all.***

#### Media Features in Media Queries :
Media features identify what attributes or properties will be targeted within the media query expression. 

### Mobile First:

The operating belief behind mobile first design is that a user on a mobile device, commonly using a smaller viewport, shouldn’t have to load the styles for a desktop computer only to have them over written with mobile styles later. Doing so is a waste of bandwidth. Bandwidth that is precious to any users looking for a snappy website.


## Flexible Embedded Media:

Unfortunately the max-width property doesn’t work well for all instances of media, specifically around iframes and embedded media. When it comes to third party websites, such as YouTube, who use iframes for embedded media this is a huge disappointment. Fortunately, there is a work around.

 The parent element needs to have a width of 100% so that it may scale based on the width of the viewport. The parent element also needs to have a height of 0 to trigger the hasLayout mechanism within Internet Explorer.


# Float :
Float is a CSS positioning property. 
 Floated elements remain a part of the flow of the web page.


There are four valid values for the float property. `Left` and `Right` float elements those directions respectively. `None` (the default) ensures the element will not float and `Inherit` which will assume the float value from that elements parent element.


While floats can still be used for layout, these days, we have much stronger tools for creating layout on web pages. Namely, Flexbox and Grid. Floats are still useful to know about because they have some abilities entirely unique to them.


### Clearing the Float
An element that has the clear property set on it will not move up adjacent to the float like the float desires, but will move itself down past the float

Clear has four valid values as well:
* `Both` is most commonly used, which clears floats coming from either direction
* `Left` and `Right` can be used to only clear the float from one direction respectively
* `None` is the default, which is typically unnecessary unless removing a clear value from a cascade
* ` Inherit` would be the fifth, but is strangely not supported in Internet Explorer

### Techniques for Clearing Floats 
* `clear: both;`
* `<div style="clear: both;"></div>`
* The Overflow Method 
* The Easy Clearing Method


floats are pretty similar to the dynamics of riding an escalator, and I am going to show how they can be used alongside the clear property to create crystal-clear relationships within divs. This way, the next time you try to use floats in your code, you won’t encounter any surprises.


`Clear: left` tells each person floating left that they should align themselves behind the first element that is floated left. Depending on the size of the bottom two people, it could be challenging for any normal elements to squeeze through and occupy the space on the top right. So even good escalator practices can still lead to blockages

`clear:both` This allows you to reset the flow of elements, as opposed to continuing to maintain a right, left and normal flow.


# SMACSS 

 SMACSS is a way to examine your design process and as a way to fit those rigid frameworks into a flexible thought process. It is an attempt to document a consistent approach to site development when using CSS.







