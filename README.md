
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rtutorials: interactive statistics tutorials

<!-- badges: start -->
<!-- badges: end -->

This R package is currently under active development. It provides
interactive `learnr` statistics tutorials, aiming to teach statistics
along with the basics of the R programming language.  
It is in German language and directed at bachelor students of
environmental and civil engineering, accompanying their first statistics
lecture.

## Installation

### Quick Start

Copy the following code into your RStudio [console
pane](https://cengel.github.io/R-intro/backgroud.html#rstudio-console-and-command-prompt)
and hit Enter.

``` r
install.packages(c("devtools", "learnr"))
devtools::install_github("statistik-lehre/rtutorials")
```

**Explanation**

`install.packages()` is a function that installs R packages. `devtools`
and `learnr`.

`learnr` is the framework we used to write the tutorials and required to
run them.

`devtools` is a package that adds functionality to build R packages from
source code. The source code for the tutorial package we want to build
into a functional package that you can use is available in this repo.

In the second line, we use the `install_github()` function and specify
that it can be found within the `devtools` package with double colons
`::`. Inside the brackets, we specify the last part of this GitHub
Repository URL containing the source code.

### Accessing the tutorials in RStudio

In RStudio, you will see the tutorials pane on the top right. Click
there to select from different tutorials and start them. It might
require a R restart until the tutorials appear.

Alternatively, to list all available tutorials, run

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

Either fork the repo or create a new branch. After your contribution,
please submit it with a pull request. The content of the tutorials is
found at `inst/tutorials/…/….Rmd`. For more in depth guidelines, check
out the [`learnr`](https://rstudio.github.io/learnr/) documentation.

## Licensing

All rights are currently reserved to Kassel University, because they are
our employers. However, we are striving to license this project with an
open source license in the near future.

## Funding

Kassel University, HessenHub
