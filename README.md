# Assessing greenhouse gas (GHG) emissions from nitrogenous fertilizers

This project evaluates the greenhouse gas (GHG) emissions associated with various fertilizers used in agricultural practices. The goal is to understand their contributions to total emissions and identify the most impactful types to inform sustainable fertilizer management strategies.

## Project Objectives

- **Assess GHG Emissions**: Quantify the total GHG emissions attributed to each fertilizer.
- **Compare Contributions**: Evaluate the percentage contribution of each fertilizer to the overall emissions.
- **Analyze Trends**: Explore how factors like fertilizer usage, soil pH, organic matter, and time impact GHG emissions.

## Dataset Description

The dataset used for this analysis includes the following key variables:

- **Date**: Date of fertilizer application or recording.
- **Time Index**: A numerical representation of time, calculated as the number of years since the first recorded date.
- **Usage (kg/ha)**: Fertilizer application rate in kilograms per hectare.
- **Soil pH**: A measure of soil acidity or alkalinity.
- **Organic Matter (%)**: Percentage of organic matter in the soil.l
- **Emissions Factor (kg CO2e/kg)**: Emission factor associated with the fertilizer.
- **GHG Emissions (kg CO2e/ha)**: Total GHG emissions per hectare.

## Methodology

1. **Data Preprocessing**:

   - Converted dates to a numerical time index for analysis.
   - Standardized variable names and ensured consistent units across the dataset.
2. **Regression Analysis**:

   - Built an Ordinary Least Squares (OLS) regression model to assess the relationship between GHG emissions and independent variables such as fertilizer usage, soil pH, and organic matter.
   - Analyzed coefficients, p-values, and confidence intervals to determine the significance of each factor.
3. **Emissions Contribution Analysis**:

   - Calculated the total GHG emissions for each fertilizer type.
   - Determined the percentage contribution of each fertilizer to the overall emissions.
4. **Visualization**:

   - Created scatter plots and line plots to explore relationships and trends.
   - Compared contributions of different fertilizers using tables and summaries.

## Key Results

### Regression Analysis

- **Significant Variables**:

  - **Usage (kg/ha)**: A positive and statistically significant impact on GHG emissions.
- **Insignificant Variables**:

  - **Time Index**: No significant trend over time.
  - **Soil pH and Organic Matter**: No significant impact on GHG emissions in this analysis.

### Contribution Analysis

| Fertilizer       | Total GHG Emissions (kg CO2e) | Contribution (%) |
| ---------------- | ----------------------------- | ---------------- |
| Ammonium Nitrate | 930.22                        | 24.39            |
| Ammonium Sulfate | 962.18                        | 25.23            |
| Calcium Nitrate  | 965.13                        | 25.31            |
| Urea             | 956.26                        | 25.07            |

- **Calcium Nitrate** contributes the highest emissions (25.31%), followed closely by Ammonium Sulfate and Urea.
- **Ammonium Nitrate** has the lowest contribution (24.39%).

## Insights and Recommendations

1. **Target High-Impact Fertilizers**:

   - Focus on reducing the usage or improving the efficiency of fertilizers with the highest emissions, particularly Calcium Nitrate.
2. **Adopt Sustainable Practices**:

   - Explore alternative fertilizers with lower emission factors.
   - Enhance soil management practices to improve organic matter and mitigate emissions.


## License

This project is licensed under the MIT License. See the LICENSE file for details.
