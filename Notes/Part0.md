# Fundamentals of Web Apps

1st rule of web development: 
* Always keep the developer console on your web browser
* On macOS: option-cmd-i

The most important tabs are **Network** and **Console**

HTTP GET
* The server and the web browser communicate with each other using the HTTP protocol. The Network tab shows how the browser and network communicate

When the example webpage is loaded, we see there are two events. The browser fetches the contents of the page, and then downloads the image. Because the contents of the page contains an img tag, the browser makes a second HTTP-request to fetch the image. It may be difficult to notice, but the page begins to render before the image has been fetched.

Traditional web applications
* The homepage of the example works as a traditional web application
    * When entering the page, the browser fetches the HTMl document detailing the structure and content.
* The contents of the HTML page are saved as a template string, which allows for variables in the midst of it
* Writing HTML in the midst of code is not smart, but for old-school PHP-programmers it was a normal practice

DOM (Document Object Model)
* We can think of HTML-pages as implicit tree structures
* DOM is an API which enables programmtic modification of the lement trees corresponding to web-pages

Manipulating the DOM from console
* The topmost node of the DOM tree of an HTML document is called the document object. We can perform various operations on a web-page using the DOM-API
* Access the document object by typing document into the Console-tab

AJAX (Asynchronous Javascript and XML)
* enables the fetching of content to web pages using JS included within the HTML without the need to rerender the page

Single page app
* A style of creating web-applications
* SPA-style websites don't fetch all their pages separately from the server, instead comprises of only one HTML pages fetched from the server, the contents of which are manipulated with Javascript that executes in the browser
