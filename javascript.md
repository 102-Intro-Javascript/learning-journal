# Javascript

## Chapter 1
* It is best to keep JavaScript code in its own JavaScript
file. JavaScript files are text files (like HTML pages and
CSS style sheets), but they have the . j s extension.
* The HTML script element is used in HTML pages
to tell the browser to load the JavaScript file (rather like
the link element can be used to load a CSS file).
* If you view the source code of the page in the browser,
the JavaScript will not have changed the HTML,
because the script works with the model of the web
page that the browser has created.

<!DOCTYPE html>
<html>
    <head>
        <title>Constuctive &amp; Co.</title>
        <link rel="stylesheet" href="css/c01.css"/>
    </head>
    <body>
        <h1>Constructive &amp; Co.</h1>
        <script src="js/add-content.js"></script>
        <p>for all orders and inquiries please call 
            <em>555-3344</em>
        </p>
    </body>
</html>

var today = new Date();
var hourNow = today.getHours();
var greeting;

if (hourNow > 18) {
    greeting = 'Good Evening!';
} else if (hourNow > 12) {
    greeting = 'Good Afternoon!';
} else if (hourNow > 0) {
    greeting = 'Good Morning!';
} else {
    greeting = 'Welcome!';
}

document.write('<h3>' + greeting + '</h3>');