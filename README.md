# Uncommon HTML Bug: DOM Manipulation Before Load

This repository demonstrates a subtle but common error in HTML: attempting to manipulate the Document Object Model (DOM) before the page is fully loaded. This often happens when JavaScript code tries to access elements that haven't been parsed by the browser yet.

**The Bug:**
The `bug.html` file shows an example where JavaScript attempts to change the content of a `div` element *before* the browser has finished rendering the page. This results in the intended change not occurring.  The incorrect code attempts to access the DOM prematurely.

**The Solution:**
The `bugSolution.html` file provides a corrected version that uses the `DOMContentLoaded` event listener to ensure that the DOM is fully loaded before attempting to make changes to it. This guarantees that the changes occur as expected.