# Tailwind CSS @apply Directive: Conflicting Styles

This repository demonstrates a subtle bug related to Tailwind CSS's `@apply` directive when dealing with conflicting styles applied via custom utility classes.

## Problem

The `@apply` directive in Tailwind CSS provides a convenient way to reuse styles. However, when applying multiple custom utility classes that have conflicting styles, the order of application might unexpectedly influence the final result. This can be challenging to debug, especially in complex CSS structures.

The `bug.css` file contains an example illustrating the conflicting styles problem. In the given example, we'd expect `custom-width-override` to have priority, but this doesn't always happen.

## Solution

The `bugSolution.css` file provides a solution using CSS specificity to guarantee the intended styling override.