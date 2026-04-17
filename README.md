# DSCI-250, Spring 26 - Course Project

This repository contains instructions for the Course Project assigned in Intermediate Data Science (DSCI-250, Spring 2026) at Lewis & Clark College by Dr. Lawley.

## Deadlines

-   [Project Proposal](instructions/00_project-proposal.md): Mon, 04/06/26, 11:59 pm
-   [Data Source](instructions/01_data-source.md): Wed, 04/15/26, 11:59 pm
-   [Rough Draft](instructions/02_rough-draft.md): Wed, 04/22/26, 9:00 am
-   Peer Review Reflection: Wed, 04/22/26, 11:59 pm
-   [Final Draft](instructions/03_final-draft.md): Wed, 4/29/26, 11:59 pm

## Important Dates

-   Peer Reviews: Wed, 04/22/26, during class
-   Project Presentations, Thu, 05/07, 8:30 am - 11:30 am

## Project Description

Your course project is a data journalism style report.
You will explore data on a topic of your choice using the data science skills you've learned in this course.
Your data collection, analysis, and final report must be all reproducible.
The specific requirements for each section of your project are detailed below.

## Project Requirements

### Data Source

Data used must be obtained via one of the following methods:

-   From a Web API using the [httr2](https://httr2.r-lib.org/) package
    -   [Open-Meteo](https://open-meteo.com/en/docs#api_documentation)
    -   [eBird](https://documenter.getpostman.com/view/664302/S1ENwy59)
    -   etc.
-   From a Web API using an API-wrapping R package
    -   [geonames](https://docs.ropensci.org/geonames/)
    -   [rebird](https://docs.ropensci.org/rebird/)
    -   etc.
-   Scrapped from the web using the [rvest](https://rvest.tidyverse.org/) package
-   Other method (by approval only)

The code you write to collect your data will be included in your final submission.
It should be inside of its own R script and *not* inside of your actual report qmd file.

### Data Analysis

Must contain all of the following items

-   **x1 custom function that performs a data wrangling task**
    -   Takes at least one argument
    -   Includes comment (inside of function body) describing what the function does and what the input arguments should be
    -   Used at least once (but ideally is used more than once)
    -   Includes at least 2 checks: implemented using `stop()`, `warning()`, or `stopifnot()`
    -   Examples:
        -   Function that cleans up a string. Applied to multiple columns using the purrr package
-   **x1 custom function that creates a plot based on user inputs**
    -   Takes at least 2 arguments (e.g., data frame value to filter some column by)
    -   Includes comment (inside of function body) describing what the function does and what the input arguments should be
    -   Used at least once (but ideally is used more than once)
    -   Includes at least 2 checks: implemented using `stop()`, `warning()`, or `stopifnot()`
    -   Examples:
        -   Function that filters a data frame so it only contains rows where column matches value provided and creates a customized plot. Used to create multiple variations of the same plot.
-   **At least 3 visualizations**
    -   Wherever possible, all visualizations have appropriately labeled axes, legends, titles, etc and are mindful of the ink/information ratio.
    -   At least one visualization MUST employ three variables (for example, x for x-axis, y for y-axis, and z for color)
    -   Beyond that, the specifics are up to you
-   **At least 1 table**
    -   Essentially a curated print out of some aspect of your data.
    -   Could highlight an interesting feature of your dataset (e.g., top 10 most popular X)...could be a summary statistics table...choice is up to you.

### Written Portions

Alongside your code chunks, please include written text.
In general, but not always, every code chunk should be accompanied by some narration.
Please avoid having long sections of code without any narrative mixed in whenever possible.

Some questions to consider when narrating code:

*Why is this code included? What does it do? Why did you make choice X and Y?*

Overall, your final document will be a mixture of code chunks and written text.
When done successfully, a reader should be able to fully understand your project without any additional explanation or guidance from you.

**General guidelines for written portions:**

-   Use complete sentences and be devoid of spelling, grammatical, and typographical errors.
-   Be well-organized. Similar thoughts should be grouped together. The document should have a purpose; every element should support this purpose.
-   Provide evidence for claims.
-   Have something important to say. The very best papers change the reader's thinking about the topic.
-   Omit needless words. Language should communicate rather than getting in the way.

### Template

**Please see `instructions/template.pdf` and `instructions/template.qmd` for what sections you are expected to include in your final report and what each entails.**
