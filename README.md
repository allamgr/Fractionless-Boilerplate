# Fraction.less Boilerplate

Fraction.less is an HTML5/CSS3 quick-start kit meant to be super easy to start with. Check out the grid classes and you can have a page layout in no more than 5 minutes!

Fraction.less has a totally misleading name. The grid is based totally on fractions but in a way that won't require much math. If you can add fractions to equal one-whole then you can use Fraction.less.

Fraction.less isn't meant to be all things to all people. It's meant for simple page layouts that can be divided from halves down to fourths and most things in between. Before all you hipsters write it off, actually look at the grid styles.

## Components

Fraction.less Boilerplate uses code from the following projects:

* jQuery Effects Library (1.6.4) - Minified and uncompressed dev versions included
* Normalize.css - Not a reset, a baseline to be modified
* 1140 CSS Grid - The heart of our Less-based grid system, modified with Less
* Less CSS - The Less stylesheet language. See (lesscss.org)[http://lesscss.org] for more.
* More as we add them...

# Usage

Setup is pretty easy and Fraction.less comes with some tools to help you test your development environment.

## Initial Setup

Download and extract the files to where you want to start developing or do a 
    git clone git://github.com/billpatrianakos/Fractionless-Boilerplate.git


## The Grid

The Fraction.less grid is based on the 1140 Grid System. It works out of the box but you have the option of being able to change the widths of each class by modifying a few Less variables.

To use the grid, apply the `.full-width` class to any container elements. These will either hold content spanning the entire page width or a minimum of two smaller elements.

Always add the `.left` class to all elements you plan to line up in a row. All rows must add up to 1 thus you must be able to add simple fractions in your head.

The last element in each row will get a `.last` class so you don't mess up the layout.

Apply `.clearfix` to any `.full-width` elements that act up on you. In 90% of my tests, all layout issues could be solved with `.clearfix`.

The grid is easily extensible but only ships with divisions from full-width to one-quarter. This is enough to get a layout working within 5 minutes and can be easily added to with intermediate sized columns if needed.

## style.less

This is your main stylesheet. It imports the grid and normalize.css files. Imports will only work if you've compiled your Less files first which requires either the Less Ruby Gem, the Less compiler running on Node.js, or Less.app on Mac.

We've also included `less.js` for those who want to save compiling for later or want a quick way to experiment with Less.

## Compiling your .less files

Mac users can search for and install Less.app which gives you an easy GUI interface app that watches for changes to .less files and compiles them automatically.

First install the LESS gem using `you@computer$ gem install less`

Or you can get LESS if you've got node.js and npm using `you@computer$ npm install less`

To compile your less stylesheets run `you@computer$ cd /path/to/project/` making sure that you switch to the directory that holds your `/less` and `/css` directories. Then run the following command:

`you@computer$ lessc /less

### Usage Notes

Take heed of the following as there are some components of the boilerplate that need a bit of extra attention to work correctly.

_.htaccess Files_ - Fraction.less comes with a file named `1.htaccess`. On many systems hidden files are not included when pressing `Ctrl + A` then `Ctrl + C` to copy files between folders. To ensure this important file gets included in that situation we've named it. For it to work correctly you must rename it to simply `.htaccess`.

### Credits

We have to give credit where credit is due. Thanks to all these folks who are by far much smarter and more talented that I.

Paul Irish - HTML5 Boilerplate - http://html5boilerplate.com
@andytlr - 1140 Grid System - http://cssgrid.net
Cloudhead - LESS dynamic stylesheet language - http://lesscss.org
Bryan Jone - LESS.app (Mac only) - http://incident57.com/less/
... and more coming soon.

# License

Fraction.less Boilerplate is licensed under the Apache License 2.0. See the License.md file for details. This means you can use it however and wherever you want. You don't have to release any derivatives as open source and you are free to charge money for derived works. That's why I didn't go with the GPL. GPL kind of sucks...