## Programming with Javascript - Read 07

## Control flow
The control flow is the order in which the computer executes statements in a script.

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:

if (isEmpty(field)) {
  promptUser();
} else {
  submitForm();
}

## Types of JavaScript Operators

**There are different types of JavaScript operators:**

Arithmetic Operators
Assignment Operators
Comparison Operators
Logical Operators
Conditional Operators
Type Operators

## JavaScript Functions
A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

## JavaScript Function Syntax
A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses ().

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: {}

## Function Invocation
The code inside the function will execute when "something" invokes (calls) the function:

When an event occurs (when a user clicks a button)
When it is invoked (called) from JavaScript code
Automatically (self invoked)

## Why Functions?
You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.

## JavaScript Assignment Operators
Assignment operators assign values to JavaScript variables.

The Addition Assignment Operator (+=) adds a value to a variable.

## Things I want to know more about

- how to identify improper function
- how to fix/correct functions and operators
