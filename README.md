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

Installation/Updates
====================

#### Package Control

The easiest way to install this package in Sublime Text is to use WBond's Package Control - https://sublime.wbond.net/

Once you have this installed, simply run `Install Package` and select `MetaQuotes (MQL4) Language Package` in the prompt.

Bang. You're done!


#### Manually

To install the package by ZIP file do:

+ Download the zip file either in GitHub (click on Zip button above)
+ Unzip the file into Sublime Text's "Packages" folder (found by clicking "Preferences" menu then "Browse Packages...")
+ Restart Sublime Text

To install the package using the command line (CLI) do:

##### On linux:
```bash
cd ~/.config/sublime-text-2/Packages/
git clone https://github.com/currencysecrets/mql4.git
```
##### On OSX:
```bash
cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/
git clone https://github.com/currencysecrets/mql4.git
```
## Pull updates

##### On linux:
```bash
cd ~/.config/sublime-text-2/Packages/mql4/
git pull
```
##### On OSX:
```bash
cd ~/Library/Application\ Support/Sublime\ Text\ 2/Packages/mql4/
git pull
```

You may also want to download WBond's Package Control found here: http://wbond.net/sublime_packages/package_control

And install packages such as: BracketHighlighter (Cmd + Shift + p then enter "install package" then "brackethighlighter" hit return to install).

Usage
=====

To use the MQL4 language simply begin typing your code. You will begin to see a code hinting box that will link to MetaTrader data types, functions, constants and reserved words. Simply enter or tab the selected term you wish to use and Sublime Text will populate any necessary parameters into your working file.


Parameter Data Types
--------------------

Some MQL4 functions have parameters and for brevity sake the following abbreviations have been used in replacement of the standard data types recognised by MetaTrader. Please be aware that these shorter terms are only to be used as an indication of what type of value needs to be placed for the selected parameter:

+ bool = boolean
+ char = character
+ clr = color
+ dtt = datetime
+ dbl = double
+ obj = object
+ int = integer
+ str = string
+ ... = anything

Some function parameter values have options and this has been distinguished with the available values possible with each value separated by a pipe symol "|". If a parameter value has a default value this is distinguished as a parameter option with an asterisk "*" (eg. ExampleFunction( bool check=TRUE*|FALSE)) or as a lone paramater value (eg. AnotherExampleFunction( str me="Alone" )).

The easiest way to cycle through parameter values is to use the TAB key on your keyboard.


Templates (as of v1.1.0)
------------------

Besides functions, parameters, data types and reserved keywords which are populated in the code hinting box we also have basic templates added.

By entering in `expertstart` the user can get a blank template for writing their expert advisor, as shown here:

```
//+------------------------------------------------------------------+
//| Test.mq4
//| Copyright 2013, MetaQuotes Software Corp.
//| http://www.metaquotes.net
//+------------------------------------------------------------------+
#property copyright "Copyright 2013, MetaQuotes Software Corp."
#property link      "http://www.metaquotes.net"

//--- input parameters
extern int       ExtParam1=0;
extern int       ExtParam2=0;
//+------------------------------------------------------------------+
//| expert initialization function                                   |
//+------------------------------------------------------------------+
int init()
  {
//----

//----
   return(0);
  }
//+------------------------------------------------------------------+
//| expert deinitialization function                                 |
//+------------------------------------------------------------------+
int deinit()
  {
//----

//----
   return(0);
  }
//+------------------------------------------------------------------+
//| expert start function                                            |
//+------------------------------------------------------------------+
int start()
  {
//----

//----
   return(0);
  }
//+------------------------------------------------------------------+
```

Users can also add core individual templates by entering `init`, `deinit` or `start` in the text editor.


Feature Requests
----------------

If you any feature requests or amendments to be made to the code please let me know!!

Find me now at [Robot Trading Forex](https://robottradingforex.com)
