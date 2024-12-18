# Applied Statistics
## By Joanne Feeney

## Introduction

This repository was created for my work on the "Applied Statistics" module, taught by ATU Galway.

It contains two Jupyter notebooks titled `tasks.ipynb` & `project.ipynb` and a folder titled `datasets`, which contains all the datasets used for these notebooks.

All the work that I have completed was done so on Visual Studio Code. I would recommend that this editor is used by anyone viewing the notebooks in this repository.

Some of the tasks and the project were created with the help of Github Co-Pilot: https://github.com/features/copilot

## Tasks

All 4 tasks are completed in `tasks.ipynb` and labelled accordingly.

### Task 1: Permutations and Combinations

**Altering the Lady Tasting Tea experiment to involve twelve cups of tea.**

I calculate, using Python, the probability that a person (assuming they have no special powers) select the correct six cups which had milk in first.

I then investigate if I am willing to accept one error (i.e. the person will guess five of the six cups correctly). 

I calculate the probability that the person makes one error and then the difference if I allow for two errors.

My conclusion is that I would not accept two errors as the probability that the person guesses correctly increases dramatically.

### Task 2: numpy's Normal Distribution

**Assessing whether numpy.random.normal() properly generates normal values.**

I generate a sample of one hundred thousand values with mean 10.0 and standard deviation 3.0.

I use the scipy.stats.shapiro() function to test whether the created sample came from a normal distribution.

I use a histogram & q-q plot to assist in visualising the sample data.

I plot a histogram of the values and the corresponding normal distribution probability density function on top of it.

My results suggest that numpy.random.normal() appears to properly generate normal values.

### Task 3: t-Test Calculation

**Calculating the t-statistic of a provided dataset containing resting heart rates for patients before and after embarking on a two-week exercise program.**

I use the help of a stripplot and a boxplot to visualise the data.

I perform a t-test and calculate the t-statistic on this dataset, using Python. 

I compare it to the value given by scipy.stats. 

The t-statstics vs. scipy.stats t-test result shows that both display the same value and probability.

### Task 4: ANOVA

**Estimating the probability of committing a type II error in specific circumstances.**

I create a variable called `no_type_ii` and set it to 0.

I use numpy.random.normal to generate three samples with 100 values each. Each has a standard deviation of 0.1. The means are 4.9, 5.0 and 5.1.

I perform one-way anova on the three samples and add 1 to `no_type_ii` whenever a type II error occurs.

I use a loop to perform the test 10,000 times.

In conclusion I am rejecting the (false) null hypothesis for this test. The probability of committing a type II error is 0%.

The means of the three samples are adequately different.

*******************************

## Project

My project code is in a file called `project.ipynb`.

In this project, I analyze the [PlantGrowth R dataset](https://vincentarelbundock.github.io/Rdatasets/csv/datasets/PlantGrowth.csv).

The dataset contains two main variables, a treatment group and the weight of plants within those groups.

I perform t-tests and ANOVA on this dataset while describing the dataset and explaining my work.


I have successfully:

1. Downloaded and saved the dataset to my repository.

2. Described the dataset in the above notebook.

3. Described what a t-test is, how it works, and what my assumptions are.

3. Performed a t-test to determine whether there is a significant difference between the two treatment groups `trt1` and `trt2`.

4. Performed ANOVA to determine whether there is a significant difference between the three treatment groups `ctrl`, `trt1`, and `trt2`.

5. Explained why it is more appropriate to apply ANOVA rather than several t-tests when analyzing more than two groups.
