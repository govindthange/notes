
> With derivatives our primarly goal is to use hedging to neutralize the risk as much as possible.

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

## Stack & Roll

Creating a long-dated futures contract by trading a series of short-dated contracts.

You enter into a sequence of futures contracts. When the first futures contract is near expiration, it is closed out and the hedger enters into a second contract with a later delivery month. When the second contract is close to expiration, it is closed out and the hedger enters into a third contract with a later delivery month; and so on.

# Managing Hedge

## "hedge and forget"

## "tailing the hedge"

# Hedge Scenarios

Companies take positions in derivatives to offset exposure (..of their product/service..) to the price of an (..underlying..) asset (..in the market..).

## Short Hedge Scenarios

This is done when a company plans to sell the underlying asset.

A company planning to sell an asset in distant future can lock its sell price today and prevent losses due to drop in prices later.
- Hedger may already own assets and expect to sell it in future OR
- Hedger currently may not own any assets but plans to sell soon after acquiring them.

## Long Hedge Scenarios

This is done when a company plans to buy the underlying asset.

A copmany planning to purchase an asset in distant future can lock its buy price today and prevent losses due to rise in prices later.

## No Hedge Scenarios

### Competition as Hedge

No hedging is needed when the competitive pressures within the industry are such that the prices of the goods & services produced by the industry fluctuate to reflect the underlying raw material costs, interest rates, exchange rates, and so on.

Due to this the company that does not hedge can expect its profit margins to be roughly constant. However, a company that does hedge can expect its profit margins to fluctuate!

#### Example

##### Manufacturers of gold jewelry

The cost of jewelry always reflects the price of the underlying gold so no hedging is needed as profit margin is unaffected.

- Lets say you did a short hedge to neutralize the effects of "Gold's" price movement by fixing it for today's price.
- Now lets say gold price crashes after 3 months. Then although the Gold's price would have been fixed for you, for the market it is available for cheap.
- Cheap gold would imply cheaper jewelry. Now for you the profit-margin in the produced jewelry would inevitably go down as the jewelry prices would have gone down in the industry. So now you would be making the cheaper jewelry for the gold that you hedged to lock its 3 months old price (which was higher).

[[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018 | Page #68]]

##### Harvesting of Corn by farmers

Refer Problem 3.17 (Page #23 in the solutions manual)

## Cross Hedge Scenarios

Cross hedging occurs when the asset being hedged is different from the asset underlying the derivative contract.

Cross hedging occurs when an asset that gives rise to the hedger's exposure is sometimes different from the asset underlying the futures contract that is used for hedging. This leads to an increase in the basis risk.

# Calculating Hedge Ratios

It is the ratio of the average change in the spot price for a particular change in the futures price.

```WRONG <-- confirm and delete!
`Hedge Ratio`
=> `Futures Contract Size` / `Size of the Exposure`
=> `Futures Contract Size` / `Portfolio Size`
```

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

∴ hᵛ = ρ (σₛ / σ꜀)

Where:
- σₛ is the standard deviation of ΔS
- σ꜀ is the standard deviation of ΔF
- ρ, the rho, is the coefficient of correlation between the σₛ and σ꜀ i.e. correlation between the futures price and spot price.

Note:

ρ, σₛ and σ꜀ is usually estimated from historical data on ΔS and ΔF by choosing a number of equal nonoverlapping time intervals and the values of ΔS and ΔF for each of the intervals are observed. Ideally, the length of each time interval is the same as the length of the time interval for which the hedge is in effect.

### Step 2. Calculate optimal number of contracts

#### Optimal numbers of forward contracts

The number of `forward` contracts required is given by:

N꜀ = hᵛQₕ/Q꜀

Where:
- N꜀ is the optimal number of `forward contracts` for hedging.
- hᵛ is the `Minimum Variance Hedge Ratio (hᵛ)`, `Best Hedge Ratio` or `Optimal Hedge Ratio`.
- Qₕ is the size of position being hedged (units)
- Q꜀ is the size of 1 futures contract (units)

[[min-variance-hedge-ratio.ods]]
https://financetrain.com/minimum-variance-hedge-ratio/

#### Optimal number of futures contracts for 1 day hedge

`Optimal numbers of Futures Contract for Hedging` = 𝛽 x (`Total Portfolio Value` ÷ `Futures Value of 1 Contract`)

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

=> ρₚ (Vₕσₛₚ / V꜀σ꜀ₚ)

> ∴ N꜀ = ₕ₁Vₕ/V꜀

Where:
- N꜀ is the optimal number of `futures contracts` for hedging.
- ₕ₁ = ρₚ (σₛₚ / σ꜀ₚ)
- ρₚ is correlation between 1 day % changes in the spot and futures
- σₛₚ is σ of 1 day % changes in the spot price
- σ꜀ₚ is σ of 1 day % changes in the futures price
- Vₕ = S x Qₕ
- V꜀ = F x Q꜀

## The Hedge Effectiveness

The proportion of the variance that is eliminated by hedging.

Hedge Effectiveness
=> R² from the regression of ΔS against ΔF
=> ρ²