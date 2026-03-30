# DSCI-250, Spring 26 - Course Project

This repository contains instructions for the Course Project assigned in Intermediate Data Science (DSCI-250, Spring 2026) at Lewis & Clark College by Dr. Lawley.

## Deadlines

- [Project Proposal](instructions/00_project-proposal.md): Mon, 04/06/26, 11:59 pm
- Data Source: Mon, 04/13/26, 11:59 pm
- Rough Draft: Mon, 04/20/26, 11:59 pm
- Peer Review Reflection: Wed, 04/22/26, 11:59 pm
- Final Draft: Wed, 04/29/26, 11:59 pm

## Important Dates

- Peer Reviews: Wed, 04/22/26, during class
- Project Presentations, Thu, 05/07, 8:30 am - 11:30 am


## Project Description

Your course project is a data journalism style report. 
You will explore data on a topic of your choice and use the data science skills you've learned in this course to analyze the data.
The specific requirements for each section of your project are detailed below.

## Project Requirements (WIP)

### Data Source

Data used must be obtained via one of the following methods:

- From a Web API using the [httr2](https://httr2.r-lib.org/) package
      - [Open-Meteo](https://open-meteo.com/en/docs#api_documentation)
      - [eBird](https://documenter.getpostman.com/view/664302/S1ENwy59)
      - etc.
- From a Web API using an API-wrapping R package
      - [geonames](https://docs.ropensci.org/geonames/)
      - [rebird](https://docs.ropensci.org/rebird/)
      - etc.
- Scrapped from the web using the [rvest](https://rvest.tidyverse.org/) package
- Other method (by approval only)


The code you write to collect your data will be included in your final submission.
It should be inside of its own R script and *not* inside of your actual report qmd file. 


### Data Analysis

Must contain all of the following items

-  **x1 custom function that performs a data wrangling task**
    -   Takes at least one argument
    -   Includes comment (inside of function body) describing what the function does and what the input arguments should be
    -   Used at least once (but ideally is used more than once)
    -   Includes at least 2 checks: implemented using `stop()`, `warning()`, or `stopifnot()`
    -   Examples: 
        - Function that cleans up a string. Applied to multiple columns using the purrr package
-  **x1 custom function that creates a plot based on user inputs**
    -   Takes at least 2 arguments (e.g., data frame value to filter some column by)
    -   Includes comment (inside of function body) describing what the function does and what the input arguments should be
    -   Used at least once (but ideally is used more than once)
    -   Includes at least 2 checks: implemented using `stop()`, `warning()`, or `stopifnot()`
    -   Examples: 
        - Function that filters a data frame so it only contains rows where column matches value provided and creates a customized plot. Used to create multiple variations of the same plot.

...




