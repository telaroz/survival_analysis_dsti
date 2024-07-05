# Project for the Survival Analysis Course 

## Using R Projects

For reproducibilty propuses it is highly advised to use R Projects for work that
is done in R. 
The only needed thing is to have an `.Rproj` file inside the project directory.
Also, the place where this file is located will be the base or working directory
(can be checked with `getwd()` command).

[Rstudio Projects](https://support.posit.co/hc/en-us/articles/200526207-Using-RStudio-Projects)

## Using quarto

Quarto is an open-source scientific and technical publishing system that allows 
you to weave together narrative text and code to produce high-quality outputs 
including reports, presentations, websites, and more.

One of the main features of Quarto is that it isn’t just built for R. It’s 
language-agnostic. It can render documents that contain code written in R, 
Python, Julia, or Observable.

[About quarto](https://www.jumpingrivers.com/blog/quarto-rmarkdown-comparison/)

quarto files work like `.Rmd` files, but is optimized, works more smoothly and
has more options overall. 
Also works without issue in multiple programming languages, so you can combine
for example R and Python code in the same document.

## Data used

Data taken from [Kaggle](https://www.kaggle.com/competitions/sliced-s01e10-playoffs-2/data?select=train.csv).

We only use the `train.csv` data, because we have no `outcome_type` information
in the `test.csv` file.