# Layout

### Positioning Elements

##### CSS treats each HTML element as if it is in its own box. Box witll be either a block-level or inline box.

##### block-level elements (h1, p, ul, li)

##### inline elements (img, b, i)

##### if one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

###### It is common to group a number of elements together inside a div (or other block-level) element.

##### CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS> You can also float elements using the float property

##### Normal flow (position:static) each block-level elements sits on top of the next one. Its the default

##### Relative positioning (position:relative) moves an element in relation to where it would have been in the normal flow. 

##### Absolute positioning (position:absolute) the box is taken out of normal flow and no longer affects the position of other elements on the page (they act like it is not there)

##### fixed positions (position:fixed) a type of absolute positioning that requires the position property to have a value of fixed.

##### overlapping elements (z-index) when you use relative, fixed or absolute positioning, boxes can overlap. If they do, the elements that appear later in HTML code sit on top of those that are earlier in the page. Z-index controls what is seen first (used in CSS)

##### floating elements (float) allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. You should also use the width property to indicate how wide the floated object is to ensure readability.

##### clearing floats (clear) see page 372

### Fixed width layouts

##### Fixed width layouts do not change size as teh user increases or decreases the size of their browser window. Measurements tend to be given in pixels.

##### Liquid Layouts stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

##### Layout grids. Grids set consistent proportions and spaces between items which help to create a professional looking design.

##### See page 393 for grid based layout example
