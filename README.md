# CSS Specificity Gotcha: Unexpected Overriding Due to Combined ID and Class Selectors

This repository demonstrates a subtle but important issue related to CSS specificity.  A class selector added to an ID selector increases the specificity, leading to unexpected style overriding.  The `bug.css` file contains the problematic code, while `bugSolution.css` offers a solution.

Understanding CSS Specificity:
CSS specificity determines which styles are applied when multiple selectors apply to the same element.  Generally, ID selectors (#) are highly specific.  However, adding a class selector (.) increases the specificity even further.

The Problem:
The issue arises when an ID selector is combined with a class selector in a way that unexpectedly overrides a more intuitive selector with higher specificity (in this case, the more simple id selector).

The Solution:
The solution focuses on understanding the specificity rules and either restructuring the CSS selector or appropriately altering style precedence.