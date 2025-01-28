# Tailwind CSS @apply Directive Issue with Pseudo-classes

This repository demonstrates a bug with the Tailwind CSS `@apply` directive when used with pseudo-classes such as `:hover`, `:focus`, or `:active`.  The `@apply` directive, when used with such classes, will not apply styles correctly unless the pseudo-class condition is met.

## Bug Reproduction

1. Clone this repository.
2. Open `bug.css` to see the problematic code.
3. Notice that the button doesn't have the expected hover effect because of the way `@apply` interacts with the `:hover` state in this scenario.
4. Open `bugSolution.css` to see the workaround.

## Solution

Instead of using `@apply` with pseudo-classes directly within a class definition, define the pseudo-class styles directly in the class or use a different approach to manage the styling.