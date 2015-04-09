# layoutDemo
Using display:inline-block to position elements. Responsive design.

# Code explanation

## Remove margins
    *{
        margin: 0;
    }

Elements have default margin to which adds space around the element. This code removes the space from all elements. The * is the universal selector.

## Colour backgrounds
    background-color: red;

Added to show where the elements are.

## [Displaying content](https://developer.mozilla.org/en-US/docs/Web/CSS/display)
    display: inline-block;

How should content be put on screen. There is `block` and `inline`.

`block` are things that form chunks on page like `p` `h1` and `div`.

`inline` are things that go inside the blocks. E.g. `a`, `strong` and `em`.

There are other options. inline-block allows elements to have block properties but be treated externally like inline elements.

## Aligning elements
    vertical-align: top;

The inline-block elements can have different heights. This makes them have their tops at same level. The default is at the bottom. Comment out the vertical-align from #order to see the difference.

## Setting width
    width: 60%;

By default block elements are 100% of the width of it's container (the surrounding tag).

Inline elements are the width of their content.

On the page the header is 100% of the page.

On the page the menu section is 60% of the page.

On the page the order section is 39% of the page.

Having this total at 99% is < 100 so they fit next to each other. If they were larger the order section would be forced onto a new line under the menu. Increase the width of the order section to demonstrate this.

The sections in the class menuPart are inside the menu section. So they are 49% of 60%. Not the page.

The margin (reset by *) is set by .menuPart This is to ensure there are gaps.
