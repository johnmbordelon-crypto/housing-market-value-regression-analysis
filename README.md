# Housing Market Value Analysis | Multiple Regression

### Statistical Analysis Portfolio | Microsoft Excel

## Project Overview

This project examines factors associated with the market value of single-family housing units using data from the **2013 American Housing Survey (AHS)**.

The analysis uses descriptive statistics, data visualization, variable transformations, and multiple linear regression to investigate relationships between housing values and property, household, and geographic characteristics.

Three regression specifications were evaluated to compare model performance and assess whether selected changes improved explanatory power.

**Tools:** Microsoft Excel  
**Dataset:** 2013 American Housing Survey  
**Regression Sample:** 31,785 observations  
**Primary Outcome:** Natural logarithm of housing market value (LN_VALUE)

## Research Question

**What factors are associated with the market value of single-family housing units?**

The analysis considers property characteristics, housing conditions, household measures, and geographic factors.

## Analytical Methodology

### 1. Data Preparation

The original dataset was filtered to focus on relevant single-family housing observations.

Data preparation included examining invalid values, removing unsuitable records, and preparing variables for regression analysis.

The cleaned regression sample contained 31,785 observations.

### 2. Descriptive Statistics and Visualization

Descriptive statistics and histograms were used to examine the distribution of housing values.

Because housing values were strongly right-skewed, a natural logarithm transformation was applied to the dependent variable.

The transformed distribution was more symmetrical, making LN_VALUE a more appropriate outcome for the regression analysis.

### 3. Multiple Regression Analysis

Three regression specifications were evaluated:

| Model | Description |
|---|---|
| Model 1 | Original regression using 14 explanatory variables |
| Model 2 | Regression excluding the bedrooms variable |
| Model 3 | Regression replacing Fair Market Rent (FMR) with its natural logarithm |

The models were compared using R-squared and adjusted R-squared.

## Key Statistical Findings

### Model Performance

The original regression model produced:

| Metric | Result |
|---|---:|
| Observations | 31,785 |
| Explanatory Variables | 14 |
| R-squared | 0.1148 |
| Adjusted R-squared | 0.1145 |

The original specification had the highest R-squared and adjusted R-squared of the three models, although the differences were small.

An R-squared of approximately 0.115 indicates that the model explains roughly 11.5% of the observed variation in log-transformed housing value.

The regression was statistically significant overall, but its limited explanatory power means it is not suitable as a reliable standalone predictor of individual home values.

### Housing Characteristics

The analysis identified associations between housing market value and selected property characteristics, including the number of rooms and indicators of housing inadequacy.

These relationships provide information about how property characteristics correspond with estimated market values after accounting for other included variables.

### Fair Market Rent Transformation

The third model evaluated the natural logarithm of Fair Market Rent.

Its coefficient of approximately 0.805 suggests that a 1% increase in FMR was associated with approximately a 0.81% increase in predicted housing value, holding the other included variables constant.

This alternative specification did not improve overall model fit.

## Conclusions

The analysis identified statistically significant relationships between housing market value and several explanatory variables. However, the models explained a relatively small share of the overall variation in housing values.

Comparing three specifications demonstrated the importance of evaluating alternative model structures rather than assuming that additional transformations or variable changes will improve performance.

The findings represent statistical associations rather than evidence of causal relationships.

## Limitations and Reproducibility

- The analysis uses historical 2013 housing survey data and should not be interpreted as reflecting current housing-market conditions.
- The relatively low R-squared limits the models' predictive usefulness.
- Regression coefficients represent associations, not causal effects.
- The workbook contains descriptive statistics, visualizations, statistical outputs, and interpretation, but does not include the cleaned row-level regression dataset.
- Consequently, the regression models cannot be independently reproduced using the published workbook alone.

## Excel and Analytical Skills Demonstrated

- Descriptive statistical analysis
- Data preparation and filtering
- Frequency distributions and histograms
- Logarithmic variable transformations
- Multiple linear regression
- Coefficient and p-value interpretation
- R-squared and adjusted R-squared comparison
- Statistical model evaluation
- Analytical reporting and communication

## Workbook Contents

| Worksheet | Contents |
|---|---|
| PROJECT INFORMATION | Project details |
| Summary Report | Written findings and interpretations |
| Data Descriptors | Descriptive statistical measures |
| Graphs and Charts | Housing-value distributions and visualizations |
| Statistical Tests | Regression outputs and comparisons |

## Data Source

U.S. Census Bureau and U.S. Department of Housing and Urban Development — 2013 American Housing Survey.

## Project Background

This analysis was originally completed as a statistics capstone assignment and adapted for a professional analytics portfolio.

It demonstrates the application of statistical methods, interpretation of quantitative evidence, and critical evaluation of model limitations.

---

*Educational statistical analysis using historical survey data. Not intended for real estate appraisal or current housing-price prediction.*
