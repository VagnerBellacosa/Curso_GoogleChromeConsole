# View and change CSS

View an element's CSS
Add a CSS declaration to an element
Add a CSS class to an element
Add a pseudostate to a class
Change the dimensions of an element
Complete these interactive tutorials to learn the basics of viewing and changing a page's CSS using Chrome DevTools.

View an element's CSS 
Right-click the Inspect Me! text below and select Inspect. The Elements panel of DevTools opens. The Inspect Me! element is highlighted in the DOM Tree.
In the DOM Tree, find the value of the data-message attribute for the Inspect Me! element.
Enter the value in the text box below.
The Styles tab on the Elements panel lists the CSS rules being applied to whatever element is currently selected in the DOM Tree, which should still be the Inspect Me! element in this case. Find the aloha class rule. The fact that you see this rule means that it's being applied to the Inspect Me! element.
The aloha class is declaring a value for padding. Enter that value in the text box below.
The inspected element is highlighted in the DOM Tree
Figure 1. The inspected element is highlighted blue in the DOM Tree

If you'd like to dock your DevTools window to the right of your viewport, like you see in Figure 1, see Change DevTools placement.

CSS classes being applied to the inspected element are highlighted in the Styles tab
Figure 2. CSS classes being applied to the selected element, such as aloha, are displayed in the Styles tab

Add a CSS declaration to an element 
Use the Styles tab when you want to change or add CSS declarations to an element.

Note: Complete the View an element's CSS tutorial before doing this one.

Right-click the Add A Background Color To Me! text below and select Inspect.
Click element.style near the top of the Styles tab.
Type background-color and press Enter.
Type honeydew and press Enter. In the DOM Tree you can see that an inline style declaration was applied to the element.
Adding a CSS declaration to the element via the Styles tab
Figure 3. The background-color:honeydew declaration has been applied to the element via the element.style section of the Styles tab

Add a CSS class to an element 
Use the Styles tab to see how an element looks when a CSS class is applied to or removed from an element.

Note: Complete the View an element's CSS tutorial before doing this one.

Right-click the Add A Class To Me! element below and select Inspect.
Click .cls. DevTools reveals a text box where you can add classes to the selected element.
Type color_me in the Add new class text box and then press Enter. A checkbox appears below the Add new class text box, where you can toggle the class on and off. If the Add A Class To Me! element had any other classes applied to it, you'd also be able to toggle them from here.
Applying the color_me class to the element
Figure 4. The color_me class has been applied to the element via the .cls section of the Styles tab

Add a pseudostate to a class 
Use the Styles tab to permanently apply a CSS pseudostate to an element. DevTools supports :active, :focus, :hover, and :visited.

Note: Complete the View an element's CSS tutorial before doing this one.

Hover over the Hover Over Me! text below. The background color changes.
Right-click the Hover Over Me! text and select Inspect.
In the Styles tab, click :hov.
Check the :hover checkbox. The background color changes like before, even though you're not actually hovering over the element.
Toggling the hover pseudostate on an element
Figure 5. Toggling the :hover pseudostate on an element

Change the dimensions of an element 
Use the Box Model interactive diagram in the Styles tab to change the width, height, padding, margin, or border length of an element.

Note: Complete the View an element's CSS tutorial before doing this one.

Right-click the Change My Margin! element below and select Inspect.

In the Box Model diagram in the Styles tab, hover over padding. The element's padding is highlighted in the viewport.

Note: Depending on the size of your DevTools window, you may need to scroll to the bottom of the Styles tab to see the Box Model.

Double-click the left margin in the Box Model, which currently has a value of - meaning that the element doesn't have a left-margin.

Type 100 and press Enter. The Box Model defaults to pixels, but it also accepts other values, such as 25%, or 10vw.

Hovering over the element's padding
Figure 6. Hovering over the element's padding

Changing the element's left-margin
Figure 7. Changing the element's left-margin

[Artigo original](https://developer.chrome.com/docs/devtools/css/#view)