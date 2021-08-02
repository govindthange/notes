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

σ² = Σ(x-μ)²/(n-1)

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

## Standard Deviation (σ)

Standard Deviation
=> The measure of spread.
=> The amount of variation within data.
=> Distribution of occurrences around the mean (μ).

σ = √(Σ(x-μ)²/(n-1))

Standard Deviation tells how spread out a set of data is. It tells how much does the data vary from the average. Larger the Standard Deviation, the larger the dispersion.

It helps in determining whether the value is statistically significant or a part of expected variation.

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
