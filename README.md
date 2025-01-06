# Uncommon HTML Bug: Accessing Non-Existent Attributes

This repository demonstrates a subtle bug that can occur in HTML when dealing with DOM elements and their attributes. The bug arises from attempting to directly access an attribute that does not exist on an element.  This can lead to unexpected `null` values or runtime errors.

## The Bug
The `bug.html` file shows the problem. We try to access a non-existent attribute ("nonExistentAttr") directly. This will return `null`, but any further operations on it might throw errors. 
The solution, shown in `bugSolution.html`, demonstrates the proper ways to handle attribute access and setting them.

## Solution
The correct approach is to use the `getAttribute()` method to safely retrieve attribute values or `setAttribute()` method to add or update them.  Alternatively, you can assign values directly using attribute property for modern browsers. 

## How to reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser. Observe the output in the browser's console. 
3. Open `bugSolution.html` to see how to correctly handle attribute access and setting them.