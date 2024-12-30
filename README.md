# Streaming TV Hours Analysis

## Project Overview

This project analyzes data on people watching streaming TV, focusing on estimating the factors that influence streaming hours. The dataset contains information on age, income, and coupon receipt, along with the number of streaming hours for each person in a given week. The goal is to model streaming hours using various regression techniques.

## Data Description

The dataset, `streaming_data.RData`, contains the following variables:

- **age**: Age of the person.
- **income**: Income of the person.
- **coupon**: Indicator variable for whether the person received a coupon for the streaming service.
- **streaming_hours**: Number of streaming hours watched by the person in a given week.

## Methodology

In this project, the following models were used to estimate the number of streaming hours:

1. **Ordinary Least Squares (OLS)**: Estimated a model of streaming hours using **age**, **income**, and **coupon** as explanatory variables.
2. **Tobit Model**: Applied a Tobit model to estimate streaming hours, accounting for censoring in the data.
3. **Truncated Regression**: Estimated streaming hours using truncated regression to handle data that is cut off at a certain threshold.

All three models were compared to evaluate their performance and suitability for this type of data.

## Tools and Libraries Used

- **Programming Language**: R
- **Key Libraries**: `lm`, `AER`, `tobit`, `ggplot2`, `dplyr`

## How to Run

1. Clone this repository to your local machine.
2. Load the `streaming_data.RData` dataset into R.
3. Open the R script or R Markdown file to run the analysis.

## License

This project is open-source under the [MIT License](LICENSE).
