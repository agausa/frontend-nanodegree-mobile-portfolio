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
- added transform: translateZ(0); to randomPizzaContainer style;
- moving select query to elements outside of for loops;
- move 'var phase' outside the for loop - will prevent creation of variable each iteration;
- optimized number of floating pizzas - giveMeMorePizza() function. Listen on 'resize' event;

####How to run the application

To run, please open 'index.html' in any browser. Locate to pizza page to see optimized page!

####How to run profile on the application

To inspect the site on your phone, you can run a local server

$> cd /path/to/your-project-folder
$> python -m SimpleHTTPServer 8080
Open a browser and visit localhost:8080

Download and install ngrok to the top-level of your project directory to make your local server accessible remotely.

$> cd /path/to/your-project-folder
$> ./ngrok http 8080
Copy the public URL ngrok gives you and try running it through PageSpeed Insights!


####Customization with Bootstrap

The portfolio was built on Twitter's Bootstrap framework. All custom styles are in dist/css/portfolio.css in the portfolio repo.

Bootstrap's CSS Classes
Bootstrap's Components
