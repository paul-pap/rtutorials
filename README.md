
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rtutorials: learn basic statistics and R interactively

<!-- badges: start -->
<!-- badges: end -->

*This R package is currently under active development.*

teaching statistics along with the basics of the R programming language.

Language: German

Audience: Written for statistic newbies, in our case 3rd semester
bachelor students of environmental and civil engineering

## Installation

### Quick Start

Prerequisites: R + RStudio installed

Copy the following code into your RStudio [console
pane](https://cengel.github.io/R-intro/backgroud.html#rstudio-console-and-command-prompt)
and hit Enter.

``` r
install.packages(c("devtools", "learnr"))
devtools::install_github("statistik-lehre/rtutorials")
```

**Explanation for those who want to understand these two lines, skip if
you already know**

`install.packages()` is a function that installs R packages.

`c()` is combining stuff, in our case the two package names.

The packages we are installing are called `devtools` and `learnr`.

- `learnr` is necessary because it supplies the interactive tutorials
  functionality

- `devtools` is necessary to install packages from GitHub.

`install_github()` is self explanatory - it installs a package from a
GitHub repo. The double colons `::` show that the function lives inside
the `devtools` package.

Inside the parentheses, we supply the name of this GitHub repo, which
contains the tutorials you will learn in this semester:
`"statistik-lehre/rtutorials"`.

### Accessing the tutorials in RStudio

**The graphical way**

In RStudio, you will see a tutorials tab in the top right. Click it to
select from different tutorials and start them. You will see all
tutorials of all different packages, including example tutorials from
the `learnr` package.

It might require an RStudio restart until the tutorials of the
`rtutorials` package appear.

Click “Start Tutorial” to learn interactively. That’s it!

Below is some code which achieves the same thing without a navigating a
click- and scrollable menu surface.

**The command way**

To list all available tutorials from `rtutorials`, copy paste following
code to the console:

``` r
learnr::available_tutorials(package = "rtutorials")
```

And to run the individual tutorials:

### Einleitung

``` r
learnr::run_tutorial("Einleitung", package = "rtutorials")
```

- why do we need statistics, why programming languages
- fist examples of R as a calculator

### Funktionen erkunden

``` r
learnr::run_tutorial("Funktionen_erkunden", package = "rtutorials")
```

- installing and loading packages
- what is a script? what is a R notebook?
- playfully learn the structure of function calls with `cowsay::say()`

### Vektoren

``` r
learnr::run_tutorial("Vektoren", package = "rtutorials")
```

- Learn how to assign content to a variable
- how to find your variable in the environment
- what is a vector?
- combining vectors with `c()`
- vector based calculations
- vectorised nature of R
- Using the colon operator `:`

### Indizierung

``` r
learnr::run_tutorial("Indizierung", package = "rtutorials")
```

- What is indexing (subsetting)?
- Subsetting with integer vectors
- … with logical vectors
- … with character vectors
- Using your first conditional statements

#### tutorials to come:

- writing your own functions
- Datenimport
- Objekte in R verstehen
- Data Wrangling
- Visualisierung
- t-Tests
- Warum Effektstärke wichtig ist
- Power berechnen
- Ab wann sind Daten normalverteilt
- Chi-Square-Test
- Korrelation
- einfache lineare Regression

## Contributing

Feedback and contributions are welcome!

If you spot a typo, some incorrect content or see just a better way to
do it, you are welcome to collaborate. Either report it as an issue or
even better, fix it yourself!

Fork the repo, contribute and please submit your changes with a pull
request.

The tutorial source code is found at `inst/tutorials/…/….Rmd`.

For more in depth guidelines on `learnr` tutorials, check out the
[`learnr`](https://rstudio.github.io/learnr/) documentation.

## Licensing

We would be happy to hear from you if you want to modify or redistribute
the contents of this course.

This software comes to you with an OpenSource license, because we are
fond believers in the strength of commons.

However, this only applies to the contents of this repository. Other
course materials that you may get as a student can and probably will be
subjected to copyright.

## Funding

Kassel University, HessenHub, 2022 - 2023
