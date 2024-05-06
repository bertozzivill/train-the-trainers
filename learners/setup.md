---
title: Setup
---

## Logistics

We will meet every day from April 29th to May 10th, excluding the
holiday on May 1st. Class will run from 9am to 1pm every day. We will
meet at dLab Kilimanjaro Room, block D.

Participants not in Dar should also be able to join remotely via this
[zoom
link](https://zoom.us/j/98559482416?pwd=UzA3ZVFJNS9ZRnFYamhhUW1RVG5QUT09){target="_blank"}.
The meeting ID is 985 5948 2416, and the password is 213509. Sessions
will be recorded if you are unable to join in-person or online.

### Pre-Course Survey

Before we begin, please take a moment to fill out the [pre-course
survey](https://forms.gle/1eyZ96SjfWD9SLvc9){target="_blank"}.

### Schedule (Subject to Change)

+-----------------+-----------------------+----------------------+
| Day             | Subjects              | Amelia Afternoon     |
|                 |                       | Location             |
+=================+=======================+======================+
| Monday April 29 | Welcome and           | dLab                 |
|                 | Introduction          |                      |
|                 |                       |                      |
|                 | What Makes a Good     |                      |
|                 | Teacher?              |                      |
|                 |                       |                      |
|                 | Intro to Growth       |                      |
|                 | Mindsets              |                      |
+-----------------+-----------------------+----------------------+
| Tuesday April   | Skill Levels, Mental  | Out for conference   |
| 30              | Models, and           |                      |
|                 | Misconceptions        |                      |
|                 |                       |                      |
|                 | Lesson Design         |                      |
+-----------------+-----------------------+----------------------+
| Wednesday May 1 | Holiday               |                      |
+-----------------+-----------------------+----------------------+
| Thursday May 2  | Finding your Target   | dLab                 |
|                 | Audience              |                      |
|                 |                       |                      |
|                 | Creating Objectives   |                      |
+-----------------+-----------------------+----------------------+
| Friday May 3    | Discussion: Dealing   | dLab                 |
|                 | with the Unexpected   |                      |
|                 |                       |                      |
|                 | Designing Assessments |                      |
+-----------------+-----------------------+----------------------+
|                 |                       |                      |
+-----------------+-----------------------+----------------------+
| Monday May 6    | Week 1 Recap          | dLab                 |
|                 |                       |                      |
|                 | Lesson Plans &        |                      |
|                 | Crafting Content      |                      |
|                 |                       |                      |
|                 | Equity, Inclusion, &  |                      |
|                 | Accessibility         |                      |
+-----------------+-----------------------+----------------------+
| Tuesday May 7   | How to Code Live      | dLab                 |
+-----------------+-----------------------+----------------------+
| Wednesday May 8 | The Physical Act of   | dLab                 |
|                 | Teaching              |                      |
|                 |                       |                      |
|                 | Lesson Prep Free Time |                      |
+-----------------+-----------------------+----------------------+
| Thursday May 9  | Live Coding Sessions  | dLab                 |
+-----------------+-----------------------+----------------------+
| Friday May 10   | Live Coding           | dLab                 |
|                 | Reflections           |                      |
|                 |                       |                      |
|                 | Conclusion            |                      |
+-----------------+-----------------------+----------------------+

### Group Work for Live Coding

Over the course of this workshop, you will collaborate with your peers
in small groups to develop a short lesson from start to finish. This
includes how to identify your target audience, determine what content to
teach, and create an assessment-based curriculum for that content.
Because much of our work involves programming, you will also learn how
to effectively teach using the live coding method. Over the last two
days of the session, groups will lead the class through their short
lesson and receive feedback. This session will have a mix of R and
Python coders, so you will actually be teaching people something new!

Take some time today or tomorrow to create a group of three people. Make
sure all of your are familiar with the same programming language (R or
Python). Begin to think about something you really enjoy about your
programming language that you might like to share with others. Whatever
it is, it must be *small*! Examples include:

-   how to make a specific type of plot (line, scatter, bar, etc)
-   how to customize the color scheme of a plot
-   how to convert from one date-time type to another
-   how a single function can help solve a common data cleaning problem

In the coming days, you and your group will decide on a specific thing
you'd like to teach and begin building your curriculum from there.

Over the course of the workshop, when you see a section labeled **Group
Work**, it's a sign for you to assemble with your group members to
develop a new part of your curriculum.

On Thursday and Friday of next week, each group will take us through
their lesson. You will have **30 minutes total** to introduce your
topic, teach it with live coding, and deliver a brief assessment.
Afterwards we will have 10 minutes of feedback before moving on to the
next group. This is a short amount of time, so the topic of your
curriculum must be very concise. We will work together to pick an
appropriate topic for each group.

### Code of Conduct

To make clear what is expected, everyone participating in The
Carpentries activities is required to abide by our [Code of
Conduct][coc]. Any form of behaviour to exclude, intimidate, or cause
discomfort is a violation of the Code of Conduct. In order to foster a
positive and professional learning environment we encourage you to:

-   Use welcoming and inclusive language
-   Be respectful of different viewpoints and experiences
-   Gracefully accept constructive criticism
-   Focus on what is best for the community
-   Show courtesy and respect towards other community members

If you believe someone is violating the Code of Conduct, we ask that you
report it to The Carpentries Code of Conduct Committee by completing
[this form](https://goo.gl/forms/KoUfO53Za3apOuOK2).

## Learning Objectives

After attending this training, participants will be able to:

-   teach with a growth mindset, and encourage a growth mindset in
    students;
-   comfortably lead live coding sessions;
-   design lessons and assessments using the principles of backward
    design.

## Prerequisites

Before joining this training, participants should:

-   have the latest versions of [R and
    RStudio](https://bertozzivill.github.io/r-install-instructions)
    installed (see below).
-   have some familiarity with programming in Python or R, especially
    making plots in either language.

## Software Setup

Please make sure you have a stable internet connection, then follow these steps:

### R and RStudio

If you have not already done so, please follow the [R setup
instructions](https://bertozzivill.github.io/r-install-instructions) to
download or update your R and RStudio.

This is a mixed course, with participants who are most comfortable in either Python or R. In order to run R scripts, everyone should have downloaded and installed R and RStudio yesterday. And luckily, RStudio can also function as a development environment for Python, so we shouldn't need to download Python separately. What we will need to do is install the R package that will help us run Python, as well as a few Python packages.

### R Packages Needed
Please make sure you have installed the `tidyverse` package in R by running the the `install.packages("tidyverse")` in the console. 


### `reticulate`
You can run Python code from an R session using an R package called `reticulate`. Make sure you have `reticulate` installed, either using the GUI or by running `install.packages("reticulate")` from the RStudio console. 

Now, open a new R script and name it "install_python_packages.R". On the first line, type `library(reticulate)`.

### Python packages
Like R, Python has a robust system of libraries that need to be installed and loaded before they can be used. We can use our R script to install these packages using the `reticulate` function `py_install()`.

On a lower line of your R script, type:

```
py_install(c("pandas", "streamlit", "matplotlib"))
```

This should install the packages you will need to use in Python for this session. If you ever have trouble with a package loading, or you need to install a new package, we can come back and rerun or modify this script. 


### Test your installation

From the top menu bar, select, "Session/New Session". A new R session will open. Check the label in the top right of the session:

![](fig/rstudio_project.png)


If it does not say "Project: (None)", you need to close the project you're in. Click on the label and select "Close Project". It should now say "Project: (None)" in the corner.

Open a new **Python script** by going to File/New File/Python Script in the menu bar. Name it "test_python.py". Write the following: 

```
import pandas as pd
import matplotlib.pyplot as plt
import streamlit as st

d = {'col1': [1, 2], 'col2': [3, 4]}
df = pd.DataFrame(data=d)
```

Try running this code and see if it throws any errors. If it does, email Amelia at amelia.bertozzi-villa@gatesfoundation.org.


::::: callout

## Note for Python Users

Even if you are a Python user who already has these packages installed, you will need to install them again using py_install. This is because `reticulate` creates a virtual environment to run Python from R, so it doesn't interfere with the instance of Python running on your main machine.
:::::




## Acknowledgment

This lesson was built using [The Carpentries
Workbench][carpentries-workbench] by Amelia Bertozzi-Villa and Punam
Amratia. Much material was adapted from the Carpentries courses
[Collaborative Lesson Development Training][lesson-dev] and [Instructor
Training][instructor-training], while other material is original.
