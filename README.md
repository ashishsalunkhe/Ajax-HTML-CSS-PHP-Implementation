# Ajax-HTML-CSS-PHP-Implementation
# 1. PHP
The PHP Hypertext Preprocessor (PHP) is a programming language that allows web
developers to create dynamic content that interacts with databases. PHP is basically used for
developing web based software applications.
PHP has a total of eight data types which we use to construct our variables −
Integers − are whole numbers, without a decimal point, like 4195.
Doubles − are floating-point numbers, like 3.14159 or 49.1.
Booleans − have only two possible values either true or false.
NULL − is a special type that only has one value: NULL.
Strings − are sequences of characters, like &#39;PHP supports string operations.&#39;
Arrays − are named and indexed collections of other values.
Objects − are instances of programmer-defined classes, which can package up both
other kinds of values and functions that are specific to the class.
Resources − are special variables that hold references to resources external to PHP
# PHP MySQL Connectivity
<?php
$servername = "localhost";
$username = "username";
$password = "password";

// Create connection
$conn = new mysqli($servername, $username, $password);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
} 
echo "Connected successfully";
?>

# 2. AJAX
AJAX stands for Asynchronous JavaScript and XML. AJAX is a new technique for creating
better, faster, and more interactive web applications with the help of XML, HTML, CSS, and
Java Script.
 Ajax uses XHTML for content, CSS for presentation, along with Document Object
Model and JavaScript for dynamic content display.
 Conventional web applications transmit information to and from the sever using
synchronous requests. It means you fill out a form, hit submit, and get directed to a
new page with new information from the server.
 With AJAX, when you hit submit, JavaScript will make a request to the server,
interpret the results, and update the current screen. In the purest sense, the user would
never know that anything was even transmitted to the server.
 XML is commonly used as the format for receiving server data, although any format,
including plain text, can be used.
 AJAX is a web browser technology independent of web server software.
 A user can continue to use the application while the client program requests
information from the server in the background.
 Intuitive and natural user interaction. Clicking is not required, mouse movement is a
sufficient event trigger.
 Data-driven as opposed to page-driven.

# The XMLHttpRequest Object
All modern browsers support the XMLHttpRequest object. The XMLHttpRequest object can
be used to exchange data with a server behind the scenes. This means that it is possible to
update parts of a web page, without reloading the whole page.
var xhttp = new XMLHttpRequest();
Send a Request To a Server
To send a request to a server, we use the open() and send() methods of the XMLHttpRequest
object:
xhttp.open(&quot;GET&quot;, &quot;ajax_info.txt&quot;, true);
xhttp.send();
# Property Description
onreadystatechange Defines a function to be called when the readyState property changes
readyState Holds the status of the XMLHttpRequest. 
If readyState=
0: request not initialized 
1: server connection established
2: request received 
3: processing request 
4: request finished and response is ready

