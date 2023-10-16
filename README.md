
<!-- README.md is generated from README.Rmd. Please edit that file -->

# rtutorials

<!-- badges: start -->
<!-- badges: end -->

*This R package is currently under active development.*

Acquire basic statistics and R knowledge (somewhat) interactively and
self paced.

- **Language**: German

- **Audience**: Written for statistic newbies, in our case 3rd semester
  bachelor students of environmental and civil engineering

### Quick Start

By installing this package, you add handcrafted lessons to your RStudio
Tutorials Pane.

**Prerequisites**: R + RStudio installed

Copy the following code into your RStudio [console
pane](https://cengel.github.io/R-intro/backgroud.html#rstudio-console-and-command-prompt)
and hit Enter.

``` r
install.packages(c("devtools", "learnr"))
devtools::install_github("statistik-lehre/rtutorials")
```

## Contents

Each tutorial is associated with one of eleven lectures. Lecture
material is not included. Tutorials could be useful in a standalone
fashion anyways.

All tutorials are in German. Here are the titles translated to English
for the convenience of the English readers. A German detailed overview
can be found at the end.

Tutorials with substantial content ( \> 50% completion status) are
highlighted.

| Lecture | Tutorial Subject                      | Status |
|---------|---------------------------------------|--------|
| 1       | **Introduction**                      | 80%    |
| 1       | **Exploring Functions and Arguments** | 95%    |
| 1       | **Scientific Process**                | ~70%   |
| 2       | **Vectors**                           | 90%    |
| 2       | **Indexing**                          | 65%    |
| 2       | Data Frames                           | 30%    |
| 3       | Data Import                           | 0%     |
| 3       | Scales                                | 40%    |
| 3       | Measures of Central Tendency          | 10%    |
| 3       | Missing Values                        | 0%     |
| 4       | **Measures of Spread**                | 90%    |
| 4       | z-Standardization                     | 0%     |
| 5       | Visualization                         | 0%     |
| 6       | **Sampling**                          | 40%    |
| 6       | t-Tests                               | 0%     |
| 7       | Levene-Test                           | 0%     |
| 8       | Chi Squared                           | 0%     |
| 8       | Power Analysis                        | 0%     |
| 8       | Correlations                          | 0%     |
| 9       | **Simple Linear Regression**          | 85%    |
| 10      | **Scientific Process**                | ~70%   |
| 11      | **Programming Basics**                | ~70%   |

## Accessing the tutorials

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

And to run the individual tutorials, run:

    learnr::run_tutorial("name", package = "rtutorials")

## Contributing

Feedback and contributions are welcome!

If you spot a typo, some incorrect content or see just a better way to
do it, you are welcome to collaborate. Either report it as an issue or
even better, fix it yourself!

Fork the repo, contribute and please submit your changes with a pull
request.

The tutorial source code is found at `inst/tutorials/…/….Rmd`.

A template tutorial for the stylings we use is found at
`inst/tutorials/template`, but not included in the built package.

For more in depth guidelines on `learnr` tutorials, check out the
[`learnr`](https://rstudio.github.io/learnr/) documentation.

## Licensing

We would be happy to hear from you if you want to modify or redistribute
the contents of this course.

This software comes to you with an OpenSource license, because we are
fond believers in the strength of commons.

However, the use is restricted to noncommercial purposes and only
applies to the contents of this repository. Other course materials that
you may get as one of our students are subject to copyright.

## Explanation of Quick Start commands

*for those who want to understand the installation code, skip if you
already know*

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

## Funding

Kassel University, HessenHub, 2022 - 2023

## German

Detaillierte Übersicht über den Inhalt + Codes zum Starten der einzelnen
Tutorials:

    Available tutorials:
    * rtutorials
      - 01a_intro           : "Einführung Idee"
      - 01a_intro_alt       : "Einleitung"
      - 01b_funktionen      : "Funktionen erkunden"
      - 01c_prozess         : "Wissenschaftlicher Prozess"
      - 02a_vektoren        : "Vektoren"
      - 02b_index           : "Indizierung bei Vektoren"
      - 02c_dataframes      : "Arbeit mit Tabellen"
      - 03a_import          : "Datenimport"
      - 03b_skalen          : "Skalenniveaus"
      - 03c_zentraletendenz : "Maße der zentralen Tendenz"
      - 03d_tidydata        : "Lang und Breit"
      - 03e_na              : "Fehlende Werte"
      - 04a_dispersion      : "Dispersionsmaße"
      - 04b_zstandard       : "z-Standardisierung"
      - 05a_vis             : "Visualisierung"
      - 06a_sampling        : "Inferenzstatistik"
      - 06b_ttest           : "Teststärke"
      - 07a_levene          : "Levene-Test"
      - 08a_chi             : "Chi-Quadrat-Test"
      - 08b_korrelationen   : "Korrelationen"
      - 09a_regression      : "Regression"
      - 10a_prozess_lang    : "Wissenschaftlicher Prozess"
      - 11a_programmieren   : "Programmieren Basics"

#### Einleitung

``` r
learnr::run_tutorial("01a_intro", package = "rtutorials")
```

- R als Taschenrechner

#### Funktionen erkunden

``` r
learnr::run_tutorial("01b_funktionen", package = "rtutorials")
```

- Funktionsaufruf am Beispiel von `cowsay`

- Argumente spezifizieren

- Skripte erstellen

#### Wissenschaftlicher Prozess (kurz)

``` r
learnr::run_tutorial("01c_prozess", package = "rtutorials")
```

#### Vektoren

``` r
learnr::run_tutorial("02a_vektoren", package = "rtutorials")
```

- Variablen erstellen, Assignment

- Gute Namen

- Was ist das Environment

- Recycling beim Rechnen mit Vektoren

- Vektorisierung

#### Indizierung bei Vektoren

``` r
learnr::run_tutorial("02b_index", package = "rtutorials")
```

- Auf spezifische Elemente eines Vektors zugreifen mittels `[]`…

- Über die Position

- Über eine logische Bedingungsprüfung

- Über Namen (Attribute)

#### Data Frames

``` r
learnr::run_tutorial("02c_dataframes", package = "rtutorials")
```

- Wie werden Tabellen in R repräsentiert?

- Indizierung bei Data Frames mit `$`

#### Maße der Streuung

``` r
learnr::run_tutorial("04a_dispersion", package = "rtutorials")
```

- Was ist Varianz

- Spannweite

- Quartile und Interquartilsabstand

#### Sampling

``` r
learnr::run_tutorial("06a_sampling", package = "rtutorials")
```

- “Stichprobenkennwerteverteilung” verstehen

- das Konzept “Stichprobenvariation” verstehen

- simulierte Stichprobenziehung mit `moderndive::rep_sample_n()`

#### t-Test

``` r
learnr::run_tutorial("06b_ttest", package = "rtutorials")
```

- einen t-Test in R ausführen und Output interpretieren

#### Einfache lineare Regression

``` r
learnr::run_tutorial("09a_regression", package = "rtutorials")
```

- Interpretation der Koeffizienten

- Erstellen eines `lm()` (linear model)

- Output lesen lernen

- Voraussetzungen der Regression prüfen

#### Wissenschaftlicher Prozess (lang)

``` r
learnr::run_tutorial("10a_prozess_lang", package = "rtutorials")
```

- Nachschlagewerk für den detaillierten Ablauf des typischen
  Forschungsprozesses auf einer Roadmap

#### Programmieren Basics

``` r
learnr::run_tutorial("11a_programmieren", package = "rtutorials")
```

- Schleifen und Bedingungen

- `for`, `while`, `if`, `else`, …
