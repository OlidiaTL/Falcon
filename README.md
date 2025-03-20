# Analyzing the Impact of Gender Integration: A Case Study of Falcon College

## Introduction
I had the privilege of being one of the "12 pioneers" of Falcon College, Zimbabwe in 2017 as one of the first 12 girls 
to join the previously all-male boarding school. 

![Pioneers](https://github.com/OlidiaTL/Falcon/blob/main/pioneers.jpg?raw=true)

This project analyzes the impact of gender integration at Falcon College, which transitioned from an all-male institution to coeducational in 2017. The study examines enrollment patterns, academic performance, and sixth form participation before and after integration.

Gender Integration stuff...............

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

