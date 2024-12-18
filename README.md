# Applied Statistics - By Joanne Feeney

## Introduction
This repository contains my work for the "Applied Statistics" module, taught by ATU Galway. The repository includes two Jupyter notebooks and a folder containing datasets used throughout the course:

- **Notebooks:**
  - `tasks.ipynb` – contains solutions to four tasks related to statistical analysis.
  - `project.ipynb` – contains a final project where I analyze the "PlantGrowth" dataset using statistical methods.

- **Folder:**
  - `datasets/` – contains all the datasets used in the notebooks.

All work was completed using **Visual Studio Code**. I recommend using this editor for optimal experience with the notebooks.

Some tasks and the project were assisted by **GitHub Co-Pilot**:
[GitHub Co-Pilot](https://github.com/features/copilot)

## Tasks

The following tasks are completed in `tasks.ipynb`:

### Task 1: Permutations and Combinations
This task modifies the Lady Tasting Tea experiment to involve twelve cups of tea. The goal is to calculate the probability that a person can correctly identify six cups with milk in them.

- **Analysis:** I calculate the probability of selecting the correct six cups, and then test how the probability changes when allowing for one or two errors.
- **Conclusion:** I conclude that allowing for two errors significantly increases the probability of guessing correctly, making it less likely for me to accept such errors.

### Task 2: numpy's Normal Distribution
In this task, I test if `numpy.random.normal()` generates values that properly follow a normal distribution.

- **Method:** I generate 100,000 random values with a mean of 10 and standard deviation of 3. Then, I use `scipy.stats.shapiro()` to test for normality and visualize the distribution with a histogram and Q-Q plot.
- **Conclusion:** My analysis shows that `numpy.random.normal()` generates values that closely follow a normal distribution.

### Task 3: t-Test Calculation
This task involves calculating the t-statistic for a dataset containing resting heart rates of patients before and after a two-week exercise program.

- **Method:** I visualize the data using strip and box plots, then perform a t-test using Python and compare my result to the value obtained from `scipy.stats`.
- **Conclusion:** The t-statistics from my calculations and `scipy.stats` match, confirming the validity of the t-test.

### Task 4: ANOVA
This task estimates the probability of committing a Type II error in an ANOVA test.

- **Method:** I generate three samples with slightly different means (4.9, 5.0, and 5.1) using `numpy.random.normal()`. I perform one-way ANOVA 10,000 times and track the occurrence of Type II errors.
- **Conclusion:** I conclude that the probability of committing a Type II error is 0%, as the differences in means are adequately detectable.

## Project: PlantGrowth Analysis

The project in `project.ipynb` focuses on analyzing the **PlantGrowth** dataset from R.

- **Dataset:** The dataset contains two variables:
  - `group`: The treatment group (e.g., ctrl, trt1, trt2).
  - `weight`: The weight of plants in each group.

### Objectives:
- Perform **t-tests** and **ANOVA** to analyze the significance of differences between plant groups.
- Describe the dataset, the statistical methods used, and the assumptions made.

### Key Steps:
1. **Data Download:** The dataset was downloaded and saved to the repository.
2. **t-Test:** I performed a t-test to check if there’s a significant difference between two treatment groups, `trt1` and `trt2`.
3. **ANOVA:** I performed ANOVA to check for significant differences between the three groups: `ctrl`, `trt1`, and `trt2`.
4. **Reasoning:** I explain why ANOVA is more appropriate than multiple t-tests when analyzing more than two groups.

### Conclusion:
The results from both the t-test and ANOVA reveal significant differences between the groups, with ANOVA being the more appropriate test for comparing multiple groups.

## Conclusion

This repository demonstrates various statistical methods, including permutations, normal distributions, t-tests, and ANOVA, through practical exercises and a final project. It provides both the Python code used and detailed explanations of the underlying statistical concepts.
