## Website Performance Optimization portfolio project

Your challenge, if you wish to accept it (and we sure hope you will), is to optimize this online portfolio for speed! In particular, optimize the critical rendering path and make this page render as quickly as possible by applying the techniques you've picked up in the [Critical Rendering Path course](https://www.udacity.com/course/ud884).

To get started, check out the repository and inspect the code.

### Getting started

####Part 1: Optimize PageSpeed Insights score for index.html

Optimization includes:

- commenting out Google Font API call. The font will not make a big difference in page layout/style, but slows down load time;
- minify style.css to style_min.css;
- move portrait styles in separate file;
- convert pizzeria image to 8 bit and resize;
- move Google Analytics JS code to the bottom of the HTML page.

####Part 2: Optimize Frames per Second in pizza.html

Optimization for main.js:

- make determineDx inline code with some modifications. Thank you, Cameron!
- in updatePositions() - move style reading out of loop. It speed up rendering to 60fps during scroll.
