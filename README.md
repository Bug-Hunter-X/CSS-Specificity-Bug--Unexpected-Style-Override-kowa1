# CSS Specificity Bug: Unexpected Style Override

This repository demonstrates a subtle but important bug related to CSS specificity. The issue revolves around the unexpected behavior that can occur when combining ID and class selectors, leading to unexpected styling overrides.

## Bug Description
The bug stems from the higher specificity of ID selectors compared to class selectors.  When an element has both an ID and a class, and conflicting styles are defined for both, the ID selector's style will always take precedence.

## How to Reproduce
1. Open `bug.css`.
2. Observe the unexpected styling of the element with both the ID `myElement` and class `myElement`.
3. Compare it to the expected styling based on the class selector alone.

## Solution
The solution involves understanding and carefully managing CSS specificity. In this case, ensuring that the class selector is more specific can prevent the issue.  See the solution in `bugSolution.css`.

## Lessons Learned
This example underscores the need to understand CSS specificity rules thoroughly. Careful consideration of selector specificity is essential for predictable and consistent styling.