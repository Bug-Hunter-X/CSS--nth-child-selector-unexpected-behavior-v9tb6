# CSS :nth-child Selector Unexpected Behavior

This repository demonstrates a common mistake when using the `:nth-child` pseudo-class in CSS to style list items.  The issue arises from a misunderstanding of how the selector works, particularly when attempting to style every other item starting from a specific index.

## The Problem

The `bug.css` file contains CSS that intends to style every other list item starting from the second one. However, due to an incorrect use of `:nth-child`, only even-numbered items are styled. This is because `2n` selects every even-numbered element, instead of every other element after the first.

## The Solution

The `bugSolution.css` file shows the corrected CSS using `2n+1`, ensuring every other list item (starting from the second) is correctly styled.

## How to Reproduce

1. Clone the repository.
2. Open the `index.html` file (which contains an unordered list) in your web browser.
3. Observe that the styling in `bug.css` only highlights the even-numbered list items. 
4. Replace `bug.css` with `bugSolution.css` and observe the corrected styling.