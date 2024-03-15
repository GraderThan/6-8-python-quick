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
# While Loops 🔁
---
# Understanding Loops in Python

- Loops allow repeated execution of code based on a condition.
- `while` loops continue as long as their condition is true.

<!-- 
- This slide introduces the concept of loops in Python, focusing on how they enable repetitive tasks through a conditional framework.
- Discuss the importance of loops in automating tasks and handling repetitive actions efficiently in programming.
-->

---
# While Loop Syntax
```
while some_condition:
    #do some action
```
- Looks similar to if statement
- Checks the condition
- Repeats the action as long as the condition is true
---
# Basic While Loop Pattern

- Initialize a variable before the loop starts.
- The loop runs as long as a condition is met.
- Update the variable within the loop to avoid infinite loops.
```
counter = 0
while counter < 5:
    print(f"The count is {counter}")
    counter += 1
```

<!-- 
- Explain the structure of a while loop, emphasizing initialization, condition checking, and updating the variable.
- Highlight the risk of infinite loops if the condition never becomes false and how updating the variable within the loop prevents this.
-->

---

# Control Statements: Break and Continue

- `break` exits the loop immediately.
- `continue` skips to the next iteration of the loop.

---
# Example using Break and Continue
```
counter = 0
while counter < 5:
    if counter == 1:
        continue
    if counter == 3:
        break
    print(f"The count is {counter}")
    counter += 1
```


<!-- 
- See if students can determine the output (0 and 2)
- Discuss how `break` and `continue` control the flow within loops.
- break exits the loop immediately
- continue skips to the next iteration
- Provide examples or scenarios where using `break` and `continue` can be useful in managing loop execution effectively such as if you encounter an error, or want to skip over something (odd nums, even nums, etc.)
-->

---
# Turtle Challenges 🐢
---
# Exercise 1: Drawing a Square with Turtle 🟦

- Use a `while` loop to draw a square.
- Increment a counter to repeat the drawing process 4 times.

<!-- 
- Introduce the turtle graphics library as a fun way to learn about loops.
- Explain how each iteration of the loop draws one side of the square and how the loop facilitates drawing a complete square.
-->

---

# Exercise 2: Creating a Spiral with Turtle 🌀

- Draw a spiral pattern by gradually increasing the distance the turtle moves.

<!-- 
- Encourage experimenting with different distances and angles to see how it affects the spiral's appearance.
-->
