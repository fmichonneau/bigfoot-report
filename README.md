# Bigfoot sightings report

A Quarto report exploring reports of Bigfoot sightings in North America. This project uses [renv](https://rstudio.github.io/renv/) to record the R packages it depends on, so you can recreate the same environment on your machine.

## Get started

1. Clone the project in RStudio: File ▸ New Project… ▸ Version Control ▸ Git, and paste the URL of this repository.
2. When the project opens, renv installs itself and reports that some packages recorded in the lockfile are not installed.
3. In the console, run:

   ```r
   renv::restore()
   ```

4. Open `bigfoot-report.qmd` and click **Render**.

## What's in the project

- `bigfoot-report.qmd`: the report
- `data/bigfoot.csv`: the sightings data
- `renv.lock`: the R version and the packages (with their versions) the report needs
- `.Rprofile`: sets the package repository to a dated snapshot of CRAN on Posit Package Manager, then activates renv when R starts
- `renv/activate.R`, `renv/settings.json`: files renv uses to activate the project library

## Data

The data comes from the [Bigfoot Field Researchers Organization (BFRO)](https://www.bfro.net/), through [data.world](https://data.world/timothyrenner/bfro-sightings-data) and [TidyTuesday](https://github.com/rfordatascience/tidytuesday/blob/main/data/2022/2022-09-13/readme.md).
