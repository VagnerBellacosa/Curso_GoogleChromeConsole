# Console features reference

This page is a reference of features related to the Chrome DevTools Console. It assumes that you're already familiar with using the Console to view logged messages and run JavaScript. If not, see Get Started.

If you're looking for the API reference on functions like console.log() see Console API Reference. For the reference on functions like monitorEvents() see Console Utilities API Reference.

Open the Console 
You can open the Console as a panel or as a tab in the Drawer.

Open the Console panel 
Press Control+Shift+J or Command+Option+J (Mac).

The Console panel.
Figure 1. The Console panel.

To open the Console panel from the Command Menu, start typing Console and then run the Show Console command that has the Panel badge next to it.

The command for showing the Console panel.
Figure 2. The command for showing the Console panel.

Open the Console tab in the Drawer 
Press Escape or click Customize And Control DevTools Customize And Controls DevTools and then select Show Console Drawer.

Show Console Drawer.
Figure 3. Show Console Drawer.

The Drawer pops up at the bottom of your DevTools window, with the Console tab open.

The Console tab in the Drawer.
Figure 4. The Console tab in the Drawer.

To open the Console tab from the Command Menu, start typing Console and then run the Show Console command that has the Drawer badge next to it.

The command for showing the Console tab in the Drawer.
Figure 5. The command for showing the Console tab in the Drawer.

Open Console Settings 
Click Console Settings Console Settings.

Console Settings.
Figure 6. Console Settings.

The links below explain each setting:

Hide Network
Preserve Log
Selected Context Only
Group Similar
Log XmlHttpRequests
Eager Evaluation
Autocomplete From History
Open the Console Sidebar 
Click Show Console Sidebar Show Console Sidebar to show the Sidebar, which is useful for filtering.

Console Sidebar.
Figure 7. Console Sidebar.

View messages 
This section contains features that change how messages are presented in the Console. See View messages for a hands-on walkthrough.

Disable message grouping 
Open Console Settings and disable Group similar to disable the Console's default message grouping behavior. See Log XHR and Fetch requests for an example.

Log XHR and Fetch requests 
Open Console Settings and enable Log XMLHttpRequests to log all XMLHttpRequest and Fetch requests to the Console as they happen.

Logging XMLHttpRequest and Fetch requests.
Figure 8. Logging XMLHttpRequest and Fetch requests.

The top message in Figure 8 shows the Console's default grouping behavior. Figure 9 shows how the same log looks after disabling message grouping.

How the logged XMLHttpRequest and Fetch requests look after ungrouping.
Figure 9. How the logged XMLHttpRequest and Fetch requests look after ungrouping.

Persist messages across page loads 
By default the Console clears whenever you load a new page. To persist messages across page loads, Open Console Settings and then enable the Preserve Log checkbox.

Hide network messages 
By default the browser logs network messages to the Console. For example, the top message in Figure X represents a 404.

A 404 message in the Console.
Figure 10. A 404 message in the Console.

To hide network messages:

Open Console Settings.
Enable the Hide Network checkbox.
Filter messages 
There are many ways to filter out messages in the Console.

Filter out browser messages 
Open the Console Sidebar and click User Messages to only show messages that came from the page's JavaScript.

Viewing user messages.
Figure 11. Viewing user messages.

Filter by log level 
DevTools assigns each console.* method a severity level. There are 4 levels: Verbose, Info, Warning, and Error. For example, console.log() is in the Info group, whereas console.error() is in the Error group. The Console API Reference describes the severity level of each applicable method. Every message that the browser logs to the Console has a severity level too. You can hide any level of messages that you're not interested in. For example, if you're only interested in Error messages, you can hide the other 3 groups.

Click the Log Levels dropdown to enable or disable Verbose, Info, Warning or Error messages.

The Log Levels dropdown.
Figure 12. The Log Levels dropdown.

You can also filter by log level by opening the Console Sidebar and then clicking Errors, Warnings, Info, or Verbose.

Using the Sidebar to view warnings.
Figure 13. Using the Sidebar to view warnings.

Filter messages by URL 
Type url: followed by a URL to only view messages that came from that URL. After you type url: DevTools shows all relevant URLs. Domains also work. For example, if https://example.com/a.js and https://example.com/b.js are logging messages, url:https://example.com enables you to focus on the messages from these 2 scripts.

A URL filter.
Figure 14. A URL filter.

Type -url: to hide messages from that URL. This is called a negative URL filter.

A negative URL filter. DevTools is hiding all messages that match the URL https://b.wal.co
Figure 15. A negative URL filter. DevTools is hiding all messages that match the URL https://b.wal.co.

You can also show messages from a single URL by opening the Console Sidebar, expanding the User Messages section, and then clicking the URL of the script containing the messages you want to focus on.

Viewing the messages that came from wp-ad.min.js.
Figure 16. Viewing the messages that came from wp-ad.min.js.

Filter out messages from different contexts 
Suppose that you've got an ad on your page. The ad is embedded in an <iframe> and is generating a lot of messages in your Console. Because this ad is in a different JavaScript context, one way to hide its messages is to open Console Settings and enable the Selected Context Only checkbox.

Filter out messages that don't match a regular expression pattern 
Type a regular expression such as /[gm][ta][mi]/ in the Filter text box to filter out any messages that don't match that pattern. DevTools checks if the pattern is found in the message text or the script that caused the message to be logged.

Filtering out any messages that don't match /[gm][ta][mi]/.
Figure 17. Filtering out any messages that don't match /[gm][ta][mi]/.

Run JavaScript 
This section contains features related to running JavaScript in the Console. See Run JavaScript for a hands-on walkthrough.

Re-run expressions from history 
Press the Up Arrow key to cycle through the history of JavaScript expressions that you ran earlier in the Console. Press Enter to run that expression again.

Watch an expression's value in real-time with Live Expressions 
If you find yourself typing the same JavaScript expression in the Console repeatedly, you might find it easier to create a Live Expression. With Live Expressions you type an expression once and then pin it to the top of your Console. The value of the expression updates in near real-time. See Watch JavaScript Expression Values In Real-Time With Live Expressions.

Disable Eager Evaluation 
As you type JavaScript expressions in the Console, Eager Evaluation shows a preview of that expression's return value. Open Console Settings and disable the Eager Evaluation checkbox to turn off the return value previews.

Disable autocomplete from history 
As you type out an expression, the Console's autocomplete popup shows expressions that you ran earlier. These expressions are prepended with the > character. Open Console Settings and disable the Autocomplete From History checkbox to stop showing expressions from your history.

The autocomplete popup showing expressions from history.
Figure 18. document.querySelector('a') and document.querySelector('img') are expressions that were evaluated earlier.

Select JavaScript context 
By default the JavaScript Context dropdown is set to top, which represents the main document's browsing context.

The JavaScript Context dropdown.
Figure 19. The JavaScript Context dropdown.

Suppose you have an ad on your page embedded in an <iframe>. You want to run JavaScript in order to tweak the ad's DOM. To do this, you first need to select the ad's browsing context from the JavaScript Context dropdown.

Selecting a different JavaScript context.
Figure 20. Selecting a different JavaScript context.

Clear the Console 
You can use any of the following workflows to clear the Console:

Click Clear Console Clear Console.
Right-click a message and then select Clear Console.
Type clear() in the Console and then press Enter.
Call console.clear() from your webpage's JavaScript.
Press Control+L while the Console is in focus.

[Artigo original](https://developer.chrome.com/docs/devtools/console/reference/)