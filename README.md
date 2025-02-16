# Uncommon HTML Bugs

This repository demonstrates two subtle but potentially problematic HTML errors:

1. **Accessing a Non-Existent Element:** Attempting to manipulate the content of an element using `getElementById` or similar methods when that element does not exist on the page will result in a runtime JavaScript error.  This can be difficult to debug if you're not carefully checking for the element's existence before modifying it.
2. **Missing Closing Tag:**  Leaving a closing tag off, such as `</p>`, can lead to unpredictable results with how the rest of your HTML renders. The browser will try to recover but the result might not be what you intended.  This can cause formatting issues and possibly affect the behavior of JavaScript interacting with the DOM.

The `bug.html` file contains the buggy code.  The `bugSolution.html` shows how to correct these errors.