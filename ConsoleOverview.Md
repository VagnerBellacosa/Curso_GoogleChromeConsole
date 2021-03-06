# Console overview

This page explains how the Chrome DevTools Console makes it easier to develop web pages. The Console has 2 main uses: viewing logged messages and running JavaScript.

## Viewing logged messages 

Web developers often log messages to the Console to make sure that their JavaScript is working as expected. To log a message, you insert an expression like console.log('Hello, Console!') into your JavaScript. When the browser executes your JavaScript and sees an expression like that, it knows that it's supposed to log the message to the Console. For example, suppose that you're in the process of writing the HTML and JavaScript for a page:

-  [Console Demo.Html](ConsoleDemo.Html)

### shows what the Console looks like after loading the page and waiting 3 seconds. Try to figure out which lines of code caused the browser to log the messages.

Web developers log messages for 2 general reasons:

Making sure that code is executing in the right order.
Inspecting the values of variables at a certain moment in time.
See Get Started With Logging Messages to get hands-on experience with logging. See the Console API Reference to browse the full list of console methods. The main difference between the methods is how they display the data that you're logging.

### Running JavaScript 

The Console is also a REPL. You can run JavaScript in the Console to interact with the page that you're inspecting. For example, Figure 2 shows the Console next to the DevTools homepage, and Figure 3 shows that same page after using the Console to change the page's title.

Modifying the page from the Console is possible because the Console has full access to the page's window. DevTools has a few convenience functions that make it easier to inspect a page. For example, suppose that your JavaScript contains a function called hideModal. Running debug(hideModal) pauses your code on the first line of hideModal the next time that it's called. See Console Utilities API Reference to see the full list of utility functions.

When you run JavaScript you don't have to interact with the page. You can use the Console to try out new code that's not related to the page. For example, suppose you just learned about the built-in JavaScript Array method map(), and you want to experiment with it. The Console is a good place to try out the function.

[Original](https://developer.chrome.com/docs/devtools/console/#javascript)