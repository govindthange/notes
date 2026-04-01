[...](https://www.youtube.com/watch?v=cyt_Hsjc518)

# Basics

## Mean (μ)

Mean => The Average Value

Its the average value calculated by adding all the values and dividing by the total number of values.

μ = Σxi / n

where:
- μ: A symbol called "mu" that indicates the mean.
- Σ: A symbol called "summation" that means the sum.
- xi: The ith observation in a dataset
- n: The total number of observations in the dataset

##### Example

Data = {7, 11, 11, 15, 20, 20, 28}
n = 7

μ = Σxi/n
  = 112/7
  = 16

## Median

Median => The Middle Value

Its the middle most value in the series.

When a distribution is skewed, the median does a better job of describing the center of the distribution than the mean when there are outliers present in the data.

##### Example

Data = {7, 11, 11, 15, 20, 20, 28}
Median = 15

Data = {2, 5, 6, 7, 13, 25, 33, 50}
Median = (7+13)/2
	   = 10

## Mode

Mode => The Frequent Value

The most frequent value i.e. the value that appears the most.

##### Example

Data = {7, 11, 11, 15, 20, 20, 28}
Mode = {11, 20}

## Range

Range => The difference between the MAX and the MIN value in a given series.

## Variance (σ²)

Variance
=> Its a measure of variability of the observation with a set.
=> The degree of spread in your data set.
=> Its a measure of how data points differ from the mean.
=> i.e. `how far a set of numbers are` spread out from their average value.
=> i.e. the average distance of a set of variable from the average value in that set.

Variance is the average of the squared differences from the mean.
- Variance uses squares because it weighs outliers more heavily than the data closer to the mean.
- We square so that negative distances do not cancel positive distances. i.e. differences above the mean do not cancel out those below the mean, which would result in a variance of zero. ^9ab9b8
- It is calculated by taking the average of squared deviations from the mean.

variance = σ² = Σ(x-μ)²/(n-1)

where:
- μ is the mean.
- Σ is the sum.
- σ² is the variance
- n is the sample size

##### Example

Data = {7, 11, 11, 15, 20, 20, 28}
n = 7

μ = Σxi/n
  = 112/7
  = 16

| x  | μ  | (x-μ) | (x-μ)² |
|----|----|-------|--------|
| 7  | 16 | -9    | 81     |
| 11 | 16 | -5    | 25     |
| 11 | 16 | -5    | 25     |
| 15 | 16 | 1     | 1      |
| 20 | 16 | 4     | 16     |
| 20 | 16 | 4     | 16     |
| 28 | 16 | 12    | 144    |

Σ(x-μ)² = 308

σ² = Σ(x-μ)²/(n-1)
   = 308 / (7-1)
   = 308 / 6
   = 51.34

The variance can be useful when you’re using a technique like `ANOVA` or `Regression` and you’re trying to explain the total variance in a model due to specific factors.

##### Example

You might want to understand how much variance in test scores can be explained by IQ and how much variance can be explained by hours studied. If 36% of the variation is due to IQ and 64% is due to hours studied, that’s easy to understand. But if we use the standard deviations of 6 and 8, that’s much less intuitive and doesn’t make much sense in the context of the problem.

Reading:
- https://chris-said.io/2019/05/18/variance_after_scaling_and_summing/

### Variance vs Standard Deviation

==TO BE CLARIFIED==

- σ is the measure of dispersion where as variance is the measure of variability.
- σ tells you to what extent/amount (in percent; imagine the size of the bell curve and 64-95-99 % rules) the data is likely to vary around its mean whereas variance tells you how far a set of numbers are spread out from their average value.
- σ is the average distance that a value lies from the mean while the variance tells us the square of this value.

## Standard Deviation (σ)

Standard Deviation
=> Its a measure of [[#Dispersion]] of observation within a set.
=> The measure of spread.
=> The amount of variation within data.
=> i.e. `by how much amount the data is likely to vary` around its average.
=> Distribution of occurrences around the mean (μ).
=> It calculates how far from the mean a group of numbers is by using the square root of variance.

σ = √(Σ(x-μ)²/(n-1))

Standard Deviation tells how spread out a set of data is. It tells how much does the data vary from the average. Larger the Standard Deviation, the larger the dispersion.

It helps in determining whether the value is statistically significant or a part of expected variation.

### Dispersion

Dispersion means how squeezed or scattered the variable is.

The dispersion means the (..far..) extent to which a numerical data is `likely` (..68% of the time..) to vary around its average value.

#### Types of Measures of Dispersion

There are two main types of dispersion methods in statistics which are:

1. Absolute Measure of Dispersion
2. Relative Measure of Dispersion

#### Relative measure of Dispersion

It is used to `compare the distribution of two or more data sets`. This measure compares values without units.

Common relative dispersion methods include:

1. Co-efficient of Range
2. Co-efficient of Variation
3. Co-efficient of Standard Deviation
4. Co-efficient of Quartile Deviation
5. Co-efficient of Mean Deviation

#### Co-efficient of Dispersion

It is calculated (along with the measure of dispersion) `when two series are compared`, that differ widely in their averages. The dispersion coefficient is also used when two series with different measurement units are compared. It is denoted as C.D.

##### Example

Data = {7, 11, 11, 15, 20, 20, 28}
n = 7

μ = Σxi/n
  = 112/7
  = 16

| x  | μ  | (x-μ) | (x-μ)² |
|----|----|-------|--------|
| 7  | 16 | -9    | 81     |
| 11 | 16 | -5    | 25     |
| 11 | 16 | -5    | 25     |
| 15 | 16 | 1     | 1      |
| 20 | 16 | 4     | 16     |
| 20 | 16 | 4     | 16     |
| 28 | 16 | 12    | 144    |

Σ(x-μ)² = 308

![[#^9ab9b8]]

σ² = Σ(x-μ)²/(n-1)
   = 308 / (7-1)
   = 308 / 6
   = 51.34

σ = √51.34
  = 7.165

# Calculating Standard Deviation

## Simple Data
[...](https://www.youtube.com/watch?v=179ce7ZzFA8)

## Price Data
[...](https://www.youtube.com/watch?v=omVKR85pw2s)

## Indicators

- Linear Regression (TradingView - Built-ins)
- StdDev Indicator (wpatte15)
- [[Bollinger Bands]] (TradingView - Built-ins)

# Quantifying a Move: Standard Deviation
[...](https://youtu.be/omVKR85pw2s?t=338)

# Trading σ
[...](https://www.youtube.com/watch?v=pqe-MUcQsMY)

## σ vs iv/vix
[...](https://youtu.be/StEHQgvVoto?t=692)

### IV Definition

iv = vix = 1σ expected move
=> A stock will close within 1σ 68.2% of the time.

The volatility of an option is by definition equal to a 1 standard deviation expected move. [...](https://www.youtube.com/watch?v=RMRWlwcKmJA)

`Question:` Why Standard Deviation is used as a `Volatility` measure?

`Answer:` It emphasizes the outliers i.e. it is sensitive to breakouts and adaptive to changes in regime. The σ calculation magnifies the big deviations from price away from the average.

## The 68/95/99 Rule

![Standard Deviation Graph](standard-deviation-4sigma.jpg)

A stock will close:
- within 1σ 68.2% of the time
- within 2σ 95.4% of the time
- within 3σ 99.7% of the time

### The 2σ Move

- It is where the Buying Power Reduction (BPR) is set.
- The risk while trading derivatives is inside this 2σ move.
- If your BPR is based off of 2σ then that is a reasonable expectation for max risk.

## The VIX Position / 1σ Short Option

If we sell an OTM put at 1σ below the stock price, it has an 84% probability of finishing OTM. [...](standard-deviation-4sigma.jpg)

Understand that selling options is certainly very risky but it is considerably easier to manage 1 loser against 9 winners compared to managing 9 losers against 1 winner.
