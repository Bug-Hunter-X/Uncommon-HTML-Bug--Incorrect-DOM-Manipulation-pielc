# Uncommon HTML Bug: Incorrect DOM Manipulation

This repository demonstrates a common mistake when manipulating the DOM in HTML using JavaScript.  The bug involves incorrectly attempting to modify the content of a div element and inefficiently retrieving it. The solution showcases the correct way to achieve the desired effect.

## Bug
The primary issue is the misuse of `textContent` on a div element.  `textContent` is designed to set the plain text content, whereas `innerHTML` allows for HTML content.  Additionally, using `getElementsByTagName` to retrieve a single element when its ID is known is inefficient;  `getElementById` should be used instead.

## Solution
The solution corrects these issues by using `innerHTML` to set the content of the div element and by using `getElementById` to retrieve the element efficiently.

## How to run the code:
1. Clone the repository.
2. Open `bug.html` in a web browser to observe the incorrect behavior.
3. Open `bugSolution.html` to see the corrected version.