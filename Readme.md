# Welcome to our Intro to Python Course Repository! 🌟

Hello, amazing educators! 👩‍🏫👨‍🏫

We're thrilled to share with you this repository, a treasure trove of resources for teaching Python to 6th through 8th graders. This isn't your typical course content – it's a journey into the exciting world of Python programming, tailored specifically for young, curious minds!

## What's Inside? 📦

This repository holds a collection of slides and interactive Jupyter notebooks. These notebooks are more than just a learning tool; they're a playground for students to engage with and create applications, all while learning Python. And guess what? They get to play with a virtual turtle! 🐢

## Course Structure 🏗️

The course is neatly divided into 7 comprehensive modules. Each module comes with its own interactive notebooks, a set of challenge problems to test understanding, and detailed lesson plans to guide your teaching journey.

### 1. **Variables and Calculations**
   Dive into the world of variables and basic arithmetic operations. Students
   will learn how to store data and perform calculations, a fundamental skill in
   programming.
   
   - **[Google Slides](https://drive.google.com/drive/folders/1Ys-_71AGSn3de3QUNSoiIKBlXTN83G4s?usp=sharing)**
   - **[Marp Slides](./slides/01_variables.md)**
   - **[Notebook](./notebooks/01_variables.ipynb)**

### 2. **Input/Output**
   Discover the magic of interaction! Students learn how to use `input` to
   gather data and `print` to display information, making their code converse
   with users. 

   - **[Google Slides](https://drive.google.com/drive/folders/1Ys-_71AGSn3de3QUNSoiIKBlXTN83G4s?usp=sharing)**
   - **[Marp Slides](./slides/02_input_and_output.md)**
   - **[Notebook](./notebooks/02_input_and_output.ipynb)**

### 3. **Conditional Statements and Logical Expressions**
   Introduce decision-making in code. This module explores how programs can make
   choices using conditional statements and logical operators. 

   - **[Google Slides](https://drive.google.com/drive/folders/1Ys-_71AGSn3de3QUNSoiIKBlXTN83G4s?usp=sharing)**
   - **[Marp Slides 1](./slides/03_01_logical_expressions.md)**
   - **[Notebook 1](./notebooks/03-01_logical_expressions.ipynb)**

### 4. **Loops**
   Unravel the power of repetition in coding with loops. This is where students
   learn to automate tasks efficiently.

### 5. **Lists**
   Jump into managing collections of data. Lists are powerful tools for
   organizing and manipulating multiple pieces of information. 

### 6. **Functions**
   Functions are like mini-programs within your program. This module helps
   students understand how to create and use these handy blocks of code. 

## Getting Started With Grader Than:

Follow these steps to enable your students to have full IDE support for Vex VR.

**Prerequisites:** A [Grader Than Workspace setup](https://docs.graderthan.com/workspace/create/) is required.

1. Create a `Python Course Content` dependency. Refer to these [instructions](https://docs.graderthan.com/workspace/config/#create-a-dependency) for guidance on setting up a dependency.
2. Use the following script as your install guide for the `Python Course Content` dependency you just created:

   <details>
   <summary>Click to show dependency script</summary>

   ```shell
   #!/bin/bash

   crsdir="/home/developer/Documents/course-content"

   # Create the course content directory if it doesn't exist
   mkdir -p "$crsdir"

   git_repo_url=https://github.com/graderthan/6-8-python-quick.git

   repo_name=$(basename -- "${git_repo_url}")
   repo_name="${repo_name%.*}"

   cd $crsdir

   if [ -d "./$repo_name" ]; then
      # The local repo exists.
      cd "./$repo_name"
      # Save student's local changes
      git stash save
      # Get the latest content
      git pull -X ours
      # Overwrite conflicting new changes with the student's save changes 
      git stash pop
      git checkout --theirs .
      git add .
   else
      # The local repo does not exist b/c it's the first time.
      git clone "${git_repo_url}"
   fi

   # Set up the symbolic link
   src_dir="${crsdir}/${repo_name}/notebooks"
   dest_dir="/home/developer/Documents/code/notebooks"

   # Check if the destination directory exists, create it if it doesn't
   mkdir -p "$(dirname "$dest_dir")"

   # Create the symbolic link if it doesn't exist
   if [ ! -L "$dest_dir" ]; then
      ln -s "$src_dir" "$dest_dir"
   fi

   # If anything goes wrong don't prevent the workspace from starting.
   exit 0
   ```

   </details>

3. **🥳 Completion!** Your students and course now have full IDE support for Vex VR.

We believe that learning to code should be fun, interactive, and accessible. With these resources, we hope to ignite a passion for programming in your students and equip them with the skills to explore the vast universe of coding.

Happy teaching! 🍎💻🌈

---

If you have any questions or need further assistance, please don't hesitate to
reach out to us at [support@graderthan.com](support@graderthan.com]). Let's make
coding a favorite adventure for your students! 🌟 