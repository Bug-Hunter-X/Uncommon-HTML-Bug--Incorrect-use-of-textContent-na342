# Uncommon HTML Bug: Incorrect use of textContent

This repository demonstrates a subtle bug related to using `textContent` to modify the content of an HTML element that contains other elements.  The `textContent` property is designed to work with plain text nodes, and will not correctly update the content if nested elements are present. `innerText` is recommended when you want to set the visible text, regardless of the content's underlying structure.

## Bug Description:
The original `bug.html` file attempts to change the text content of a div using `textContent`.  However, this fails to update the displayed text because the div contains other elements, resulting in unexpected behaviour.

## Solution:
The `bugSolution.html` file shows how to correctly modify the displayed text of the div using the `innerText` property. `innerText` handles nested elements properly.
