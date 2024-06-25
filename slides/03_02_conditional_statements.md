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
# Understanding If/Else Statements 🚦

- If/else statements: Road signs in coding
- Direct your program based on conditions

<!-- 
- This slide introduces if/else statements as fundamental decision-making tools in programming.
- Explain that these statements guide the flow of the program, much like road signs guide traffic.
-->

---

# Basic Syntax of If Statement

```python
if condition:
    # code to execute if condition is true
```

- **If statement**: Executes a block of code if the condition is True.

<!-- 
Speaker notes: Discuss the syntax of an if statement. Highlight the importance of the condition being True for the code block to execute. This is the starting point for understanding conditional logic in programming.
-->

---

# Basic Syntax of If/Else Statement

```python
if condition:
    # code if condition is true
else:
    # code if condition is false
```

- Executes different blocks based on the condition's truth value.

<!-- 
Speaker notes: Explain the addition of the else statement for handling cases where the condition is False. This expands on the decision-making capabilities of programs, allowing for two possible paths of execution.
-->

---

# Try It Out! 🌟
```python
temperature = 80 # Change this to see different outputs
if temperature > 70:
    print("It's a warm day!")
else:
    print("It's a bit chilly today!")
```

- Experiment by changing the `temperature` value.
- Observe how the program's response changes.

<!-- 
Speaker notes: Encourage students to actively modify the temperature variable to see how the conditional logic in the program responds. This hands-on activity helps solidify their understanding of if/else statements through direct experimentation.
-->

---

# Introducing Elif Statements

- `elif` allows checking multiple conditions in sequence.
- It's used between `if` and `else` for more complex decisions.

<!-- 
Speaker notes: Introduce `elif` as a way to extend the basic if/else logic to handle multiple conditions. Explain that `elif` stands for "else if," providing a means to check several "if" conditions in one coherent structure.
-->

---

# Syntax for If/Elif/Else

```python
if condition:
    # code if condition is true
elif another_condition:
    # code if the second condition is true
else:
    # code if none of the conditions are true
```

- Facilitates checking multiple conditions one by one.

<!-- 
Speaker notes: Dive deeper into the syntax of using if/elif/else statements together. Highlight how this structure allows programmers to construct more nuanced decision-making paths in their code.
-->
---
# Conditional Logic with Turtle 🐢
---

# Problem 1: Color Change Based on Position 🎨

- Change turtle's color with position.
- Use `if` to turn the turtle blue if x > 50, else red.

<!-- 
This problem introduces a practical application of if/else statements, using the turtle's position to determine its color. It's a visually engaging way to understand conditional logic.
-->

---

# Problem 2: Temperature Indicator 🌡️

- Simulate a temperature indicator with turtle movement.
- Change the turtle's direction or action based on temperature.

<!-- 
The temperature indicator problem uses conditional logic to visually represent data (temperature) through turtle movement, showcasing a creative application of if/elif/else statements in programming.
-->