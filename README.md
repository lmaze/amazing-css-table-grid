# [Amazing CSS table grid](https://github.com/lmaze/amazing-css-table-grid)

Create powerful multi-device layouts quickly and easily with this pure CSS grid system based on the display table property. If you're familiar with grid systems, you'll feel right at home. If not, you'll learn quickly.

To get started, check out <http://lmaze.github.io/amazing-css-table-grid/>.


## Why another grid ?

Almost all current grid systems are based on the display `inline-block` CSS property or on floating elements. There are several problems and limitations with this approach. For example it is not possible to easily make columns of the same height or vertically aligning column content. The use of negative margins can also be problematic. So here is a grid based on the display `table` property which making some kind of magic ;-)


## Compatibility

You can use this grid system with all browsers that are compatible with CSS 2.1. In practice it covers almost all browsers except Internet Explorer below version 8. You can get more information on [caniuse](http://caniuse.com/#feat=css-table).

If you want the grid to be responsive in IE8 you must include a polyfill like [Respond.js](https://github.com/scottjehl/Respond) to support media queries. This operation is not necessary for other browsers, **only CSS is needed**.


## Which version do you need?

This grid comes in three flavours : classic version, postprocessor version, and Sass version.

### Classic version

If you aim to use this grid system without changing it's configuration, just download the CSS file `table-grid.css` in your project. You should at least rewrite the media queries to have custom breakpoints.

### Postprocessor version
If you use only a postprocessor like [Pleeease](http://pleeease.io/) or [Myth](http://www.myth.io/), you should grab the CSS file `table-grid.next.css`. At the start of this file you can change the custom media queries and set the custom properties with your own values.

### Sass version

If you're used to deal with the [Sass](http://sass-lang.com/) preprocessor, your best choice is to install this version : it is far more flexible and scalable than the basic CSS and the postprocessor versions. In the `_config.scss` file you can :

* Enable the xl columns
* Set a prefix for all the CSS class names (`tg-` for example)
* Set the width of the gutters
* Set the total number of columns
* Set the media queries configuration
* Enable the use of future CSS's features (postprocessor required) and set the custom media queries configuration
