# CO2-GDP-and-Longevity

This project analyzes the relationships between CO2 emissions, GDP, and life expectancy using data from the World Bank's World Development Indicators.

## Project Overview

The study aims to understand the complex relationships between economic, environmental, and health factors across countries. It focuses on three key aspects:
1. Environmental impact (measured by CO2 emissions per capita)
2. Economic development (measured by GDP per capita)
3. Human wellbeing (measured by life expectancy at birth)

The analysis employs linear regression models to explore these relationships, considering additional factors such as:
- Access to electricity
- Secondary school enrollment
- Agriculture's share of GDP
- Income inequality (GINI index)

## Repository Structure

- [`CO2_GDP_Longevity_Analysis.Rmd`](./CO2_GDP_Longevity_Analysis.Rmd): R Markdown file containing the full analysis
- [`CO2_GDP_Longevity_Analysis.pdf`](./CO2_GDP_Longevity_Analysis.pdf): PDF output of the analysis report
- [`data/`](./data/): Directory containing data information
- [`requirements.txt`](./requirements.txt): List of R packages required to run the analysis
- [`.gitignore`](./.gitignore): Specifies intentionally untracked files to ignore

## How to Run

1. Ensure you have R and RStudio installed on your system.
2. Install the required packages listed in [`requirements.txt`](./requirements.txt).
3. Open [`CO2_GDP_Longevity_Analysis.Rmd`](./CO2_GDP_Longevity_Analysis.Rmd) in RStudio.
4. Run the chunks in the R Markdown file to reproduce the analysis.

## Results

The analysis reveals complex interactions between CO2 emissions, GDP, and life expectancy, highlighting the challenges in balancing economic development, environmental sustainability, and human wellbeing.

Key findings include:
- Economic development is associated with both increased CO2 emissions and higher life expectancy.
- Access to electricity and secondary education are positively associated with CO2 emissions.
- Higher agricultural GDP share and income inequality are associated with lower life expectancy.

For detailed results and discussion, please refer to the full report in [`CO2_GDP_Longevity_Analysis.pdf`](./CO2_GDP_Longevity_Analysis.pdf).

## Author

Hedayatullah Hakimi

## References

- World Bank. (2021). World Development Indicators.
- R Core Team. (2021). R: A language and environment for statistical computing.
- Wickham, H. et al. (2019). Welcome to the tidyverse. Journal of Open Source Software, 4(43), 1686.
