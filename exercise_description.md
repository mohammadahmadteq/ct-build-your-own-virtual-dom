# Build your own Virtual DOM

## Overview:

Virtual Document Object Model (DOM) is a concept used by modern web frameworks such as React, Vue, and Angular to optimize web application performance. By using a Virtual DOM, changes in the application state are first reflected in the Virtual DOM, which then updates the actual DOM. This way, the framework only updates the necessary parts of the DOM, reducing the number of expensive DOM manipulations required.

Here are general steps of how a virtual DOM funcions:

1. When a user interacts with a web application, the virtual DOM is updated with the new state of the application.
2. The virtual DOM then compares the updated state with the previous state to determine what has changed.
3. Once the changes have been identified, the virtual DOM creates a minimal set of instructions (known as a "diff") that are required to update the real DOM.
4. Finally, the real DOM is updated with the changes, and the web page is re-rendered to reflect the new state of the application.

Performing this exercise will be helpful to front-end developers because it will provide a hands-on opportunity to understand and implement one of the core concepts used by modern web frameworks to optimize web application performance. Building your own Virtual DOM library will help you to gain a deeper understanding of how Virtual DOM works and how to leverage its benefits to improve web application performance. By completing this exercise, you will be better equipped to make informed decisions about which libraries and frameworks to use for your own projects, and to develop more efficient, performant web applications.


## Implementation Details:

The DOM is usually represented as a tree in the browser, as you can see in the image down below:

![image](https://user-images.githubusercontent.com/114756286/222674145-d5d6685e-590e-4f0b-97b4-4778217a9460.png)

Each node in the tree represents an HTML element, these elements can have branches that have child elements, Each node apart from containing their children has certain other properties which are known as attributes, these attributes could be things like href, source image (src) etc. The HTML in the browser is then rendered top to bottom.

This tree can be represented as an object in Javascript, here is an example object representation of a react virtual DOM.

<div id="main">
<div id="header">
<h1 id="heading">
Hello World </h1>
<p_id="paragraph">  Building VDOM </p>
  </div>
  </div>

## Exercise Details:
In this exercise you should implement a Virtual DOM library using JavaScript or TypeScript. The library should have the following functionality:

1. Create virtual nodes with a given tag name and attributes.
2. Create a virtual text node with a given text content.
3. Append a child virtual node to a parent virtual node.
4. Remove a child virtual node from a parent virtual node.
5. Update the attributes or text content of a virtual node.
6. Diff two virtual nodes and return a list of patches to be applied to the actual DOM.

To complete the exercise, you should create a simple web page that uses your Virtual DOM library to render dynamic content. This could be a simple counter that updates on button clicks along with an input box and a button which when clicked updates the header of the page. Your Virtual DOM library should be designed to handle changes to the application state efficiently, updating only the necessary parts of the DOM to improve performance.
