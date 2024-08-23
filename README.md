# Project for the Survival Analysis Course 

## Description

For this analysis we wanted to work with a dataset different from health issues. In this case we took data related to animals in a shelter
and their adoption. It should be mentioned that the data frame does not contain the date of entry of the animals to the shelter, but the date of birth, so we had to adapt to the available data, since we really wanted to apply the analysis in another area, and therefore the results
will be more a function of the age that an animal has before it is adopted, given that it is in the shelter.

In terms of survival analysis, the objective of this project is to determine the “risk” that pets in an animal shelter have of being adopted , based on different characteristics that are available in the chosen data set. It is worth mentioning that the data contains different outcomes for the animals: adoption, transfer, or no outcome. However, in our case we will only use a dichotomous output indicating whether it was adopted or not. The data ends on February 1st, 2018, after which date it is not known what happens to the animals.

We will also analyze how the following variables, when possible to include them, may influence the adoption or non-adoption of the animals.

Data dictionary :

• id: unique id for each animal

• age_upon_outcome: age of the animal when the outcome was determined

• animal_type: cat, dog, or … something else

• breed: breed of the animal

• color: color of the animal

• date_of_birth: date of birth of the animal

• datetime: date and time when the outcome was determined

• name: name of the animal

• outcome_type: there are three possible outcomes: adoption, transfer, no outcome (euthanized, died)

• sex: sex of the animal

• spay_neuter: whether the animal was spayed or neutered: intact or fixed.

## Main files
survival_project.qmd : Full script.

survival_project.pdf : Report.

survival_project_appendix.pdf : Appendix.

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

To render a pdf you might night to run `quarto install tinytex` in the terminal

## Data used

Data taken from [Kaggle](https://www.kaggle.com/competitions/sliced-s01e10-playoffs-2/data?select=train.csv).

We only use the `train.csv` data, because we have no `outcome_type` information
in the `test.csv` file.