# CS3

This repository contains all of the materials necessary to complete this case study, including the hook document, rubric, data, code, and supplemental materials.

## Section 1: Software and platform

**Software Used:**
- R Studio for time series modeling and forecasting.
- Git for version control and GitHub for hosting.

**Add-on R packages required (install with `install.packages()` or via `renv`)**
- `tidyverse` (includes `dplyr`, `ggplot2`, `readr`, `tibble`, etc.)
- `rmarkdown`, `knitr` (rendering reports) , `forecast`

## Section 2: Map of Documentation

 1. **Data**
  - `mean_max_monthly_temps_2000_2025.csv` – Just the mean maximum monthly temperature data. 
  - `mean_min_monthly_temps_2000_2025.csv` – Just the mean mimimum monthly temperature data. 
 2. **Scripts**
  - `ModelBuilding.Rmd` – Model building script where time series model is fitted and forecats are made.
 3. **Supplemental Materials**
  - `A Practical Guide to ARIMA with auto.arima Function in R | by Zaki Nurkholis | Medium.pdf` – Article on the technicalbackground of building ARIMA models and making forecasts.
  - `What Is Climate Change? | United Nations.pdf` – Writing on the importance of studying temperatures rising.
 4. **Hook Document.pdf**
 5. **README.md**
 6. **Weather Temperatures Case Study Rubric.pdf**


## Section 3 – How to Reproduce Our Results

If you want to reproduce our analysis and see all the figures and tables from our project, follow these steps:

1. **Get the Repository**
   - Clone the repo using Git:
     ```bash
     git clone https://github.com/2014cb22-del/CS3.git
     ```
   - Or download it as a ZIP file and extract it.
   - Open RStudio and set your working directory to the project folder.

2. **Make Sure the Data Files Are There**
   - The following CSV files need to be in the **same folder** as `ModelBuilding.Rmd`:
     - `mean_max_monthly_temps_2000_2025.csv`
     - `mean_min_monthly_temps_2000_2025.csv`
   - These files are included in the repository, so you shouldn’t need to download anything else.

3. **Install R and Packages**
   - We used **R** (version 4.0 or higher) and RStudio.
   - Install the packages we used if you don’t already have them:
     ```r
     install.packages(c("tidyverse", "dplyr", "ggplot2",
                        "tidytext", "forecast", "knitr", "rmarkdown"))
     ```

4. **Run the Analysis**
   - Open `ModelBuilding.Rmd` in RStudio.
   - Feel free to change the h values in the forecast function to predict more into the future (set to 12 right now to predict 12 months into future)
   - Click **Knit** to run all the code and generate the full report.
   - This will produce the HTML (or PDF) report with all of our results, including plots, tables, and model outputs.

5. **Troubleshooting**
   - Make sure your working directory is the project folder and the CSV files are in the right place.
   - If anything seems off, you can run `sessionInfo()` in R to check your package versions.
  
## References

Nurkholis, Z. “A Practical Guide to ARIMA with auto.arima Function in R.” Medium, 2021, https://medium.com/@mouse3mic3/a-practical-guide-to-arima-with-auto-arima-function-in-r-252aa84232af

United Nations. “What Is Climate Change?” UN Climate Change. Web. https://www.un.org/en/climatechange/what-is-climate-change





