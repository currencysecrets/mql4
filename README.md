MetaQuotes Language Package (MQL4)
==================================

If you've been coding using MetaTrader for quite some time you've no doubt come across those times where you've experienced problems such as:

+ An unbalanced parentheses
+ Code that's too long which won't collapse
+ Renaming of variable and parameter names
+ Styling of the look and feel of the editor
+ Code hints not working or disappearing after selecting a function
+ Not enough detail and going to the MQL4 site to read the documentation only to find their site is down for maintenance

Yes, I've been there too.

I like MetaTrader though, but coding on their platform can be a real nightmare.

So, I decided to couple the best text editor in the world with the best automated forex trading language in the world. And you now have before you the result of a couple of weeks work in getting all aspects of the MQL4 language into a Sublime Text snippet package.

Installation
============

To install the package either:

+ Download the zip file either in github or on the website: http://www.currencysecrets.com/575/a-better-way-to-code-mql4 
+ Unzip the file on your computer
+ Move the "MQL4" folder into Sublime Text's "Packages" folder
+ Restart Sublime Text

You may also want to download WBond's Package Control found here: http://wbond.net/sublime_packages/package_control

And install packages such as: BracketHighlighter (Cmd + Shift + p then enter "install package" then "brackethighlighter" hit return to install).

Using
=====

To use the MQL4 language simply begin typing your code. 

MQL$ functions will have their necessary parameters with types, the following abbreviations being the definitions of the types needed:

+ int = integer
+ dbl = double
+ str = string
+ bool = boolean
+ clr = color
+ obj = object
+ ... = anything

Whenever a function has a default value with several parameter choices (separated by pipes "|") it is designated with an asterisk, eg

MetaTraderFunction( int test=OP_BUY*|OP_SELL )

Don't forget to tab through parameters!


If you any feature requests or amendments to be made to the code please let me know!!