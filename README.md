# Basic Web App

This is a basic web app whose purpose is to illustrate the speed advantages of using automation and automation tools, such as Yeoman, Grunt and Bower, over the manual approach used here.

## Required Steps 

To create this app, several steps are needed which are time consuming an error prone (human factor). 

* Download Bootstrap
* Download jQuery
* Link HTML files to CSS and JS files
* Write HTML, CSS and JS boilerplate 
* Test the app in a Browser to ensure that all the pieces are working and playing nice
* Add your own custom HTML, CSS and JS 
* Uglify the JS
* Minify and optimize the CSS
* Minify the HTML
* Set up a dist folder
* Copy uglified and minified HTML, JS and CSS to dist folder
* Copy all other necessary assets (e.g. images, scripts) exist in dist folder

In all of the above steps, there is **only one** that truly interests us as developers, and that is:

* Add your own custom HTML, CSS and JS 

All of the above take a lot of time to do, and when performed manually, understandable human error obfuscates the process and introduces small mistakes that take even more time to deal with. Specifically syntax errors, wrong path errors, and others. 

## Solution

We will use Yeoman, Grunt, Bower and NPM to automate all of the above steps besides writing our own customer HTML, CSS and JS, which is all developers should be interested in. That said, developers should have a thorough understanding of the automation process happening in the background.

