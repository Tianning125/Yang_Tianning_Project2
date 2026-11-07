# Air Quality in Durham County

## Project Overview

This project processes daily air quality measurements and explores monthly patterns in carbon monoxide (CO), fine particulate matter (PM2.5), and ozone (O3). The report includes a data-cleaning function, annual minimum and maximum concentration tables, and two plots.

## Data Source

The CSV files were provided with the course project. They contain measurements from the EPA air pollution monitor at RDU airport for 2018, 2019, and January–April 2020.

## Files
- `data/AQ_2018.csv`: Original 2018 measurements.
- `data/AQ_2019.csv`: Original 2019 measurements.
- `data/AQ_2020.csv`: Original January–April 2020 measurements.
- `Yang_Tianning_Project2.Rproj`: RStudio project file.
- `Yang_Tianning_Project2.Rmd`: Data-cleaning function, analysis code, and report text.
- `Yang_Tianning_Project2.docx`: Word report generated from the R Markdown file.
- `README.md`: Project description and instructions.

## How to Reproduce
1. Download or clone this repository, keeping the file structure unchanged.
2. Open `Yang_Tianning_Project2.Rproj` in RStudio.
3. Install the required packages if needed:
```r
install.packages(c("tidyverse", "lubridate", "knitr", "rmarkdown"))
```
4. Open `Yang_Tianning_Project2.Rmd`.
5. Click **Knit** to generate the Word report.

The `clean_air()` function is defined in the R Markdown file. It removes exact duplicate rows, converts dates, replaces negative concentrations with zero, and calculates daily averages. Ozone concentrations are returned in ppm by default, with an option to convert them to ppb.

## Author
Tianning Yang  
Date: November 6, 2026
