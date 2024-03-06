# Student Workload and Anxiety Study

## Introduction

Understanding the relationship between student workload and anxiety is crucial in addressing the mental well-being of students. While the general understanding is often based on personal experiences, our goal is to uncover any causal relationship between student workload and anxiety. This study aims to explore the nature of this relationship, identify influencing factors, and provide insights for education professionals and psychologists to intervene early and enhance students' mental resilience.

## Hypotheses

- **Ho (Null Hypothesis):** Student workload and student anxiety are orthogonal and insignificant.
- **H1 (Alternative Hypothesis):** Student workload and student anxiety are related and significant.

## Methods

### Data Source

We utilized a Kaggle dataset comprising 1100 observations across 21 features categorized into Psychological, Physiological, Environmental, Academic, and Social aspects.

### Experimental Design

We employed a Randomized Control Trial (RCT) along with Matching and Regression Adjustment techniques to investigate the relationship between study load and anxiety levels.

### Outcome and Treatment Variables

- **Outcome:** Anxiety Levels (0 to 21)
- **Treatment:** Having High Study Load
- **Treatment Effect:** Effect of Study Load on Anxiety Levels
- **Treatment Group:** Students with high Study Load (Study Load = 3, 4, 5)
- **Control Group:** Students with lower study load (Study Load = 0, 1, 2)

## Results

### Randomized Control Trial (RCT)

- Covariate balance was achieved using the KS Test and QQ Plots.
- The DiM indicated a slight numerical difference in anxiety levels but was not statistically significant (p-value > 0.05).
- Regression analysis further supported the insignificance of the observed difference.

### Matching and Regression Adjustment

- Matching was done using academic performance on study load.
- A calliper of 0.3 for academic performance improved match quality.
- Regression analysis on matched data revealed a statistically significant treatment effect of ~1 unit increase in anxiety for each unit increase in study load.

### Instrument Variable (IV) Analysis

- With OLS, the treatment effect was 0.92, while with IV, it increased to 5.48.
- Weak Instrument Test and Wu Hausman Test supported the use of IV.
- The final estimate with IV indicated a significant impact of study load on anxiety levels (5.48 units).

## Conclusion
Obtaining the TE of 5.48 indicates a substantial and statistically significant impact of increased study load on anxiety levels. Specifically, for every unit increase in study load, there is a corresponding increase of 5.48 units in anxiety levels. We examined marginal percentage effects by transforming the variables into log units to provide a more interpretable perspective. Consequently, our conclusion states that with a 1% increase in study load, there is an associated rise in anxiety levels by 1.93%. This analysis offers a more nuanced understanding of the proportional impact of study load on anxiety.

Our findings challenge previous literature by focusing on younger students and considering a holistic approach. We statistically demonstrate that an increase in study load has a significant impact on anxiety levels. The limitations include self-reported data, which may introduce biases. Nonetheless, our study provides valuable insights for educators and psychologists to address student anxiety at an early stage.

*Note: The data used in this study is self-reported, and caution should be taken in generalizing the findings.*


*This project was undertaken as part of the requirements for the completion of the Causal Inference course, titled Empirical Economic Analysis, instructed by Dr. Mike Aguilar at Duke University's Fuqua School of Business.*
