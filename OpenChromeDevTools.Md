# Open Chrome DevTools

There are many ways to open Chrome DevTools, because different users want fast access to different parts of the DevTools UI.

Open the Elements panel to inspect the DOM or CSS 
When you want to inspect a DOM node's styles or attributes, right-click the element and select Inspect.

The Inspect option
Figure 1. The Inspect option

Or press Command+Option+C (Mac) or Control+Shift+C (Windows, Linux, Chrome OS).

See Get Started With Viewing And Changing CSS.

Open the Console panel to view logged messages or run JavaScript 
Press Command+Option+J (Mac) or Control+Shift+J (Windows, Linux, Chrome OS) to jump straight into the Console panel.

See Get Started With The Console.

Open the last panel you had open 
Press Command+Option+I (Mac) or Control+Shift+I.

Open DevTools from Chrome's main menu 
Click Customize and control Google Chrome Customize and control Google Chrome and then select More Tools > Developer Tools.

Opening DevTools from Chrome's main menu.
Figure 2. Opening DevTools from Chrome's main menu

Auto-open DevTools on every new tab 
Open Chrome from the Command line and pass the --auto-open-devtools-for-tabs flag.

Mac:

/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --auto-open-devtools-for-tabs
This will only work if an instance of Chrome is not already running. From then on, every new tab will automatically open DevTools until the user fully quits Chrome.

[Artigo original](https://developer.chrome.com/docs/devtools/open/)