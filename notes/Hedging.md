Hedging is a way of reducing risk.

> With derivatives our primarly goal is to hedge in order to neutralize the risk (..associated with the price to be received for an asset at time T..) as much as possible.

`Hedge Expiry:` The day you close your hedge position.

# Basis Risk

## Problems

- Asset to be hedged may be different from the asset underlying the derivatives contract.
- The exact date when the asset is to be bought/sold may not be known.
- The hedge may require the futures contract to be closed out before its delivery month.

## Basis

The amount by which the spot price exceeds the futures price i.e. the difference between the spot price of an asset and its future price (on the day hedge expires).

`Basis` = `Spot price of asset to be hedged` - `Futures price of contract used`

when the futures contract is on a financial asset then Basis is calculated like so:

`Basis` = `Futures Price` - `Spot Price`

Prior to expiration the basis can be positive or negtaive.

`Zero Basis` => If the asset to be hedged and the asset underlying the futures contract are the same, the basis should be zero at the expiration of the futures contract.

`Strengthening of the basis` => Increase in the basis.

`Weakening of the basis` => Decrease in the basis.

## Choices affecting Basis Risk

44

## Stack and Roll

This means creating a long-dated futures contract by trading a series of short-dated contracts.

> You enter into "stacks" of (..sufficient..) contracts to cover exposure to the end of hedging horizon. At the end of contract expiry, you close out all contracts and "roll" them into new contracts to cover the new exposure.

You enter into a sequence of futures contracts. When the first futures contract is near expiration, it is closed out and the hedger enters into a second contract with a later delivery month. When the second contract is close to expiration, it is closed out and the hedger enters into a third contract with a later delivery month; and so on.

### Problems with stack and roll

#### No total compensation

We cannot expect a total compensation for a price decline when futures prices are below spot prices.

[[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018.pdf | Page #84, Example]]

#### Cash flow pressures

When we roll hedges forward it can lead to cash flow pressure when there are losses at the time of rolling.

# Managing Hedge

## "hedge and forget"

## "tailing the hedge"

# Hedge Scenarios

Companies take positions in derivatives to offset exposure (..of their portflio/product/service..) to the price of an (..underlying..) asset (..in the market..).

- If the exposure is such that the company gains when the price of the asset increases and loses when the price of the asset decreases, a [[#Short Hedge]] is appropriate.

- If the exposure is the such that the company gains when the price of the asset decreases and loses when the price of the asset increases, a [[#Long Hedge]] is appropriate.

## Short Hedge

This is done when a company plans to sell its asset in future but wants to prevent risks associated potential downturn price movements.

A company planning to sell an asset in distant future can lock its sell price today and prevent losses due to drop in prices later.
- Hedger may already own assets and expect to sell it in future OR
- Hedger currently may not own any assets but plans to sell soon after acquiring them.

## Long Hedge

This is done when a company plans to buy assets in future but wants to prevent risks associated with upturn price movements.

A copmany planning to purchase an asset in distant future can lock its buy price today and prevent losses due to rise in prices later.

## No Hedge

Basic governing principle is that there has to be a defined need and exposure for one to enter in to a contract toward hedging an exposure to price.

### Potentially risky hedges

Do not hedge if the basis risk is too high and/or losses from hedges cannot be offsetted by the gains from the portfolio. It becomes very difficult for hedgers to explain this situtation to senior management and bankers.

- Basis Risk
- [[#Problems with stack and roll]]

### Well-diversified portfolios

One can eliminate many risks by holding a well-diversified portfolios without any hedge.

### Competition is a Hedge

No hedging is needed when the competitive pressures within the industry are such that the prices of the goods & services produced by the industry fluctuate to reflect the underlying raw material costs, interest rates, exchange rates, and so on.

Due to this the company that does not hedge can expect its profit margins to be roughly constant. However, a company that does hedge can expect its profit margins to fluctuate!

#### Example

##### Manufacturers of gold jewelry

The cost of jewelry always reflects the price of the underlying gold so no hedging is needed as profit margin is unaffected.

- Lets say you did a short hedge to neutralize the effects of "Gold's" price movement by fixing it for today's price.
- Now lets say gold price crashes after 3 months. Then although the Gold's price would have been fixed for you, for the market it is available for cheap.
- Cheap gold would imply cheaper jewelry. Now for you the profit-margin in the produced jewelry would inevitably go down as the jewelry prices would have gone down in the industry. So now you would be making the cheaper jewelry for the gold that you hedged to lock its 3 months old price (which was higher).

[[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018.pdf | Page #68]]

##### Harvesting of Corn by farmers

Refer Problem 3.17 (Page #23 in the solutions manual)

## Cross Hedge

Cross hedging occurs when the asset being hedged is different from the asset underlying the derivative contract.

Cross hedging occurs when an asset that gives rise to the hedger's exposure is sometimes different from the asset underlying the futures contract that is used for hedging. This leads to an increase in the basis risk.

### Hedging equity portflio with index futures

A hedge using index futures removes the risk arising from market moves and leaves the hedger exposed only to the performance of the portfolio relative to the market.

```
An index is a weighted average representative sample of the market. There are many indices and each is calculated in a different way and each has a different base value. Changes in indices are calculated from a base value.

A stock index is a means of calculating a change in an economy/market. So the very number that represents an index is not as significant as the index's percentage changes.

Futures contracts on stock indices are marked-to-market and settled in cash on expiry at the closing price of last thrusday of the delivery month.
```

#### When portfolio mirror the index

N꜀ = Vₕ/V꜀

#### When portfolio does not mirror the index

You can use 𝛽 to calculate the total number of futures contracts needed for hedging and lock the benefits of a good stock picking.

N꜀ = 𝛽.(Vₕ/V꜀)

[[#Hedging an equity portflio with stock index futures]]

##### Use 𝛽 to lock stock picking benefits

𝛽 is the slope of the best-fit line obtained when `excess return on the portfolio over the risk-free rate` is regressed against the `excess return of the index over the risk-free rate`

∴ 𝛽 = (`Expected return on portfolio` - `Risk-free interest rate`) ÷ (`Return on index` - `Risk-free interest rate`)

So if you know `𝛽` of your portfolio against the index then you can predict the `percent return of the portfolio` by using `dividend yield on index` and `risk-free returns` in above formula.

Note that by calculating 𝛽 to buy proportional numbers of Index's futures contracts (N꜀) you have essentially synchronized your porfolio with market's price movement. If everything remains same then your porfolio value will not be impacted by the market as the portfolio returns will offset the market returns. Aafter synchronizing portfolio with index using 𝛽 your portfolio returns will be __relative to the market__ returns i.e. if stocks in your profolio doesn't do anything different from the market then whether market goes up or down, your portfolio will remain unaffected. So in order for you to make money the stocks in your portfolio __must outperform the market__ and only then you will make money.

# Calculating Hedge Ratios

It is the ratio of the average change in the spot price for a particular change in the futures price.

Hedge Ratio (<-- TO BE CONFIRMED)
=> `Futures Contract Size` / `Size of the Exposure`
=> `Futures Contract Size` / `Portfolio Size`

[[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018.pdf | Page #86, Summary section, para #4]]

## The Perfect Hedge Ratio

The hedge that completely eliminates the risks (..of price..) is a perfect hedge.

### Hedge Ratio of 1.0

It is natural to use hedge ratio of 1.0 when the asset underlying the futures contract is the same as the asset being hedged.

## The Optimal Hedge Ratio
=> `Minimum Variance Hedge Ratio (hᵛ)`
=> `Optimal Hedge Ratio`
=> `Best Hedge Ratio`

In cross hedging, 1.0 hedge ratio is not always an optimal ratio. You are required to calculate the minimum variance hedge ratio to calculate `the optimal number of contracts` for hedging.

You need optimal hedge ratio to find the optimal number of contracts required for hedging an asset that is not the same asset underlying the contract.

### Step 1. Calculate optimal hedge ratio

An optimal hedge ratio `minimizes the variance of the hedged position value`.

An optimal hedge ratio depends on the relationship between the changes in the spot prices and changes in the futures price.

If:

- hᵛ is the `Minimum Variance Hedge Ratio (hᵛ)`, `Best Hedge Ratio` or `Optimal Hedge Ratio`
- `ΔS` is the change in spot price, S, during a period of time equal to the life of the hedge.
- `ΔF` is the change in futures price, F, during a period of time equal to the life of the hedge.

Then:

hᵛ = Correlation between the variance of the value of an asset and that of the hedging instrument that is meant to protect it.

∴ hᵛ = The slope of the best-fit line when ΔS are regressed against ΔF. i.e. The best-fit line is created from a linear regression of ΔS against ΔF.

∴ hᵛ = The ratio of the average change in S for a particular change in F

∴ hᵛ = The product of coefficient of correlation between ΔS and ΔF

∴ hᵛ = ρ.(σₛ/σ꜀)

Where:
- σₛ is the standard deviation of ΔS
- σ꜀ is the standard deviation of ΔF
- ρ, the rho, is the coefficient of correlation between the σₛ and σ꜀ i.e. correlation between the futures price and spot price.

Note:

ρ, σₛ and σ꜀ is usually estimated from historical data on ΔS and ΔF by choosing a number of equal nonoverlapping time intervals and the values of ΔS and ΔF for each of the intervals are observed. Ideally, the length of each time interval is the same as the length of the time interval for which the hedge is in effect.

### Step 2. Calculate optimal number of contracts

#### Optimal numbers of forward contracts

The number of `forward` contracts required is given by:

N꜀ = hᵛ.(Qₕ/Q꜀)

Where:
- N꜀ is the optimal number of `forward contracts` for hedging.
- hᵛ is the `Minimum Variance Hedge Ratio (hᵛ)`, `Best Hedge Ratio` or `Optimal Hedge Ratio`.
- Qₕ is the size of position being hedged (units)
- Q꜀ is the size of 1 futures contract (units)

[[min-variance-hedge-ratio.ods]]
https://financetrain.com/minimum-variance-hedge-ratio/

#### Optimal number of futures contracts for 1 day hedge

> The σ of 1 day change in `the value of the position being hedged` is Vₕσₛₚ

Where:
- Vₕ = S x Qₕ
- Vₕ is the value of the position being hedged
- S is the spot price
- Qₕ is the size of position being hedged (units)
- σₛₚ is σ of 1 day % changes in S

> The σ of 1 day change in `the value of the futures contract` V꜀σ꜀ₚ

Where:
- V꜀ is the value of the 1 futures contract
- V꜀ = F x Q꜀
- F is the futures price
- Q꜀ is the size of 1 futures contract (units)
- σ꜀ₚ is σ of 1 day % changes in F

∴ The optimal number of `futures` contracts for a one-day hedge is given by:

=> ρₚ ([The `daily settlement` value of the position being hedged] ÷ [The `daily settlement` value of the futures contract])

=> ρₚ ([The `σ of 1 day change` in the value of the position being hedged] ÷ [The `σ of 1 day change` in the value of the futures contract])

=> ρₚ.(Vₕ.σₛₚ/V꜀.σ꜀ₚ)

> ∴ N꜀ = ₕ₁.(Vₕ/V꜀)

Where:
- N꜀ is the optimal number of `futures contracts` for hedging.
- ₕ₁ = ρₚ.(σₛₚ/σ꜀ₚ)
- ₕ₁ is the slope of the best-fit line when `% 1 day change in the portfolio` are regressed against `% 1 day changes in the futures price of the index`
- ρₚ is correlation between 1 day % changes in the spot and futures
- σₛₚ is σ of 1 day % changes in the spot price
- σ꜀ₚ is σ of 1 day % changes in the futures price
- Vₕ = S x Qₕ
- V꜀ = F x Q꜀

#### Optimal number of futures contracts close to maturity of the hedge

##### Hedging an equity portflio with stock index futures

Stock index futures can be used to hedge the systematic risk in an equity portfolio.

Note that hedge results in the investor's position growing at the risk-free rate. So you will always find a hedger's position at the end of hedge expiry to be about [risk-free-percent x hedge-period ÷ 12-months] % higher than at the beginning of the months when you entered your hedge position.

![[#Use 𝛽 to lock benefits of stock picking]]

> N꜀ = 𝛽.(Vₕ/V꜀)

Where:
- N꜀ is the optimal numbers of futures contract close to maturity of the hedge
- 𝛽 is the slope of the best-fit line when the `return from the portfolio` is regressed against the `return from the index`.
- Vₕ is the current value of the portfolio
- V꜀ is the current value of 1 futures contract

Note that 𝛽 ≈ ₕ₁ from previous section's formula.

##### Using index futures to change 𝛽

Stock index futures can also be used to change the beta of a portfolio without changing the stocks that make up the portfolio.

## The Hedge Effectiveness

The proportion of the variance that is eliminated by hedging.

Hedge Effectiveness
=> R² from the regression of ΔS against ΔF
=> ρ²

# Summary

Step #1. Calculate the number of contracts required to cross-hedge an asset.
- min. variance hedge ratio
	- s.d. of spots and futures
	- p
- value of the portfolio
- value of 1 futures contract 0

Step #2. Calculate the `P&L for futures position` for a single contract by using initial futures price and the futures price at expiry of the hedge. Multiplying this P&L value to the total number of contracts calculated in above Step #1.

Step #3. Calculate the "expected percent" return on portfolio using:
- % returns from index
- % risk-free interest rate
- beta value

Step #4. Finally calculate p&l by using percent return on portfolio calculated in the above steps #3.

Step #5. Now add results of step #2 and step #4 to get the total value of the positoin.

Conclusion: Total exepcted value of the hedger's position is almost independent of the value of the index. This is what one would expect if the hedge is a good one! So beta and p should be correctly deduced.


`Question:` Why the hedger should go to the trouble of using futures contracts to earn the risk-free interest rate, the hedger can simply sell the portfolio and invest the proceeds in a risk-free security?

`Answer:` A hedge using index futures removes the risk arising from market moves and leaves the hedger exposed only to the performance of the portfolio relative to the market.

[[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018.pdf | Page #78, #82]]