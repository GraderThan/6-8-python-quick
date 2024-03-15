---
marp: true
author: Grader Than Technology LLC
title: "Variables"
theme: uncover
lang: en
size: 16:9
header: ![Grader Than Logo w:40](./images/gt-logo.png)
footer: <a href="https://www.graderthan.com/">GraderThan.com</a>
enableHtml: true
style: |
    header img {
        float: left;
    }
    footer {
        font-weight: 500;
        color: #4178bc;
        padding: 10px;
    }
    footer a {
        color: #4178bc;
    }
    pre code {
        padding: .7rem !important;
        border-radius: 8px;
    }
---
# Functions in Python 📠
---
## What are Functions❓
- Functions group code for a specific task
- They make code organized, reusable, and easier to read

<!-- 
- Speaker Note: Emphasize that functions are fundamental in programming for code organization and reuse.
- Speaker Note: Highlight that we'll learn how to create and use functions in Python.
-->

---

## Creating Functions ⚙️

```python
def greet():
    print("Hello, world!")
```

- `def greet()`: Defines a function named `greet`.
- Functions must be called to execute.

<!-- 
- Speaker Note: Explain `def` keyword, function name, parentheses, and colon.
- Speaker Note: Stress the importance of indentation in Python, as it defines the function's body.
- Speaker Note: Mention that defining a function doesn't execute it; calling it does.
-->

---

## Calling a Function 📱

```python
def greet():
    print("Hello, world!")

greet()
```

- Defining `greet` function.
- Calling `greet` prints "Hello, world!".

<!-- 
- Speaker Note: Show the actual code to define and then call the `greet` function.
- Speaker Note: Explain that after defining a function, calling it by its name followed by parentheses executes all the code within its body.
-->
---
## Passing Arguments ⚽

```python
def greet(name):
    print("Hello, " + name + "!")

greet("John")
```

- Demonstrates passing a single argument to a function.

<!-- 
- Speaker Note: Explain how arguments allow functions to perform tasks with different inputs.
- Speaker Note: Show how to define a function that accepts arguments and how to call it.
- The example `greet("John")` prints out "Hello, John!"
-->
---
## Passing Many Arguments ⚽🏀

```python
def multiply(a, b):
    print(a * b)
```
- To pass multiple arguments separate them with commas
---
## Return Values

```python
def add(a, b):
    return a + b
```

- `return a + b`: The function returns the sum of `a` and `b`.
- Functions can send Python objects back to the caller.

<!-- 
- Speaker Note: Highlight the use of `return` to send back a result from a function.
- Speaker Note: Mention that not all functions need to return something explicitly; without `return`, Python automatically returns `None`.
-->
---
## What Can Go In Functions 🌈
- Variables
- If/else
- Loops (while and for)
- Anything else we've learned so far
---
## Variables in Functions 📈

- Variables in functions are stored separately
- Use arguments and return values to share info

<!-- Explain how you can have the same variable name in multiple functions and they can all have different values
Each function is like its own bubble. To get info from one bubble to another, we use return values and arguments 
-->
---
# Turtle Challenges 🐢
---
## Drawing a Square 🟪


- Use a function to draw a square with turtle graphics.
- Function must accept the turtle and the square size

<!-- 
- Point out how we have already drawn a square using turtle, we just need to put that logic into a function and call it
-->

---

## Draw N Squares 🟪🟦🟥

- Use a function to draw n squares where n is any number
- Function must accept the turtle and the number of squares

<!-- 
- Speaker Note: Students will need to use for loops to accomplish this, where the size of each square is some multiple of i
- 
-->
