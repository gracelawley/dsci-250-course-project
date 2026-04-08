# Data Source

**Due: Monday, 04/13/26, 11:59 pm**

A compressed R Project folder (.zip) that contains the following:

1.  `00_get-data.R`
    -   R Script
    -   Contains all of your code for collecting your data from a web API or by web scraping
    -   The initial output of your data collection (data frame, list, etc.) should be saved as a .csv or .rds object inside of a folder called `data/`
    -   Note: The only code in this script should be for the initial data collection. Please put any code for further data wrangling in your `01_data-source.qmd` document.
2.  `01_data-source.qmd`
    -   Quarto document
    -   Code for reading in the output of `00_get-data.R`
    -   If the output of `00_get-data.R` is already a data frame, then proceed to the data source description outlined below.
        -   If not, then perform any data wrangling now to make it into a data frame, but please delay any drastic changes (e.g., reshaping) until later.
    -   **Tell me about the data you are planning to use. If you have more than one data set (not required), repeat this for each.**
        -   **Data**
            -   Print out the actual data frame. The whole thing, so don't use `glimpse()`, just write the object name.
            -   Please include the html document option `df-print: paged` in your YAML header to prevent all rows from being shown at once when rendered.
        -   **Data file source**
            -   Name of the source
            -   Link to the website where the data came from
            -   Short description of what the data set is
            -   Note: often the same data set can be found in many different places online. Provide the link to where YOU will be getting the data from for this project.
        -   **Original source**
            -   Who originally collected the data?
            -   Link if you have one
            -   Note: not necessarily the same as the data file source!
        -   **Data collection process**
            -   How did you get this data? Web API, web scraping, something else?
            -   If from a Web API, did it require an API key?
            -   How did this step go? Was it straight-forward? Difficult? Surprising?
        -   **Initial format of collected data**
            -   Data frame? List? Something else?
            -   Note: It should already be a data frame at this point.
        -   **Current unit of analysis**
            -   What does each row in the data file currently represent?
            -   You may want to or need to change this during your analysis, but aren’t required to.
            -   If you already know that you will change this, please mention this here.
        -   **Number of rows and columns**
            -   Flexible, but recommended minimum is 1,000 rows
            -   Flexible, but recommended minimum is 5 columns
        -   **Description of columns**
            -   If there are too many to reasonably list, just describe the ones you plan to use
3.  `01_data-source.html`
    -   Rendered html version of `01_data-source.qmd`
    -   Please include the html document option `self-contained: true` in your YAML header so there is not an accompanying `*_files` folder.
4.  `data/`
    -   A folder that contains the output(s) of `00_get-data.R`
5.  **All other files inside of your project folder, such as the actual `.Rproj` file**
