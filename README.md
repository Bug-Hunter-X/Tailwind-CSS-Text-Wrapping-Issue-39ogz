# Tailwind CSS Text Wrapping Bug

This repository demonstrates a bug encountered when using Tailwind CSS for text wrapping.  Text within a div element does not wrap correctly, even when there's ample horizontal space.  The issue is likely related to the interplay of flexbox, the parent container's size, and perhaps missing or conflicting Tailwind directives.  The solution provided addresses the issue by explicitly setting the width of the inner div to ensure proper wrapping occurs.

## Steps to Reproduce
1. Clone the repository.
2. Open `bug.html` in your browser.
3. Observe the text in the inner div, noticing how the long line does not wrap.
4. Open `bugSolution.html` to see the corrected code that resolves the issue.

## Solution
The bug is resolved by setting a `max-w-full` class to the inner div. This will allow the text to wrap to the available width of the parent container.