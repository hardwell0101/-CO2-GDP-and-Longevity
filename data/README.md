# Data Source and Retrieval for CO2-GDP-and-Longevity Project

This project uses data from the World Bank's World Development Indicators (WDI) database. The data is retrieved directly using the `WDI` package in R, so no local data files are stored in this repository.

## Variables Used

The following indicators are used in this analysis:

1. NY.GDP.PCAP.KD: GDP per capita (constant 2015 US$)
2. SP.DYN.LE00.IN: Life expectancy at birth, total (years)
3. SE.SEC.ENRR: School enrollment, secondary (% gross)
4. EG.ELC.ACCS.UR.ZS: Access to electricity, urban (% of urban population)
5. NV.AGR.TOTL.ZS: Agriculture, forestry, and fishing, value added (% of GDP)
6. SI.POV.GINI: Gini index (World Bank estimate)
7. EN.ATM.CO2E.PC: CO2 emissions (metric tons per capita)

## Data Retrieval

To retrieve the data, the R script uses the following code:

```r
library(WDI)

countries <- "all"
years <- c(2010:2020)

indicators <- c("NY.GDP.PCAP.KD", "SP.DYN.LE00.IN", "SE.SEC.ENRR", 
                "EG.ELC.ACCS.UR.ZS", "NV.AGR.TOTL.ZS", "SI.POV.GINI", "EN.ATM.CO2E.PC")

data <- WDI(country = countries, indicator = indicators, start = years[1], end = years[length(years)])
```

This retrieves data for all countries from 2010 to 2020 for the specified indicators.

## Data Processing

After retrieval, the data is processed as follows:
1. Columns are renamed for clarity
2. Rows with missing values are removed

For more details on data preparation and analysis, please refer to the main R Markdown file (`CO2_GDP_Longevity_Analysis.Rmd`) in the root directory of this repository.

## Accessing the Data

To access the original data or for more information about the indicators, visit the World Bank's World Development Indicators website:
https://databank.worldbank.org/source/world-development-indicators