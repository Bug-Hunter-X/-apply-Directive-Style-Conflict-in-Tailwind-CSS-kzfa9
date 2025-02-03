# Tailwind CSS @apply Directive Conflict

This repository demonstrates a bug related to the `@apply` directive in Tailwind CSS. When using `@apply` within a class that also contains other styles, unexpected behavior can result due to the order in which Tailwind processes styles.  The `bug.css` file showcases the problem, while `bugSolution.css` provides a solution.

## Bug Description
The `@apply` directive in Tailwind CSS applies pre-defined utility classes.  However, if used within a class that already has styles defined, the order of processing can cause conflicts, leading to styles being unintentionally overwritten or omitted.

## Solution
The recommended solution is to separate `@apply` from other custom styles, either by creating separate utility classes or structuring your styles in a way to avoid conflicts.  See `bugSolution.css` for an example.