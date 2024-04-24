---
title: 'Group Project Details'
teaching: 10
exercises: 2
---

::: questions
-   What will we be working towards over the next two weeks?
:::

::: objectives
-   Have all the necessary software downloaded to run both R and Python from RStudio
-   Understand the expectations for the end-of-workshop live coding sessions.
:::

## Group Work Details

This workshop will teach you how to design and execute on a curriculum from start to finish. Over the course of the coming week, you will learn how to identify your target audience, determine what content to teach, and create an assessment-based curriculum for that content. Because much of our work involves programming, you will also learn how to effectively teach using the live coding method. 
You should have formed yourselves into groups of three-- is anyone not part of a group yet? 

Over the course of the workshop, when you see a section labeled **Group Work**, it's a sign for you to assemble with your group members to develop a new part of your curriculum. 

On Thursday and Friday of next week, each group will take us through their lesson. You will have **30 minutes total** to introduce your topic, teach it with live coding, and deliver a brief assessment. Afterwards we will have 10 minutes of feedback before moving on to the next group. This is a short amount of time, so the topic of your curriculum must be very concise. We will work together to pick an appropriate topic for each group. 

## Running Python from RStudio

This is a mixed course, with participants who are most comfortable in either Python or R. In order to run R scripts, everyone should have downloaded and installed R and RStudio yesterday. And luckily, RStudio can also function as a development environment for Python, so we shouldn't need to download Python separately. What we will need to do is install the R package that will help us run Python, as well as a few Python packages.

### `reticulate`
You can run Python code from an R session using an R package called `reticulate`. Make sure you have `reticulate` installed, either using the GUI or by running `install.packages("reticulate")` from the RStudio console. 

Now, open a new R script and name it "install_python_packages.R". On the first line, type `library(reticulate)`.

### Python packages
Like R, Python has a robust system of libraries that need to be installed and loaded before they can be used. We can use our R script to install these packages using the `reticulate` function `py_install()`.

On a lower line of your R script, type:

```
py_install(c("pandas", "seaborn", "matplotlib"))
```

This should install the most commonly used data science and plotting packages used in Python. If you ever have trouble with a package loading, or you need to install a new package, we can come back and rerun or modify this script. 

::::: callout

## Note for Python Users

Even if you are a Python user who already has these packages installed, you will need to install them again using py_install. This is because `reticulate` creates a virtual environment to run Python from R, so it doesn't interfere with the instance of Python running on your main machine.
:::::


### Testing Your Installation

Now, open a new file, but instead of opening an R script, scroll down and create a Python script. Name it "test_install.py". In the file, type the following code:

```
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

print("Hello world")
```

Raise your hand if you run into any errors and we will work through them with you.


::: keypoints
-   You will work in small groups over the course of this workshop, leading up to a final live teaching session
-   We can run both Python and R from RStudio, but need to install and set up the correct packages in both languages.
:::
