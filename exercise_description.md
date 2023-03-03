##Description:
In this exercise, you will build your own Virtual DOM library. The Virtual DOM is a concept used by modern web frameworks such as React, Vue, and Angular to optimize web application performance. By using a Virtual DOM, changes in the application state are first reflected in the Virtual DOM, which then updates the actual DOM. This way, the framework only updates the necessary parts of the DOM, reducing the number of expensive DOM manipulations required.

##Problem Statement:
Your task is to implement a Virtual DOM library using JavaScript. The library should have the following functionality:

Create virtual nodes with a given tag name and attributes.
Create a virtual text node with a given text content.
Append a child virtual node to a parent virtual node.
Remove a child virtual node from a parent virtual node.
Update the attributes or text content of a virtual node.
Diff two virtual nodes and return a list of patches to be applied to the actual DOM.
To complete the exercise, you should create a simple web page that uses your Virtual DOM library to render dynamic content. This could be as simple as a counter that updates on button clicks, or as complex as a full web application with user interaction and state management. Your Virtual DOM library should be designed to handle changes to the application state efficiently, updating only the necessary parts of the DOM to improve performance.
