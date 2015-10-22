# Basic Web App

This is a basic web app whose purpose is to illustrate the speed advantages of using automation and automation tools, such as Yeoman, Grunt and Bower, over the manual approach used here.

## Required Steps 

To create this app, several steps are needed which are time consuming an error prone (human factor). 

* Download Bootstrap
* Download jQuery
* Use NPM to globally install UglifyJS2, CSSO and Minify-HTML
* Link HTML files to CSS and JS files
* Write HTML, CSS and JS boilerplate 
* Test the app in a Browser to ensure that all the pieces are working and playing nice
* Add your own custom HTML, CSS and JS 
* Uglify the JS
* Minify and optimize the CSS
* Minify the HTML
* Set up a dist folder
* Copy uglified and minified HTML, JS and CSS to dist folder
* Update the links in the HTML so that they point at the minified JS and CSS
* Make sure that all other necessary assets (e.g. images, scripts) exist in dist folder

In all of the above steps, there is **only one** that truly interests us as developers, and that is:

* Add your own custom HTML, CSS and JS 

All of the above take a lot of time to do, and when performed manually, understandable human error obfuscates the process and introduces small mistakes that take even more time to deal with. Specifically syntax errors, wrong path errors, and others. 

## Why can we see a dist folder?

Usually, a `dist` folder would not be pushed to your repo, as it should be generated by the User manually or by automation tools. I have chosen to include it to show what state the code needs to be in at the end of the Required Steps above. This serves to illustrate the complex transformations that need to occur, hopefully strengthening my argument for automation.   

## Uglify and Minify Commands

#### Minify HTML

    html-minifier index.html --remove-comments --collapse-whitespace --remove-empty-attributes --remove-style-link-type-attributes --lint --case-sensitive --output index.min.html

### Minify CSS

    csso style.css style2.css -o style.min.css

### Uglify and Minify JS

    uglifyjs main.js main2.js --compress --mangle --output main.min.js

## Solution

We will use Yeoman, Grunt, Bower and NPM to automate all of the above steps besides writing our own custom HTML, CSS and JS, which is all developers should be interested in. That said, developers should have a thorough understanding of the automation process happening in the background.

