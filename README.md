# Sleep & Cognitive Performance Analysis

## Project Overview

This project investigates the relationship between sleep duration and cognitive performance, while accounting for socio-professional categories.

### Research Question

Are differences in cognitive performance between socio-professional categories explained by sleep duration?

---

## Project Structure
project/
│
├── script.R # Main R script (complete analysis pipeline)
├── README.md # Project documentation
└── data.csv # Dataset (selected during execution)

## Installation and Usage

### 1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo

source("script.R")
A file selection window will open to choose the dataset.

Data Requirements

The dataset must include the following variables:

Variable	Type	Description
categorie_pro	Categorical	Socio-professional category
temps_sommeil_tot_h	Numeric	Total sleep duration (hours)
Score_cognitif_10	Numeric	Cognitive score (/10)
cat_sommeil	Categorical	Sleep category
cat_score	Categorical	Score category
Methods and Analyses

1. AFC (Factorial Correspondence Analysis)
Explores associations between categorical variables:

socio-professional category
sleep category
cognitive score category

2. Descriptive Statistics
Mean and standard deviation per category
Data distribution overview

3. Assumption Checks
Levene’s Test: homogeneity of variances
Shapiro-Wilk Test: normality of residuals

4. ANOVA
Tests whether cognitive scores differ significantly between categories.

5. Tukey Post-hoc Test
Identifies pairwise differences between groups.

6. Segmented Regression
Detects a breakpoint in the relationship between sleep and cognitive performance.

7. Piecewise Linear Regression
Separate analyses:

before the breakpoint
after the breakpoint

8. Piecewise ANCOVA
Tests whether group differences persist after adjusting for sleep.

9. Post-ANCOVA Tukey Test
Compares adjusted means across categories.

Key Insights
Identification of an optimal sleep duration (approximately 7–8 hours)
Significant differences between socio-professional categories
Sleep partially explains cognitive differences, but not entirely

Limitations
Synthetic dataset (simulated data)
No causal inference (correlation does not imply causation)
Limited explanatory variables

Future Improvements
Include additional variables (age, stress, health, lifestyle)
Apply more advanced statistical or machine learning models
Use real-world datasets

Acknowledgements
I would like to express my sincere gratitude to my Data Science instructor Pascal RIGOLET for his guidance, valuable feedback, and support throughout this project.

Author
Academic project developed as part of a Data Science course
L3 Biology and Health — Université Paris-Saclay
