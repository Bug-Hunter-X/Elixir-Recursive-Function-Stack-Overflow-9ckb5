# Elixir Recursive Function Stack Overflow

This repository demonstrates a common error in Elixir: a stack overflow caused by a recursive function lacking a proper base case. The `bug.exs` file contains the faulty code, while `bugSolution.exs` provides a corrected version.

## Description

The original code attempts to traverse a deeply nested list recursively. However, it fails to define a base case to stop the recursion when it reaches the innermost elements. This leads to infinitely nested function calls, eventually exhausting the stack and resulting in a stack overflow error.

## Solution

The solution involves adding a base case to the recursive function.  The corrected function checks if the input is a list. If it's not, it means we reached the innermost element and can terminate the recursion, processing that element.

## How to run

1.  Clone this repository.
2.  Make sure you have Elixir installed.
3.  Run `elixir bug.exs` to see the stack overflow error.
4.  Run `elixir bugSolution.exs` to see the corrected version in action.
