Project Overview

This project investigates the correlation between adolescent birth rates (ABR) and climate change-induced natural disasters using data from the World Bank and the International Disasters Database. The objective is to assess whether increased natural disaster intensity and frequency, driven by climate change, correlate with changes in adolescent birth rates across countries.
Linear regression models are employed to explore this relationship, focusing on the impact of natural disaster frequency, intensity, and the number of individuals affected by disasters.

1. Imputation Decision.ipynb
This notebook decides which countries' natural disaster intensity data should be imputed based on the percentage of data availability.
Countries with significant missing data are either excluded or imputed using various techniques depending on data patterns.
The decision-making process relies on data completeness and aims to balance robustness with the size of the dataset.
2. Impute total affected data.Rmd
This RMarkdown file performs imputation for the "total affected" data column, which represents the number of individuals affected by natural disasters.
It uses statistical methods like mean, median imputation, or more advanced techniques such as multiple imputation depending on the data characteristics.
3. Natural Disaster Frequency vs. ABR dataframe creation.ipynb
This notebook creates the final dataframe by merging natural disaster frequency data with adolescent birth rate data.
It processes the raw data to ensure it is suitable for analysis, handling missing values, normalizing variables, and ensuring consistent units of measurement across the datasets.
4. Process International Disasters Database Data.ipynb
This notebook processes the raw data from the International Disasters Database. It cleans, filters, and formats the disaster data, focusing on intensity, frequency, and affected population metrics.
It prepares the data for merging with the World Bank data and regression analysis.
5. Process imputed intensity data.ipynb
This notebook processes the imputed disaster intensity data, making it suitable for merging with other data sources.
The focus is on creating a clean, consistent dataset that accurately reflects the intensity of natural disasters after handling missing values through imputation.
6. Processing World Bank Indicators.ipynb
This notebook processes the World Bank indicators, particularly focusing on confounding variables that may affect the relationship between adolescent birth rates and natural disasters.
Variables like GDP, education, and healthcare access are processed to control for external factors in the regression analysis.
7. Regressions.Rmd
This RMarkdown file runs linear regression models to examine the relationship between natural disaster metrics (frequency, intensity, total affected) and adolescent birth rates.
Various models are explored, with and without controlling for confounding variables, to identify the strength and significance of the correlation.
8. Total Affected vs. ABR merge.ipynb
This notebook merges the imputed total affected data with adolescent birth rate data, preparing it for regression analysis.
It ensures the datasets are aligned by country and year, and processes any remaining inconsistencies.
