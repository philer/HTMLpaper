HTMLpaper
=========

This is a simple CSS "Framework" that lets you create and manually layout printable HTML documents.
Basically the printed version will look exactly like what you see on screen.
You can create complex layouts using CSS without worrying about them getting botched by your browser's print settings.

Additionally, there is a very basic LaTeX style formatting option
that let's you create pages that will look like and
seemlessly integrate into LaTeX documents. See LaTeX's `pdfpages` package.

Font files for LaTeX's Latin Modern as well as the original Computer Modern are included. The css will default to a system installed version of Latin Modern and fallback to the included Latin Modern webfont.
You may also want to include [MathJax](http://www.mathjax.org) for displaying mathematical formula.

### Requirements
* I assume you know your way around HTML and CSS. Otherwise you should probably find another (easier) way to do whatever it is you are trying to do.
* A sensible, up-to-date web browser is recomended. I have only tested this in Firefox 29+ but I assume that latest Webkit browsers will work fine as well (feedback is appreciated).


### How to use
* Look at the *example.html* file. The easiest way to start will be to modify it.
You can copy-paste `div.page` to add more pages.
Make sure you leave the document structure intact and `page.css` is linked in your document's head.
* Put your content inside `div.page-inner`. Go Nuts.
* Add the appropriate CSS classes to specify what paper format you want to use.Look inside *page.css* to see what paper formats are available.
The default format is DIN A4.
Feel free to suggest more formats!
* Add a `.latex` class in your document for things that should look like LaTeX. If it all should look like LaTeX, just add it to the `body` tag.
Make sure *latex.css* is linked in your document's head and look inside to see what classes you can use.
* Open the HTML file in your browser (see requirements).
* Use the browser's print function.
Make sure to check a preview first or use a 'print to file' feature.


### When to use
Consider the following scenarios
* You want to create a short (1 or 2 pages) document, like a handout or a cheatsheet.
* You are trying to create something that looks like LaTeX but LaTeX keeps botching your complex box layout. You know you can achieve it using CSS.
* All other alternatives have failed you (office suite, InDesign, [Scribus](http://www.scribus.net/canvas/Scribus)).
* Maybe you want to automate stuff like generating a table or even create graphics with something like [D3.js](http://d3js.org/).
* Something else I haven't though of yet.


### When not to use
* Don't use this to write long, multi page documents. That's what LaTeX is for.
* Don't expect any magical auto-formatting. That's not what this is.
* Don't use this *because* you don't know LaTeX. If you *can* use this then LaTeX will be easy enough to learn for you.


### Terms
* This Software is provided as is, yada yada. I don't take any responsibility for things you manage to break or waste by using this. If you print out a thousand pages and then notice something is slightly off, that's on you.
* Don't distribute it claiming you created it yourself.
* If you create something cool with this, you may show it to me, so I can feel warm and fuzzy inside.
* License is MIT, see included LICENSE file.
