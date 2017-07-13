Highlight JS
============

Copyright
---------
Copyright © 2017 TNG Consulting Inc. - http://www.tngconsulting.ca/

This file is part of highlightJS

Highlight JS is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

Highlight JS is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with Highlight JS.  If not, see <http://www.gnu.org/licenses/>.

Authors
-------
Michael Milette - Lead Developer

Description
-----------
Highlight JS is a JavaScript that highlights search terms in the URL and
automatically scrolls down to the first instance found on the web page.
Great for search engine results.

IMPORANT: Although we expect everything to work, this ALPHA release has not been fully tested in every situation. If you find a problem, please help by reporting it in the [Bug Tracker](http://github.com/michael-milette/highlightjs/issues).

Changes
-------
The first public ALPHA version was released on 2017-07-12.

For more information on releases since then, see CHANGELOG.md.

Installation and Usage
----------------------
IMPORANT: Although we expect everything to work, this ALPHA release has not been fully tested in every situation. If you find a problem, please help by reporting it in the [Bug Tracker](http://github.com/michael-milette/highlightjs/issues).

For every page where you will want to apply this script, you will need to
include following HTML in the header section of every page:

    <style>.highlight { background: #FFFF40; }</style>
    <script type="text/javascript" src="highlight.js"></script>

Ensure the path to highlight.js is correct for every page that makes use of it.

You will also need to add an onload=highlight() attribute to the body tag:

    <body onload="highlight();">

If you don't have access to the body tag, add the following line within the
body of your page:

    <script type="text/javascript">window.onload = highlight();</script>

Optional Parameters

The highlight() function has several optional parameters available to change the way it works. These include:

* paramName: Default is 'q'. This string enables you to specify a different parameter name in URL query.
* className: Default is 'highlight'. This string enables you to specify a different class name for highlighting.
* doScroll: Default is true: If set to false, will disable automatic scrolling down to first search term found in the page.
* enableTabbing: Default is true. If set to false, will not create tab stops for each instance of the search term found in the page.

Usage

To specify one or more search term in the URL, simply add a "q" parameter and the search terms to the URL. Example:

http://www.example.com/search.html?q=search+terms

Security considerations
-----------------------
There are no known security issues at this time.

Motivation for this script
--------------------------
The development of this JavaScript was motivated through our experience with the Tipue search engine, the desire to have search terms highlighted in the results and to have the page automatically scroll down to the first search term on the page. The project is sponsored and supported by TNG Consulting Inc.

Limitations
-----------
The current version of highlightJS has been tested with up-to-date versions of most popular web browsers such as Chrome, Firefox, Safari, Edge and IE11. It could technically also be compatible with browsers that came out as far back 2012 however these have not been tested.

Future Releases
---------------
There are currently no plans for future releases however do let us know if you have any suggestions.

Further Information
-------------------
For further information regarding the highlightJS, support or to report a bug, please visit the project page at:

http://github.com/michael-milette/highlightjs

Language Support
----------------
This script has not been tested for right-to-left (RTL) language support.
If you find there is an issue with RTL as-is, feel free to prepare a pull request and submit it to the project page at:

http://github.com/michael-milette/highlightjs

Frequently Asked Questions (FAQ)
--------------------------------
IMPORANT: Although we expect everything to work, this ALPHA release has not been fully tested in every situation. If you find a problem, please help by reporting it in the [Bug Tracker](http://github.com/michael-milette/highlightjs/issues).

**Question: How can I do the autoscrolling without having the highlighing of instances of the search term?**

Answer: If you don't want highlighting but do want the autoscroll feature, simply set the class name to something that will not cause your CSS to apply highlighting (like 'nohighlight') and then use doScroll as you would normally.

**Question: I have a question that is not listed here**

Answer: Submit your question to the issue tracker. We will be happy to add the frequently asked questions and their answers to this section.

http://github.com/michael-milette/highlightjs/issues
