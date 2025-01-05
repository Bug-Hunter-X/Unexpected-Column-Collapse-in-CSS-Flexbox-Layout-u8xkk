# Unexpected Column Collapse in CSS Flexbox Layout

This repository demonstrates a common yet subtle issue encountered when using CSS Flexbox for two-column layouts.  The second column unexpectedly collapses, despite assigning a width. This occurs due to the interplay between `flex: 1` and a specified `width`.  The solution involves adjusting the flex property to resolve the conflict.

## Bug Report

The `bug.css` file contains CSS code designed to create a two-column layout using Flexbox. However, in some browsers, the second column fails to occupy its designated width of 300px, collapsing instead.

## Solution

The `bugSolution.css` file provides a corrected version of the CSS, resolving the column collapse issue. This is achieved by modifying the flex property of the second column to ensure its width is respected, instead of it inheriting the `flex: 1` of its parent. 