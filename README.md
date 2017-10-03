# Card - from CSV to print faster

Simple browser based card generator for faster prototyping of boardgames. I designed this as a single HTML file with embedded CSS and JavaScript, to make it easier for you to download, modify and run offline.

[Try it now!](http://htmlpreview.github.io/?https://github.com/vildninja/card/blob/master/index.html)

## How to Use

The tool has three text fields where you can fill in data:
* **CSS** The style of the cards. I have provided a basic example, but it should be easy to modify to your liking without too much effort. Read more about positioning elements on [w3scools.com/css](https://www.w3schools.com/css/css_positioning.asp).
* **HTML** The template of the cards. The content of this box will be duplicated for every line in the CSV document. To insert text from the CSV document simlpy write *%label%* in the template. Read more about HTML on [w3schools.com/html](https://www.w3schools.com/html/html_blocks.asp).
* **CSV** The comma seperated values. Any spread sheet editor should support export to this format. The first row of data should allways be the labels used to reference the data from the template (using *%label%*).

**You should edit CSS and HTML in an external text editor!** While your browser might remember what you have typed in the text fields, my tool does nothing to save your changes.

## The Code

The CSV parser is written by [Kash Nouroozi](https://github.com/knrz/CSV.js/tree/dev).

The rest is written by me.

The code contains two JavaScripts: the "compiled" CSV parser and my GenerateCards() function. The GenerateCards() function is where you should be looking if you want to make any additions. Further more I have included some CSS to hide everything but the cards from the printer + telling the printer to print as is (by default printers ignore background colors and images).

*Happy prototyping :)*

*/Jannek*
