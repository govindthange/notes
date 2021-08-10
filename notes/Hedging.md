
> With derivatives our primarly goal is to use hedging to neutralize the risk as much as possible.

`Hedge Expiry:` The day you close your hedge position.

# Basis Risk

## Problems

- Asset to be hedged may be different from the asset underlying the futures contract.
- The exact date when the asset is to be bought/sold may not be known.
- The hedge may require the futures contract to be closed out before its delivery month.

## Basis

The amount by which the spot price exceeds the futures price i.e. the difference between the spot price of an asset and its future price on the day hedge expired.

`Basis` = `Spot price of asset to be hedged` - `Futures price of contract used`

when the futures contract is on a financial asset then Basis is calculated like so:

`Basis` = `Futures Price` - `Spot Price`

Prior to expiration the basis can be positive or negtaive.

`Zero Basis` => If the asset to be hedged and the asset underlying the futures contract are the same, the basis should be zero at the expiration of the futures contract.

`Strengthening of the basis` => Increase in the basis.

`Weakening of the basis` => Decrease in the basis.

## Choices affecting Basis Risk

44

## Stack & Roll

Creating a long-dated futures contract by trading a series of short-dated contracts.

You enter into a sequence of futures contracts. When the first futures contract is near expiration, it is closed out and the hedger enters into a second contract with a later delivery month. When the second contract is close to expiration, it is closed out and the hedger enters into a third contract with a later delivery month; and so on.

# Managing Hedge

## "hedge and forget"

## "tailing the hedge"

# Hedge Scenarios

## Short Hedge Scenarios

This is done when a company plans to sell the underlying asset.

- Hedger already owns an asset and expect to sell it at some time in the future.
- Hedge does not own an asset right but will be owned and ready for sale at some time in the future.

## Long Hedge Scenarios

This is done when a company plans to buy the underlying asset.

- Copmany knows it will have to purchase a certain asset in the future and wants to lock in a price now.

## No Hedge Scenario

### Competition as Hedge

Competitive pressures within the industry may be such that the price of the goods and services produced by the industry fluctuate to reflect the underlying raw material costs, interest rates, exchange rates, and so on.

Due to this the company that does not hedge can expect its profit margins to be roughly constant. However, a company that does hedge can expect its profit margins to fluctuate!

- Manufacturers of gold jewelry: the cost of jewelry always reflects the price of the underlying gold so no hedging is needed as profit margin is unaffected.
	- Lets say you did a short hedge to neutralize the effects of "Gold's" price movement by fixing it for today's price.
	- Now lets say gold price crashes after 3 months. Then although the Gold's price would have been fixed for you, for the market it is available for cheap.
	- Cheap gold would imply cheaper jewelry. Now for you the profit-margin in the produced jewelry would inevitably go down as the jewelry prices would have gone down in the industry. So now you would be making the cheaper jewelry for the gold that you hedged to lock its 3 months old price (which was higher).
	- [[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018 | Page #68]]
- Harvesting of Corn by farmers
	- Refer Problem 3.17 (Page #23 in the solutoins manual)

## Cross Hedge Scenario

Cross hedging occurs when the asset being hedged is different from the asset underlying the futures.

Cross hedging is when an asset that gives rise to the hedger's exposure is sometimes different from the asset underlying the futures contract that is used for hedging. This leads to an increase in the basis risk.

# Calculating Hedge

Companies take positions in derivatives to offset (..their product/service's..) exposure to the price of an asset (..in the market..).

`Hedge Ratio`
=> `Futures Contract Size` / `Size of the Exposure`
=> `Futures Contract Size` / `Portfolio Size`

`Required number of Futures Contract for Hedging` = B x (`Total Portfolio Value`/`Futures Value of 1 Contract`)

## The Perfect Hedge

The hedge that completely eliminates the risks (..of price..) is a perfect hedge.

### Hedge Ratio of 1.0

It is natural to use hedge ratio of 1.0 when the asset underlying the futures contract is the same as the asset being hedged.

### Optimal Hedge Ratio
=> `Best Hedge Ratio`
=> `Minimum Variance Hedge Ratio (hᵛ)`

In cross hedging, 1.0 hedge ratio is not always an optimal ratio. You are required to calculate the minimum variance hedge ratio to calculate `the optimal number of contracts` for hedging.

#### Step 1. Calculate optimal hedge ratio

An optimal hedge ratio minimizes `the variance of the value of the hedged position`.

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

∴ hᵛ = ρ (σₛ / σ𝒻)

Where:
- σₛ is the standard deviation of ΔS
- σ𝒻 is the standard deviation of ΔF
- ρ, the rho, is the coefficient of correlation between the σₛ and σ𝒻 i.e. correlation between the futures price and spot price.

Note:

ρ, σₛ and σ𝒻 is usually estimated from historical data on ΔS and ΔF by choosing a number of equal nonoverlapping time intervals and the values of ΔS and ΔF for each of the intervals are observed. Ideally, the length of each time interval is the same as the length of the time interval for which the hedge is in effect.

#### Step 2. Calculate optimal number of contracts 

##### For Forward Contracts

The number of `forward` contracts required is given by:

N꜀ = hᵛQₕ/Q꜀

Where:
- N꜀ is the optimal number of futures contracts for hedging.
- hᵛ is the `Minimum Variance Hedge Ratio (hᵛ)`, `Best Hedge Ratio` or `Optimal Hedge Ratio`.
- Qₕ is the size of position being hedged (units)
- Q꜀ is the size of 1 futures contract (units)

[[min-variance-hedge-ratio.ods]]
https://financetrain.com/minimum-variance-hedge-ratio/

##### For Futures Contracts

If:
- σₛ is the standard deviation of percentage one-day day changes in the spot price
- σ𝒻 is the standard deviation of percentage one-day changes in the futures price
- ρ is correlation between parcentage one-day changes in spot and futures

Then:
- The standard deviation of the one-day change in the vlaue of the position being hedged is `Vₕσₛ`, where `Vₕ` is the value of the position i.e. `Asset Price` times `Qₕ`
- The standard deviation of the one-day change in the value of the futures position is `V꜀σ𝒻`, where `V꜀` is the `Futures Price` times `Q꜀`.

The optimal number of `futures` contracts for a one-day hedge is is given by:

N꜀ = hVₕ/V꜀

Where:
- N꜀ is the optimal number of futures contracts for hedging.
- h = ρ (σₛ / σ𝒻)
- Vₕ is the value of the position (i.e. asset price times Qₕ).
- V꜀ is the futures price times Q꜀.
- Qₕ is the size of position being hedged (units)
- Q꜀ is the size of 1 futures contract (units)

## The Hedge Effectiveness

The proportion of the variance that is eliminated by hedging.

Hedge Effectiveness
=> R² from the regression of ΔS against ΔF
=> ρ²