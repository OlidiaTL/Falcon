# Analyzing the Impact of Gender Integration: A Case Study of Falcon College

## Introduction
I had the privilege of being one of the "12 pioneers" of Falcon College, Zimbabwe in 2017 as one of the first 12 girls 
to join the previously all-male boarding school. 

![Pioneers](https://github.com/OlidiaTL/Falcon/blob/main/pioneers.jpg?raw=true)

This project analyzes the impact of gender integration at Falcon College, which transitioned from an all-male institution to coeducational in 2017. The study examines enrollment patterns, academic performance, and sixth form participation before and after integration.

## Data Preparation

### Data Cleaning and Preprocessing

To prepare the data for analysis, I performed several key data cleaning and preparation steps:

1. **Column Name Standardization**:
   - Standardized enrollment data columns to ['Year', 'Male', 'Female']
   - Added a calculated 'Total' column (sum of Male and Female students)
   - Standardized sixth form data columns to ['Year', 'L6_Male', 'L6_Female', 'U6_Male', 'U6_Female']
   - Renamed pass rate data columns to ['Year', 'IGCSE', 'AS', 'A_Level']

2. **Derived Metrics**:
   - Created 'Total_L6' (sum of L6_Male and L6_Female)
   - Created 'Total_U6' (sum of U6_Male and U6_Female)
   - Calculated 'Total' sixth form enrollment (sum of Total_L6 and Total_U6)

3. **Integration Period Identification**:
   - Determined that gender integration began in 2017 (first year with Female > 0)
   - Added a 'Period' column to all datasets, categorizing data into 'Pre-Integration' (2011-2016) and 'Post-Integration' (2017-2023)

4. **Data Validation**:
   - Verified data completeness across all years (2011-2023)
   - Confirmed consistency in metrics across datasets
   - Ensured proper data types for all variables

This data preparation created a structured foundation for subsequent exploratory and statistical analyses, enabling direct comparison between pre and post-integration periods.

Exploratory Data Analysis (EDA)

This section presents a comprehensive analysis of the data collected from Falcon College between 2011 and 2023, with a particular focus on examining the impact of gender integration which began in 2017.

## Summary Statistics

### Enrollment Patterns

Analysis of enrollment data reveals significant changes following gender integration in 2017:

- **Pre-Integration Period (2011-2016)**: 
  - Average total enrollment: 425.00 students (SD = 16.79)
  - 100% male student population
  - Enrollment ranged from 396 to 441 students

- **Post-Integration Period (2017-2023)**:
  - Average total enrollment: 446.71 students (SD = 53.57)
  - Male students: 360.57 on average (SD = 9.90)
  - Female students: 86.14 on average (SD = 52.02)
  - Enrollment ranged from 380 to 510 students

The data shows an overall **5.11% increase** in total enrollment after gender integration, suggesting that the introduction of female students expanded the college's reach. The standard deviation for the post-integration period is notably higher, indicating greater enrollment variability during this transition period.

### Age Distribution

The age distribution of students shows some interesting patterns:

- **U13-U14 Age Groups**: Notable increases post-integration, with U13 increasing from an average of 53.33 to 66.71 students, and U14 increasing from 73.33 to 82.71 students
- **U16-U17 Age Groups**: Slight decreases post-integration
- **U19 Students**: Slight increase from an average of 14.67 to 16.00 students

These changes suggest that gender integration may have particularly affected enrollment in the younger age groups, potentially indicating changing recruitment patterns or increased appeal to families with younger students.

### Sixth Form Enrollment

The sixth form data reveals shifts in upper-level education at the college:

- **Lower 6 (L6)**:
  - Pre-integration: 69.83 students on average (all male)
  - Post-integration: 56.71 male students and 8.86 female students, for a total of 65.57
  - This represents a **6.10% decrease** in overall L6 enrollment

- **Upper 6 (U6)**:
  - Pre-integration: 54.50 students (all male)
  - Post-integration: 53.86 students (combined male and female)
  - This represents a **1.18% decrease** in U6 enrollment

The data suggests that sixth form enrollment was slightly lower in the post-integration period, particularly in the Lower 6 form. This could indicate challenges in transitioning the sixth form program during integration or changing student preferences.

### Academic Performance

Analysis of pass rates across different examination levels shows mixed results:

- **IGCSE Pass Rates**:
  - Pre-integration: 80.67% average pass rate (SD = 3.20)
  - Post-integration: 76.00% average pass rate (SD = 3.16)
  - This represents a **4.67 percentage point decrease**

- **AS Level Pass Rates**:
  - Pre-integration: 81.67% average pass rate (SD = 3.39)
  - Post-integration: 80.00% average pass rate (SD = 3.74)
  - This represents a **1.67 percentage point decrease**

- **A Level Pass Rates**:
  - Pre-integration: 89.33% average pass rate (SD = 3.01)
  - Post-integration: 92.50% average pass rate (SD = 3.08)
  - This represents a **3.17 percentage point increase**

These results suggest a complex relationship between gender integration and academic performance, with lower-level examinations showing slight declines in pass rates, while advanced A Level results improved. This pattern could reflect a period of adjustment followed by stronger academic performance at higher levels.

### Time Series Analysis

#### Enrollment Trends
![Enrollment Trends at Falcon College (2011-2023)](https://github.com/OlidiaTL/Falcon/blob/main/year_students.png?raw=true)

The enrollment visualization reveals:

- **Total enrollment** declined initially after integration but grew steadily afterwards, reaching approximately 510 students by 2022 (17.6% higher than pre-integration average)
- **Male enrollment** decreased consistently post-integration, dropping from approximately 400 to 350 students
- **Female enrollment** grew steadily from zero in 2016 to around 150 students by 2023
- The net growth in total enrollment is entirely attributable to female students, which more than offset the decline in male enrollment

#### Academic Performance Trends
![Academic Performance Trends at Falcon College (2011-2023)](https://github.com/OlidiaTL/Falcon/blob/main/year_pass.png?raw=true)

Analysis of pass rates shows differentiated impacts across examination levels:

- **A Level performance** (green line) showed consistent improvement post-integration, with pass rates reaching 95-96% in 2019 and 2021, compared to a pre-integration high of 93%
- **AS Level results** (orange line) initially declined after integration but recovered to fluctuate between 77-85%
- **IGCSE performance** (blue line) experienced the most substantial drop, declining to 71% in 2018 before partial recovery

This pattern suggests that advanced academic levels may have adapted more successfully to gender integration than foundation levels.

#### Sixth Form Enrollment Trends
![Sixth Form Enrollment Trends at Falcon College (2011-2023)](https://github.com/OlidiaTL/Falcon/blob/main/year_sixthform.png?raw=true)

The sixth form data shows:

- **Total sixth form enrollment** (green line) maintained relative stability, fluctuating between 110-130 students throughout both periods
- **Lower 6 (L6) enrollment** (blue line) shows similar variability pre and post-integration, with a recent peak of approximately 83 students in 2022
- **Upper 6 (U6) enrollment** (orange line) shows no clear directional change attributable to gender integration

Unlike overall enrollment, sixth form participation patterns appear less directly affected by gender integration.

### Distribution Analysis

To understand statistical variations in key metrics before and after gender integration, I analyzed distributions using multiple visualization techniques including boxplots, violin plots, density plots, and histograms.

#### Total Enrollment Distribution
![Total Enrollment Distribution Analysis](https://github.com/OlidiaTL/Falcon/blob/main/bunch.png?raw=true)

The enrollment distribution analysis reveals:

- **Boxplot Analysis**: Pre-integration enrollment showed a tight distribution (narrow IQR) centered around 425-430 students, while post-integration enrollment exhibits substantially greater variability with a higher median (~445) and upper values extending to 510+ students.

- **Violin Plot Analysis**: The violin plots further illustrate this difference in distribution shapes. Pre-integration enrollment follows a relatively symmetric distribution, while post-integration enrollment shows a bimodal distribution with peaks around 380-400 students and 500-510 students, suggesting two distinct enrollment patterns after integration.

- **Density Plot Analysis**: The pre-integration density curve shows a narrow, peaked distribution centered around 425-440 students, while the post-integration curve is wider and flatter, extending from approximately 380 to 600 students. This confirms the considerably broader range of enrollment figures after gender integration.

- **Histogram Analysis**: The histogram provides additional evidence of the varied enrollment patterns post-integration, with both lower (380-400) and higher (480-510) enrollment counts represented, supporting the bimodal pattern seen in the violin plot.

This analysis reveals that gender integration not only affected average enrollment but fundamentally altered enrollment patterns, creating greater year-to-year variability. This suggests the college experienced distinct phases during the transition period.

#### Academic Performance Distributions
![Pass Rate Distribution Analysis](https://github.com/OlidiaTL/Falcon/blob/main/bunch2.png?raw=true)

The distribution analysis for academic performance shows varying patterns across examination levels:

**IGCSE Pass Rates**:
- The boxplot shows a clear downward shift in IGCSE pass rates, with the median dropping from approximately 80% pre-integration to 76% post-integration.
- The violin plot indicates a wider spread of results post-integration, with the distribution extending lower (to approximately 71%).
- The density plot shows the pre-integration distribution centered around 80-82%, while the post-integration distribution is centered around 75-76%, with a left shift in the overall distribution.

**AS Level Pass Rates**:
- The boxplot indicates minimal change in median AS Level pass rates, but with increased variability in the post-integration period, particularly toward lower values.
- The violin plot shows that the post-integration distribution extends both higher and lower than the pre-integration distribution, suggesting more unpredictable results.
- The density plot confirms this pattern, with the post-integration curve showing a wider spread with a longer tail toward lower values.

**A Level Pass Rates**:
- The boxplot reveals a clear upward shift in A Level pass rates, with the median increasing from approximately 88-89% pre-integration to 93-94% post-integration.
- The violin plot shows not only higher values but also a generally tighter distribution post-integration in the higher range.
- The density plot illustrates the pre-integration distribution centered around 87-88%, while the post-integration distribution is shifted right to 92-95%, with minimal overlap.

These distribution analyses reveal a nuanced pattern across academic levels:
1. IGCSE performance shows a negative shift
2. AS Level shows minimal change in central tendency but increased variability
3. A Level shows a clear positive shift

This suggests that the impact of gender integration varied significantly by academic level, with potentially negative short-term effects on lower-level examinations but positive effects on advanced studies.

### Correlation Analysis

To explore relationships between enrollment metrics and academic performance, I conducted correlation analysis using both correlation matrices and pair plots.

#### Correlation Matrix
![Correlation Matrix of Enrollment and Academic Performance](https://github.com/OlidiaTL/Falcon/blob/main/corr_matrix.png?raw=true)

The correlation matrix reveals several significant relationships:

- **Male Enrollment and IGCSE Performance**: Strong positive correlation (r = 0.71), suggesting that higher male enrollment was associated with better IGCSE pass rates.

- **Male Enrollment and A Level Performance**: Moderate negative correlation (r = -0.42), indicating that higher male enrollment was associated with somewhat lower A Level pass rates.

- **Female Enrollment and IGCSE Performance**: Moderate negative correlation (r = -0.45), showing that as female enrollment increased, IGCSE pass rates tended to decrease.

- **Female Enrollment and A Level Performance**: Weak positive correlation (r = 0.33), suggesting a modest association between increased female enrollment and improved A Level results.

- **Male and Female Enrollment**: Strong negative correlation (r = -0.67), reflecting the substitution effect as the college transitioned from all-male to mixed-gender enrollment.

- **Total Enrollment and Academic Performance**: Negligible correlations with all academic metrics (r ≈ 0.05), indicating that overall enrollment size had little relationship with academic outcomes.

These correlation patterns support the observation that the impact of gender integration varied across academic levels, with IGCSE performance showing negative associations with the demographic shift, while A Level performance showed potential benefits from increased female representation.

#### Relationships Between Variables
![Relationships Between Enrollment and Academic Performance](https://github.com/OlidiaTL/Falcon/blob/main/scatter.png?raw=true)

The pair plot provides further insights into these relationships:

- **Total Enrollment Patterns**: The top-left panel shows the clear separation between pre-integration (red, clustered around 420-440) and post-integration periods (blue, more widely distributed).

- **Female Enrollment Distribution**: The density plot in the second row clearly shows the transition from zero female enrollment pre-integration to a growing female population post-integration.

- **IGCSE vs. Female Enrollment**: The scatter plot (row 3, column 2) shows that increasing female enrollment coincided with decreasing IGCSE pass rates, visualizing the negative correlation.

- **A Level vs. Female Enrollment**: The scatter plot (row 4, column 2) illustrates that higher female enrollment generally corresponded with higher A Level pass rates in the post-integration period.

- **IGCSE vs. A Level Performance**: Examining the relationship between different academic levels (row 4, column 3) shows that in the post-integration period (blue points), there was a negative relationship between IGCSE and A Level performance (r = -0.50), suggesting that resources or focus may have shifted between these academic levels.

This multi-dimensional analysis suggests that gender integration created a complex redistribution of academic outcomes, with advanced academic levels potentially benefiting at the expense of foundation levels during the transition period.

### Statistical Testing

To determine whether observed differences between pre and post-integration periods were statistically significant, I conducted hypothesis testing using independent samples t-tests with Welch's correction for unequal variances.

#### Hypothesis Testing Results

**Total Enrollment:**
- Pre-Integration Mean: 425.00 (SD = 16.79)
- Post-Integration Mean: 446.71 (SD = 53.57)
- Absolute Change: +21.71 students
- Percent Change: +5.11%
- T-statistic: -1.016, P-value: 0.3421
- Effect Size (Cohen's d): 0.528 (medium)
- Interpretation: The increase in total enrollment is not statistically significant, though it represents a medium effect size.

**IGCSE Pass Rates:**
- Pre-Integration Mean: 80.67% (SD = 3.20)
- Post-Integration Mean: 76.00% (SD = 3.16)
- Absolute Change: -4.67 percentage points
- Percent Change: -5.79%
- T-statistic: 2.539, P-value: 0.0294
- Effect Size (Cohen's d): 1.466 (large)
- Interpretation: The decrease in IGCSE pass rates is statistically significant with a large effect size.

**AS Level Pass Rates:**
- Pre-Integration Mean: 81.67% (SD = 3.39)
- Post-Integration Mean: 80.00% (SD = 3.74)
- Absolute Change: -1.67 percentage points
- Percent Change: -2.04%
- T-statistic: 0.809, P-value: 0.4375
- Effect Size (Cohen's d): 0.467 (small)
- Interpretation: The decrease in AS Level pass rates is not statistically significant and represents a small effect size.

**A Level Pass Rates:**
- Pre-Integration Mean: 89.33% (SD = 3.01)
- Post-Integration Mean: 92.50% (SD = 3.08)
- Absolute Change: +3.17 percentage points
- Percent Change: +3.54%
- T-statistic: -1.800, P-value: 0.1020
- Effect Size (Cohen's d): 1.039 (large)
- Interpretation: The increase in A Level pass rates, while not quite reaching statistical significance (p = 0.10), represents a large effect size.

**Lower 6 Enrollment:**
- Pre-Integration Mean: 69.83 (SD = 7.14)
- Post-Integration Mean: 65.57 (SD = 8.75)
- Absolute Change: -4.26 students
- Percent Change: -6.10%
- T-statistic: 0.967, P-value: 0.3545
- Effect Size (Cohen's d): 0.529 (medium)
- Interpretation: The decrease in Lower 6 enrollment is not statistically significant but represents a medium effect size.

**Upper 6 Enrollment:**
- Pre-Integration Mean: 54.50 (SD = 7.58)
- Post-Integration Mean: 53.86 (SD = 7.88)
- Absolute Change: -0.64 students
- Percent Change: -1.18%
- T-statistic: 0.150, P-value: 0.8838
- Effect Size (Cohen's d): 0.083 (negligible)
- Interpretation: The minimal change in Upper 6 enrollment is not statistically significant and represents a negligible effect size.

#### Summary of Statistical Findings

The statistical analysis reveals that among all metrics examined, only the decline in IGCSE pass rates reached statistical significance (p < 0.05). However, several metrics showed medium to large effect sizes despite not reaching statistical significance, likely due to the relatively small sample size (pre-integration n=6, post-integration n=7).

The most notable patterns are:
1. The decline in IGCSE pass rates is both statistically significant and shows a large effect size
2. The improvement in A Level pass rates, while not quite statistically significant (p = 0.10), shows a large effect size
3. Changes in enrollment metrics (total, L6, U6) were not statistically significant

These findings suggest that gender integration had its most measurable impact on academic performance metrics rather than on enrollment figures, with differing effects across academic levels.

### Advanced Statistical Analysis

#### Hypothesis Testing with Confidence Intervals

I conducted formal hypothesis testing to rigorously assess differences between pre and post-integration periods:

**Null Hypothesis (H₀)**: There is no difference in metrics between pre and post gender integration periods.  
**Alternative Hypothesis (H₁)**: There is a difference in metrics between pre and post gender integration periods.

**Total Enrollment:**  
There is no statistically significant difference in Total Enrollment between pre and post integration periods (t(7.3)=-1.016, p=0.3421). Enrollment increased by 5.11% with a medium effect size (Cohen's d=0.53). 95% CI [-28.37, 71.79]

**IGCSE Pass Rate:**  
There is a statistically significant difference in IGCSE Pass Rate between pre and post integration periods (t(10.0)=2.539, p=0.0294). Pass rates decreased by 5.79% with a large effect size (Cohen's d=1.47). 95% CI [-8.76, -0.57]

**AS Level Pass Rate:**  
There is no statistically significant difference in AS Level Pass Rate between pre and post integration periods (t(9.9)=0.809, p=0.4375). Pass rates decreased by 2.04% with a small effect size (Cohen's d=0.47). 95% CI [-6.26, 2.93]

**A Level Pass Rate:**  
There is no statistically significant difference in A Level Pass Rate between pre and post integration periods (t(10.0)=-1.800, p=0.1020). Pass rates increased by 3.54% with a large effect size (Cohen's d=1.04). 95% CI [-0.75, 7.09]

The confidence intervals provide additional context: while IGCSE pass rates show a statistically significant decline (CI excludes zero), A Level pass rates show a strong positive effect that approaches but doesn't quite reach significance at the conventional p<0.05 threshold.

#### Two-Way ANOVA Analysis

To understand potential interaction effects between integration period and examination type, I conducted a two-way ANOVA:

| Factor | Sum of Squares | df | F-value | p-value |
|--------|---------------|-----|---------|---------|
| Period | 10.03 | 1.0 | 0.936 | 0.341 |
| Exam Type | 1065.06 | 2.0 | 49.692 | <0.001 |
| Period × Exam Type | 93.72 | 2.0 | 4.373 | 0.022 |
| Residual | 321.50 | 30.0 | | |

The ANOVA results reveal:

1. **Period Effect**: The main effect of integration period alone was not statistically significant (p=0.341)
2. **Exam Type Effect**: There was a highly significant difference between exam types (p<0.001)
3. **Interaction Effect**: Crucially, the interaction between period and exam type was statistically significant (p=0.022)

This significant interaction confirms that gender integration had differential effects across academic levels—a finding consistent with our earlier observations that IGCSE performance decreased while A Level performance improved. The interaction effect explains why analyzing each exam type separately revealed different patterns.

This analysis provides strong statistical evidence that gender integration created a redistribution of academic outcomes across different examination levels, rather than a uniform effect across all academics.

### Advanced Analysis Techniques

To strengthen causal inferences about the impact of gender integration, I employed several advanced analytical techniques beyond basic statistical testing.

#### Difference-in-Differences Analysis

I used difference-in-differences (DiD) analysis to compare changes in IGCSE and A Level pass rates, treating IGCSE as the "control" group and A Level as the "treatment" group, with gender integration as the intervention.

**Raw DiD Estimate:**
- IGCSE Pass Rate Change: -4.67 percentage points
- A Level Pass Rate Change: +3.17 percentage points
- Difference-in-Differences Estimate: +7.83 percentage points

**Regression-Based DiD Analysis:**

| Coefficient | Estimate | Std Error | t-value | p-value | [95% Conf. Interval] |
|-------------|----------|-----------|---------|---------|----------------------|
| Intercept | 80.67 | 1.27 | 63.42 | 0.000 | [78.01, 83.32] |
| Post-integration | -4.67 | 1.80 | -2.59 | 0.017 | [-8.42, -0.91] |
| Is_alevel | 8.67 | 1.80 | 4.82 | 0.000 | [4.91, 12.42] |
| Interaction | 7.83 | 2.54 | 3.08 | 0.006 | [2.53, 13.14] |

The DiD analysis provides strong evidence (p=0.006) that gender integration had a significantly different effect on A Level performance compared to IGCSE performance. The positive interaction coefficient (7.83) indicates that relative to IGCSE results, A Level performance improved by 7.83 percentage points after gender integration.

This finding supports the hypothesis that gender integration created differential impacts across academic levels, with advanced studies benefiting while foundation studies faced challenges.

#### Regression Discontinuity Design

I implemented a regression discontinuity design (RDD) to estimate the immediate effect of gender integration on A Level pass rates, using time (centered at the integration year) as the running variable:

**RDD Estimate for A Level Pass Rate:** +2.55 percentage points
**Pre-Integration Slope:** +0.40 (slight upward trend before integration)
**Post-Integration Slope:** -0.31 (slight downward trend after the initial increase)

The RDD analysis suggests an immediate positive shift in A Level pass rates at the point of integration, though the effect moderated somewhat in subsequent years.

#### Predictive Modeling for Future Trends

Using time series analysis (ARIMA modeling), I forecasted enrollment trends for the next five years:

**Total Enrollment Forecast:**
- Year 2024: 496 students
- Year 2025: 494 students
- Year 2026: 493 students
- Year 2027: 493 students
- Year 2028: 493 students

**Female Percentage Forecast:**
- Year 2024: 28.6%
- Year 2025: 27.7%
- Year 2026: 26.8%
- Year 2027: 26.0%
- Year 2028: 25.3%

The forecasting model suggests that total enrollment will stabilize around 493-496 students, while the female percentage may gradually decrease to approximately 25% by 2028. This suggests the college may be approaching a new equilibrium state where enrollment growth has plateaued and gender proportions are stabilizing.

These advanced analytical techniques provide complementary evidence for causal impacts of gender integration while offering insights into potential future trends at Falcon College.

## Executive Summary

This study analyzes the impact of gender integration at Falcon College, which transitioned from an all-male institution to coeducational in 2017. Using data from 2011 to 2023, I examined enrollment patterns, academic performance, and sixth form participation before and after integration.

Key findings reveal that gender integration had complex and varied effects: total enrollment increased by 5.11%, with female enrollment steadily growing while male enrollment declined. Academic performance showed differentiated impacts across examination levels—IGCSE pass rates significantly decreased by 5.79% (p=0.0294), while A Level pass rates increased by 3.54% (not statistically significant but with a large effect size). Advanced statistical techniques including difference-in-differences analysis confirm that integration had significantly different effects across academic levels (p=0.006).

The results demonstrate that educational institutions implementing gender integration should anticipate multifaceted impacts and prepare strategies to manage the transition, particularly at foundation academic levels.

## Conclusions and Discussion

The analysis of Falcon College's gender integration reveals several important patterns and insights:

1. **Successful Expansion of Educational Access**: The steady growth in female enrollment from zero to approximately 150 students over seven years demonstrates significant demand for girls' education at this institution. This expansion more than offset the decline in male enrollment, resulting in overall growth.

2. **Transition Period Variability**: The increased variability in enrollment and academic metrics post-integration suggests the college experienced a transition period with greater fluctuations before establishing new patterns.

3. **Differential Academic Impact**: The statistically significant interaction between period and exam type (p=0.022) confirms that gender integration affected academic levels differently. The decline in IGCSE performance coupled with improvement in A Level results could indicate:
   - Resource reallocation during transition
   - Different adaptation rates among student age groups
   - Potential benefits of gender diversity in advanced academic settings
   - Possible changes in admission standards or student demographics

4. **Sixth Form Stability**: The relative stability in sixth form enrollment despite overall demographic changes suggests institutional capacity constraints or deliberate enrollment management at upper levels.

These findings align with educational research suggesting that institutional transitions often produce variable outcomes across different metrics and student populations. The mixed academic results highlight that integration processes require careful management, particularly in supporting foundation-level students during the transition.

## Recommendations

Based on this analysis, I recommend the following for educational institutions considering or implementing gender integration:

1. **Anticipate Demographic Shifts**: Prepare for potential changes in gender balance and overall enrollment patterns. Monitor male enrollment rates and develop strategies to maintain appeal to both genders.

2. **Target Support for Foundation Levels**: Provide additional academic support specifically for lower examination levels (e.g., IGCSE), where integration appears to have more challenging impacts.

3. **Leverage Advanced Level Benefits**: Capitalize on the potential positive effects of gender diversity at advanced academic levels, which may benefit from mixed-gender learning environments.

4. **Implement Phased Integration**: Consider a gradual approach to integration that allows for adaptation at each academic level.

5. **Monitor Key Metrics**: Establish systems to track enrollment, academic performance, and student satisfaction throughout the transition process.

6. **Prepare for Increased Variability**: Build flexibility into planning to accommodate greater variability in key metrics during the transition period.

## Limitations of the Study

This analysis has several limitations that should be considered when interpreting the results:

1. **Small Sample Size**: With only 6 pre-integration and 7 post-integration time points, statistical power is limited, potentially obscuring real effects.

2. **Potential Confounding Factors**: The analysis could not control for other factors that might have influenced outcomes during this period, such as:
   - Changes in school leadership or teaching staff
   - Curriculum or assessment changes
   - Broader educational trends in Zimbabwe
   - Economic or social factors affecting enrollment

3. **Limited Variables**: The analysis focuses on enrollment and academic performance but lacks data on other important factors such as:
   - Student satisfaction
   - Teacher perspectives
   - Classroom dynamics
   - Extracurricular participation

4. **Short Post-Integration Timeline**: Seven years may be insufficient to observe the full long-term effects of gender integration.

5. **Correlation vs. Causation**: While advanced techniques like difference-in-differences strengthen causal claims, definitive causal relationships remain challenging to establish with observational data.

## How to View the Complete Analysis

The full Jupyter notebook with detailed code and additional visualizations is available:

[View this analysis in nbviewer](https://nbviewer.org/github/OlidiaTL/Expedia/blob/main/Expedia.ipynb)

