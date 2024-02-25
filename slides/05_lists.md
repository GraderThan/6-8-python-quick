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
# Python Lists 📋
---
## What Are Lists?
- Super-charged variables holding items under a single name.
- Can store different types of items, organizing data easily.

<!-- 
- this is a speaker note: Introduce Python lists as powerful tools for grouping multiple items under one name, making data organization simpler.
- this is another speaker note: Emphasize their ability to hold different types of data, which is useful for various programming tasks. 
-->

---

## Creating Lists ✨

- Put items between square brackets, separated by commas. Like this:

```python
new_list = ["hello", "there"]
```

<!-- 
- Explain how to create a list with a simple syntax.
- Highlight that lists can include multiple data types and maintain the order of items. 
-->

---

## Accessing List Elements 🔎

- Access items by their index, starting at 0.
- Use positive indexes for start, negative for end.

<!-- 
- Detail how to access list elements using indexes.
- Syntax looks like list_name[index]
- Mention the use of positive indexes for the beginning and negative indexes for accessing items from the end. 
-->

---

### Try it out!

```python
my_list = [1, 2, 3, "Python", "is", "fun"]
print(my_list[4]) # Outputs: is
print(my_list[-3]) # Outputs: Python
```

<!-- 
- Encourage students to access list elements using both positive and negative indexes.
- Provide a code example demonstrating how to access specific elements in a list. 
-->

---

## Adding and Removing From Lists ➕|➖

- Flexible: items can be added or removed after creation.
- Methods include `append`, `insert`, `remove`, and `pop`.

<!-- 
- Explain the flexibility of lists in Python, allowing items to be added or removed.
- Introduce methods for adding (`append`, `insert`) and removing (`remove`, `pop`) items. 
-->

---

### Appending To a List

- `my_list.append("awesome")` adds "awesome" to the end.

### Inserting Into a List

- `my_list.insert(0, "learning")` adds "learning" at the beginning.

<!-- 
- Show how to use `append` to add items to the end of a list.
- Demonstrate `insert` to add items at a specific position within a list. 
-->

---

### Removing an item by value

- `word_list.remove("mistake")` deletes first "mistake" found.

### Removing By Index

- `word_list.pop(3)` removes the item at index 3.

<!-- 
- Illustrate removing items by value with `remove`.
- Explain removing items by index using `pop` and its effect on the list. 
-->

---

## Checking if a Value is Inside a List 🕵️

- Use `in` keyword to check for item presence in a list.

<!-- 
- Teach how to use the `in` keyword to check if a specific item exists within a list.
- Emphasize the simplicity and usefulness of this operation for conditionals and loops. 
-->

---
# Turtle Challenges 🐢

---
### Draw A Hexagon 🌈
- Create a list of colors and use them to draw a hexagon with a turtle.

```python
from ipyturtle import Turtle

hex_turtle = Turtle()
colors = ["red", "orange", "yellow", "green", "blue", "purple"]

for color in colors:
    hex_turtle.color(color)
    hex_turtle.forward(100)
    hex_turtle.right(60)
```

<!-- 
- Introduce a practical exercise using turtle graphics to apply list concepts.
- Explain the loop structure to cycle through a list of colors and draw a hexagon. 
-->

---

### Draw A Colorful Flower 🌸

- Loop through colors list, drawing a circle for each petal.

```python
from ipyturtle import Turtle

turtle = Turtle()
rainbow_colors = ["red", "orange", "yellow", "green", "blue", "violet"]

for color in rainbow_colors:
    turtle.color(color)
    turtle.circle(100)
    turtle.left(60)
```

<!-- 
- Encourage creativity in using lists with turtle graphics to draw a colorful flower.
- Highlight the use of loops and the `circle` method for drawing petals of different colors. 
-->