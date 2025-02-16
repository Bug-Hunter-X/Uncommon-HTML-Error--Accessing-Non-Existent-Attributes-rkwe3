# Uncommon HTML Error: Handling Non-Existent Attributes

This repository demonstrates a subtle error that can occur when working with HTML attributes and provides best practices for avoiding it.

## The Problem

The `getAttribute()` method in JavaScript returns `null` if the specified attribute does not exist on an element.  If you don't handle this case correctly, your code might throw an error or produce unexpected results.

## The Solution

Always check if `getAttribute()` returns `null` before using the retrieved value.  Alternatively, use `dataset` for more concise access, but remember to check for `undefined` in that case as well.

## How to Run

1. Clone this repository.
2. Open `bug.html` in a web browser to see the error in action.
3. Open `bugSolution.html` to see the corrected version.