title: Cascading Style Sheets
category: page
slug: cascading-style-sheets
sort-order: 0411
meta: Learn how to use Cascading Style Sheets (CSS) to create your web application's user interface design on Full Stack Python.
choice1url: /javascript.html
choice1icon: fa-html5 fa-inverse
choice1text: How do I create dynamic browser interaction with JavaScript?
choice2url: /static-content.html
choice2icon: fa-spinner fa-inverse
choice2text: How should I host static content such as my CSS files?
choice3url: /source-control.html
choice3icon: fa-code-fork fa-inverse
choice3text: How can I save and version my code so it doesn't get lost?
choice4url: /application-programming-intefaces.html
choice4icon: fa-exchange
choice4text: What are APIs?


# Cascading Style Sheets (CSS)
Cascading Style Sheet (CSS) files contain rules for how to display and 
lay out the HTML content when it is rendered by a web browser.


## Why is CSS necessary?
CSS separates the content contained in HTML files from how the content 
should be displayed. It is important to separate the content from the rules
for how it should be rendered primarily because it is easier to reuse those
rules across many pages. CSS files are also much easier to maintain on large
projects than styles embedded within the HTML files.


## How is CSS retrieved from a web server?
The HTML file sent by the web server contains a reference to the CSS file(s)
needed to render the content. The web browser requests the CSS file after the
HTML file as shown below in a screenshot captured of the Chrome Web Developer 
Tools network traffic.

<img src="theme/img/css-chrome-dev-tools.jpg" width="100%" alt="Google Chrome Web Developer Tools shows how CSS is separate from the HTML content." class="technical-diagram" />

That request for the fsp.css file is made because the HTML file for Full 
Stack Python contains a reference to ``theme/css/fsp.css`` which is shown
in the view source screenshot below.

<img src="theme/img/fsp-css-source.jpg" width="100%" alt="View source screenshot for the fsp.css file in index.html." class="technical-diagram" />


## CSS preprocessors
A CSS preprocessor compiles a processed language into plain CSS code. CSS 
preprocessing languages add syntax such as variables, mixins and functions
to reduce code duplication. The additional syntax also makes it possible for
designers to use these basic programming constructs to write maintainable
front end code.

* [Sass](http://sass-lang.com/) is currently the favored preprocessor in
  the design community. Sass is considered the most powerful CSS preprocessor
  in terms of advanced language features.

* [LESS](http://lesscss.org/) is right up there with Sass and has an ace up
  its sleeve in that the [Bootstrap Framework](http://getbootstrap.com/) is
  written in LESS which brings up its popularity.

* [Stylus](http://learnboost.github.io/stylus/) is often cited as the third
  most popular CSS preprocessing language.


### CSS preprocessor resources
* The Advanced Guide to HTML and CSS book has a well-written chapter on 
  [preprocessors](http://learn.shayhowe.com/advanced-html-css/preprocessors).

* [Sass vs LESS](http://css-tricks.com/sass-vs-less/) provides a short answer
  on which framework to use then a longer more detailed response for those
  interested in understanding the details.

* [How to choose the right CSS preprocessor](http://blog.teamtreehouse.com/how-to-choose-the-right-css-preprocessor)
  has a comparison of Sass, LESS and Stylus.

* [Musings on CSS preprocessors](http://css-tricks.com/musings-on-preprocessing/)
  contains helpful advice ranging from how to work with preprocessors in a
  team environment to what apps you can use to aid your workflow.


## CSS frameworks
CSS frameworks provide structure and a boilerplate base for building a
web application's design.

* [Bootstrap](http://getbootstrap.com/)

* [Foundation](http://foundation.zurb.com/)

* [Gumby](http://gumbyframework.com/)

* [Compass](http://compass-style.org/)

* [Profound Grid](http://www.profoundgrid.com/)

* [Skeleton](http://www.getskeleton.com/)

* [HTML5 Boilerplate](http://html5boilerplate.com/)


## CSS resources
* [Frontend Development Bookmarks](https://github.com/dypsilon/frontend-dev-bookmarks)
  is one of the largest collections of valuable resources for frontend
  learning both in CSS as well as JavaScript.

* [Mozilla Developer Network's CSS page](https://developer.mozilla.org/en-US/docs/Web/CSS)
  contains an extensive set of resources, tutorials and demos for learning
  CSS.

* [CSS Positioning 101](http://alistapart.com/article/css-positioning-101)
  is a detailed guide for learning how to do element positioning correctly
  with CSS.

* [CSS3 cheat sheet](http://media.smashingmagazine.com/wp-content/uploads/images/css3-cheat-sheet/css3-cheat-sheet.pdf)

* [Learn CSS layout](http://learnlayout.com/toc.html) is a simple guide that
  breaks CSS layout topics into chapters so you can learn each part one
  at a time.

* [Google's Web Fundamentals class](https://developers.google.com/web/fundamentals/)
  shows how to create responsive designs and performant websites.

* [Tailoring CSS for performance](http://programming.oreilly.com/2014/04/tailoring-css-for-performance.html)
  is an interesting read since many developers do not consider the 
  implications of CSS complexity in browser rendering time.

* [Can I Use...](http://caniuse.com/) is a compatibility table that shows
  which versions of browsers implement specific CSS features.


## CSS learning checklist
<i class="fa fa-check-square-o"></i> 
Create a simple HTML file with basic elements in it. Use the
``python -m SimpleHTTPServer`` command to serve it up. Create a 
``<style></style>`` element within the ``<head>`` section in the HTML page. 
Start playing with CSS within that style element to change the look and feel 
of the page.

<i class="fa fa-check-square-o"></i> 
Check out front end frameworks such as Bootstrap and Foundation and integrate
one of those into the HTML page.

<i class="fa fa-check-square-o"></i> 
Work through the framework's grid system, styling options and customization
so you get comfortable with how to use the framework.

<i class="fa fa-check-square-o"></i> 
Apply the framework to your web application and tweak the design until you
have something that looks much better than generic HTML.


### Once your app is styled what do you need to learn next?
