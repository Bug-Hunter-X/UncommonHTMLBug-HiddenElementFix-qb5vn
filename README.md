# Uncommon HTML Bug: Incorrect Element Hiding

This repository demonstrates a subtle bug related to hiding HTML elements using JavaScript.  The incorrect approach can lead to unexpected layout issues.

## Bug Description
The bug lies in the way the `myDiv` element is hidden. Using `style.display = 'hidden'` maintains the space the element occupies, creating a potential layout issue if the hidden element's height was significant. This subtle error can be difficult to debug.

## Solution
The correct approach is to use `style.visibility = 'hidden'` to hide the element without removing the occupied space or  `style.display = 'none'` to remove the space completely.