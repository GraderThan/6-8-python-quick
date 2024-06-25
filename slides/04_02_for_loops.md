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

# 🔄 For Loops in Python

- Repeat code a set number of times 🎯
- Iterate over sequences like lists 📋

<!-- 
- Introduce for loops as a powerful tool for repeating tasks.
- Highlight the simplicity and efficiency of automating repetitive actions.
-->
---
### 🌈 Using `for` loops with `range()`

```python
for i in range(5):
    print(i)
```
`range(n)` creates a sequence from 0 to n-1 🚦
Loops through numbers 0 to 4 🖐️
<!-- 
- Demonstrate how to use range() in a for loop.
- Explain that range(n) generates numbers from 0 up to, but not including, n.
-->
---
### Customizing range() 🎛️
Start and stop: `range(2, 6)` ➡️ 2 to 5
Adding a step: `range(0, 10, 2)` ➡️ Even numbers
```python
for i in range(2, 6):
    print(i)  # 2 to 5
for i in range(0, 10, 2):
    print(i)  # 0, 2, 4, 6, 8
```
<!-- 
- Explain how range() can be customized with start, stop, and step parameters.
- Provide code examples to illustrate the flexibility of range() in controlling loop iterations.
-->
---

### 🛑 Using `break` to Exit Loops

```python
for i in range(10):
    if i == 5: 
        break
    print(i)  # Stops at 4
```

`break` exits the loop early
<!-- 
- The break statement exits the loop early, stopping at 4 in this example.
- Great for stopping a loop when a specific condition is met.
-->

---

### ➡️ Skipping with `continue`

```python
for i in range(10):
    if i % 2 == 0: continue
    print(i)  # Odd numbers only
```
`continue` skips over the rest of the loop once
<!-- 
- Continue skips the rest of the loop's body and continues with the next iteration.
- Useful for skipping certain conditions, like even numbers here.
-->

---

# Turtle Challenges 🐢

---
### Exercise 1: Draw a Square 🟦

```python
from ipyturtle import Turtle

t = Turtle()

for i in range(4):
    t.forward(100)  # Move forward 100 units
    t.right(90)     # Turn right by 90 degrees
```

<!-- 
- Use the loop to repeat the logic of constructing a side 4 times
-->

---

### Exercise 2: Draw a Circle using Small Lines 🔴

```python
t = Turtle()

for i in range(36):
    t.forward(10)
    t.right(10)
```

<!-- 
- A circle can be drawn by turning the turtle slightly and moving a small distance
multiple times in a loop.
-->
---
### Exercise 3: Draw a Star ⭐

```python
t = Turtle()

for i in range(5):
    t.forward(100)
    t.right(144)
```

<!-- 
Think of how to construct one side of the star and set up for the next side, then repeat it 5 times
 -->