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

# Logic (Yes | No)

---

## Boolean values

| Value  | Code   |
|--------|--------|
| ✅ yes | `True` |
| ❌ No  | `False` |

<!--
- Boolean Data Type: Booleans are simple true or false values.
  - Represent basic yes/no or true/false choices.
  - `True` stands for a positive or affirmative answer (✅ yes).
  - `False` signifies a negative or opposite response (❌ no).
  - Essential in decision-making in code, like toggling settings or checking conditions.
-->

---

## Comparison operators

<style>
html,body        {height: 100%;}
.wrapper         {width: 70%; max-width: 1280px; height: 100%; margin: 0 auto; background: rgba(255, 255, 255, .0); padding-bottom: 50px}
.h_iframe        {position: relative; padding-top: 56%;}
.h_iframe iframe {position: absolute; top: 0; left: 0; width: 100%; height: 100%;}
</style>

<div class="wrapper">
    <div class="h_iframe">
        <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/wivz8ytlHBs?si=yQm1SGVp-qLVb06X" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
</div>

---

<!-- _footer: "" -->

## Comparison operators

| Operator  |  Description        |
|-----------|---------------------|
| `==`       | Equal to           |
| `!=`       | Not equal to       |
| `>`        | Greater than       |
| `<`        | Less than          |
| `>=`       | Greater than or equal to |
| `<=`       | Less than or equal to    |

<!--

- Comparison Operators Overview: 
  - Used to compare values in Python. They create true or false values.
  - `==`: Checks if two values are equal.
  - `!=`: Determines if two values are not the same.
  - `>`: Tests if a value is greater than another.
  - `<`: Compares if a value is less than another.
  - `>=`: Checks if a value is greater than or equal to another.
  - `<=`: Tests if a value is less than or equal to another.
  - Crucial for making decisions in code, like in if-else statements.
-->

---

### Greater Than `>` Example

```py
num1 = int(input("Type a number:"))
num2 = int(input("Type another number:"))

print("Is the first number greater than the second number?", num1 > num2)
```

<!--
- Greater Than `>` Example: Demonstrates the use of the `>` operator.
  - `num1` and `num2` are variables storing user inputted numbers.
  - `int(input())` converts the user's text input into numbers.
  - The `print()` function shows if `num1` is greater than `num2`.
  - Helps students understand how to compare two numbers using `>`.
-->

---

### Equals `==` Example

```py
user_input_1 = input("Type a number:")
user_input_2 = input("Type another number:")

print("Are the inputs the same?", user_input_1 == user_input_2)
```

<!--
- Equal To `==` Example: Illustrates using the `==` operator for comparison.
  - `user_input_1` and `user_input_2` capture two separate user inputs.
  - The inputs are kept as strings (text) without converting to numbers.
  - The `print()` function checks and shows if the two inputs are identical.
  - Demonstrates how to compare two inputs for exact equality.

The students will be asked to do the following:

  1) Type "apple" and "apple" and check the output.
  2) Type "APPLE" and "apple" and check the output.
  3) Type "Apple" and "apple" and check the output.

The goal is to see how string casing matters.
-->

---

## Logical Operators 

| Operator | Description                              |
|----------|------------------------------------------|
| `and`    | True if both conditions are true         |
| `or`     | True if at least one condition is true   |
| `not`    | Inverts the truth value of a condition   |

---

### `and` operator

<style>
html,body        {height: 100%;}
.wrapper         {width: 70%; max-width: 1280px; height: 100%; margin: 0 auto; background: rgba(255, 255, 255, .0); padding-bottom: 50px}
.h_iframe        {position: relative; padding-top: 56%;}
.h_iframe iframe {position: absolute; top: 0; left: 0; width: 100%; height: 100%;}
</style>

<div class="wrapper">
    <div class="h_iframe">
        <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/riHazq0H4-o?si=pi5kOOKqFSVHzTW-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
</div>

--- 

### `and` operator

**Code:**

```py
print(True and True)
print(True and False)
```

**Output:**

```
True
False
```

<!--
- Understanding the `and` Operator: 
  - The `and` operator checks if both conditions on either side of it are true.
  - `print(True and True)` outputs `True` because both conditions are true.
  - `print(True and False)` results in `False` since one of the conditions is false.
  - Demonstrates how `and` only returns `True` when all combined conditions are true.
-->

---

### Code Challenge

Change the code so `result` is `True` if `user_input` is between 1 and 10.

```py
min_value = 1
max_value = 10
user_input = int(input("Please enter a number: "))

result = False  ← Update this line

print(f"Is your number between {min_value} and {max_value}? {result}")
```

<!--
- Code Challenge Explanation:
  - Task: Update `result` to check if `user_input` is within the specified range.
  - Current setup takes a number input and sets `result` to `False`.
  
- Answer: `result = min_value < user_input <= max_value`.
  - This modification uses a logical expression to verify if `user_input` is more than 1 (`min_value`) and up to 10 (`max_value`).
-->

---

### `or` operator

<style>
html,body        {height: 100%;}
.wrapper         {width: 70%; max-width: 1280px; height: 100%; margin: 0 auto; background: rgba(255, 255, 255, .0); padding-bottom: 50px}
.h_iframe        {position: relative; padding-top: 56%;}
.h_iframe iframe {position: absolute; top: 0; left: 0; width: 100%; height: 100%;}
</style>

<div class="wrapper">
    <div class="h_iframe">
        <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/FgzKLWxxS1Q?si=-BuwbGmwFIeV8Mwh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
</div>

---

### `or` operator

**Code:**

```py
print(True or False)
print(False or False)
```

**Output:**

```
True
False
```

<!--
- The `or` operator evaluates if at least one of the conditions is true.
- `print(True or False)` outputs `True` because at least one condition (the first one) is true.
- `print(False or False)` results in `False` since both conditions are false.
- Demonstrates how `or` returns `True` when any one of the combined conditions is true.
-->

---

### `not` Operator

**Code:**

```py
print(not True)
print(not False)
```

**Output:**

```
False
True
```

<!--
- The `not` operator inverts the truth value of the condition it precedes.
- `print(not True)` outputs `False` because `not` inverts the truth of `True`.
- `print(not False)` results in `True` as `not` changes `False` to `True`.
- Demonstrates how `not` is used to flip the boolean value of a given condition.
-->

--- 

# Code Challenge

*Do I need a jacket? 🧥*

```py
is_raining = input("Is it raining? (yes/no/soon): ")
temperature = input("What temperature is it outside?: ")

result = False ← Change this line
```

<!-- 

- Program Objective: To advise on wearing a jacket based on weather conditions.
  - The application asks if it's currently raining (`yes`) or expected to rain soon (`soon`).
  - It also requests the user to input the current temperature.
  - The program suggests wearing a jacket if:
    - It's raining or expected to rain soon, and the temperature is below 100 degrees.
    - It's not raining and the temperature is below 50 degrees.
  - **User Input Handling**: 
    - Users respond with `yes` or `no` to indicate if it's raining.
    - The program checks `is_raining` for a `yes` value to assess rain conditions.

Solution: `result = ((is_raining == "yes" or is_raining == "soon") and temperature < 100) or temperature < 50`
-->