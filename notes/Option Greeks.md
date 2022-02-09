# Greeks
[...](https://www.youtube.com/watch?v=9E2PETrQ01M)

The option premium changes as:
- volatility changes (Vega)
- spot price changes. (Delta)
	- spot moves away or towards the strike. (Gamma)
- time pases (Theta)

## Delta (𝛿)

> Measures change in option price when stock price moves.

It is the rate of change of `Premium` w.r.t `Spot Price`.
- It reflects the increase/decrease in premium in response to 1 point movement in spot.
- It is between 0 to +1 for CE.
- It is between 0 to -1 for PE.

A 0.2 Delta means for every 100% movement in the underlying the premium will move by 20%.

### Nuances

- When someone says 20 Delta or 30 Delta they mean 0.2 Δ and 0.3 Δ respectively.
- A 30 delta options (0.3 Δ) are usually just outside (or very near) 2σ range/interval
	- The 2σ `range` give ~70% chance of max profit.
	- `2σ Range` = `-1σ` to `+1σ`
	- 30 Δ PE strike prices are very near to -1σ side of the interval.
	- 30 Δ CE strike price are very near to +1σ side of the interval.
- You can look at delta and guess the probability of being ITM (or OTM)
	- Delta represents probability of being ITM.
	- So if its -0.12 Δ then it means 12% probability of being ITM, and reverse is 82% probability of being OTM.
	- Note that these PoP/PoS calculation don't exactly match but they are around the same value.
- [How delta behaves](https://youtu.be/fZe6ClmdbZg?t=934)

### Characteristics

Understanding Delta helps in deciding what strike prices to trade and what strategies to implement.

- It depends on the market momentum.
- It depends on [[#Implied Volatility VIX]].
- It drops when VIX is falling and [[#Theta]] is nearing expiry.

### Hedging Delta
https://finance.zacks.com/hedge-stock-index-futures-4584.html

### Adjusting Delta
[...](https://www.youtube.com/watch?v=kfi2YoJVQJY)

Adjusting delta is the simplest form of risk management.

> Delta is another word for the directional risk so Managing Delta = Managing Position.

In small sized trading accounts knowing and managing deltas is an essential aspect of overall trading strategy. It is an essential risk management tool and a key to succesful trading.

Note that if you have limited capital you can make limited adjustment. It is very important that one understands this adjustment game as you cannot buy/short a lot of stocks.

- Find the overall Delta of your portolio by using the `Beta Weight Function`. For small accounts you weigh it against the index so that you commoditize everything; you want to compare apples for the apples. Check the beta weighted delta insetead of non-weighted delta. [...](https://youtu.be/kfi2YoJVQJY?t=287)

Once you find out your delta then there are many ways to adjust it higher or lower.

#### Way 1. Sell OTM Put or OTM Call Credit Spread

Managing Deltas:

| Short too many Delta | Long too many Delta  |
|----------------------|----------------------|
| Sell Put Spread OTM  | Sell Call Spread OTM |

To know that you need to sell a put against a short delta position, to know that you need to sell a call against a long delta position, to know that you can do it to find risk or naked is the key.


#### Way 2. Contrarian Play: Selling a Call/Put on Stock

Either sell a Call or a Put on an individual stock that has moved in the direction of the deltas you need to balance.

##### Examples

Scenario 1:

Say Mr. David's account is short on Apple Call with 40 Delta. Apple stock goes up. You need to neutralize this position.

You can neutralize this risk by selling some OTM Put Spread i.e, Sell puts with -20 Delta on SPY Index.

You Sell it one time you take off half your position.

You sell it two times that makes you delta flat.

Since you are short of delta, selling a few put spreads will make you a little long

When you want to define risk in a small sized account use spreads as opposed to naked options. You dont need to have a lot of money and that dont give you a lot of delta but here you need a lot of delta.

## Gamma (𝛾)

> Measures change in δ when stock price moves.

It is the rate of change of [[#Delta]].
- It is expressed in percentage/decimal.
- It reflects the change in delta in response to 1 point movement in spot.

It is the 2nd Order Greek.

### Characteristics

- Gamma is a catalyst for Delta.
- It is constantly changing even with tiny movements in spot.
	- It is at its peak when the spot is near the strike.
	- It decreases as option goes deeper into or out of the money.
	- It is 0 when the option is very deep into or out of the money.
- It dominates in absence of [[#Theta]].
	- It is extremely powerful on the day of expiry. [...](https://youtu.be/9E2PETrQ01M?t=580)
	- When you short an option, you feel safe because of the time decay. Theta is your friend only until the day of expiry. On the day of expiry Gamma becomes your enemy. 

#### Example

Say you shorted nifty at ₹15.

- Days from Monday to Wednesday pass by with no major moves in the market.
- When you are on Thursday the premium would likely be around ₹2 to ₹3. But now you don't have any Theta left to cause premium to further lose its value.
- On Thursday, the day of expiry, you dont have Theta to compensate for the radical directional moves.
- On Thursday if market does move it will cause Gamma to pump and in turn accelerate Delta. If Detla is at 0.2 it will quickly become 0.5. If your premium was ₹3, it can potentially become ₹30 in no time.
- So all Option writers should disappear before 1 PM on thursday. Leave last ₹2 to ₹3 for Gamma players.

## Theta (𝜃)

> Decay in option price every day as the expiration gets nearer.

It is the rate at which options lose its `Time Value`.
- It reflects the amount by which the premium will decrease every day.
- Its expressed in negative numbers.

### Characteristics

- The closer the option is to its expiry the greater the rate of premium decay.
- It is option seller/writer's friend.
- Theta decay is high overnight and less during the day.
- Theta decay is highest on Wednesday night.
- For a new contract that starts on Thursday, Theta Decay is lowest on Thursday, then somewhat more on Friday and so on. It is highest on Wednesday and it has to become 0 on Thursday.

Positionally it is always better to Option Selling than Option Buying.

Intraday is tough for Option Sellers because [...](https://youtu.be/9E2PETrQ01M?t=1259)

> Option buyers are mostly intraday, directional traders, gamma players, breakout traders.

> Option Sellers make more money when they hold their position overnight when there is less volatility and there are no gap-up/down.

## Implied Volatility  & VIX

### VIX

VIX is about market and its movement.

It is a measure of predicted future movement.
- It increases when there is uncertainity or anticipated news.
- It decreases in times of calm.
- It is measure of fear in the market.
- VIX behavies radically on undefined events (like COVID)

### IV

IV is about strikes and the movement of its premium.

- IV depends upon VIX and forthcoming event (expiry, budget etc).
- If VIX increases then IV increases with it but the opposite may not hold true.
	- I.e. it is not necessary that VIX too will move with IV.
	- On budget days IV crosses above 100 and VIX may not move as much on these days.
- IV behaves readically on defined events (like budgets)
	- As budget day approach IV will increase.
	- On the day of budget IV drops and starts dropping from then on.

#### Calculating IV
[...](https://www.youtube.com/watch?v=iD6Z9m4u08A)

`IV` = `1σ Expected Move`

> The implied volatility of an options is, by definition, equal to a 1 standard deviation annual expected move of the underlying.

#### Calculating Expected Move or Range using IV

`Expected % Move` = `IV` / √(365/`DTE`)
	OR
`Expected % Move` = `IV` * √(`DTE`/365)

Where
- IV = Implied Volatility
- DTE = Days to Expiration

Quick Tips
- 30 DTE => `IV` / 3.5
- 60 DTE => `IV` / 2.5
- 90 DTE => `IV` / 2

[[Standard Deviation#σ vs iv vix]]

#### Nuances

- IV has a tendency to overstate the actual volatility. So the actualy volatility is always lesser than what is indicated by the number.

### Characteristics

#### Increasing VIX

- Over 70% of the times VIX increases when the market is going down and VIX decreases when the market is going up.
- In Opstra Options Analytics, the gap between the dashed-blue-line i.e. `t+0 P&L` and the solid-green-line i.e. `P&L`. The dashed-blue-line moves away from the 0 line to the downside. [...](https://youtu.be/Uj1wAy_p_Ko?list=PLpLkTHBumJ3M4shHm45QrcWBdNG9TpSRX&t=583)
	- If VIX is increasing i.e. blue-line is moving away from the 0 line then you can control this by adding hedge i.e. buying more options.
- Option Price will not decrease
- This favours Option Buyers.
- When VIX is rising and market is falling you should LONG PE @ ITM or ATM strikes to hedge your position.

> When VIX rises `LONG PE` @ ITM/ATM Strikes.

When VIX is decreasing you will `add more LONG positions` in your overall Option Strategy. [...](https://youtu.be/9E2PETrQ01M?t=893)
- When market is going down, the premium of PE you shorted below rises sharply and shorting CEs just above won't help much. The extra shorted CE won't be able to compensate for increased PE premium.
- So when the market is falling and VIX is rising then you should LONG ITM/ATM PE on the near side.
- By adding more ITM/ATM PE LONG will make your strategy more debit but it will ensure you will not lose money.

Since increasing VIX favours Option Buyers you can NOT continue becoming an Option Writer. You will have to start converting your overall Credit Position to a Debit Position on the side which is showing rise in VIX.

#### Decreasing VIX

- Over 70% of the times VIX decreases when the market is going up.
- This favours Option Writers.
- When VIX and Market both are rising you should SHORT PE to hedge your position.

> When VIX drops `SHORT PE`.

When VIX is decreasing you will `add more SHORT positions` in your overall Option Strategy.
- When market is going up, it will test your CE so you should short more PEs.

##### Example

When elections/budget days are coming closer VIX increases and only Option Buyers make money until the day before the election/budget day. Option Writer do not make money until the day before election/budget day.

And on the day of election/bundge, as soon as Finance Minister starts speaking, the VIX starts to go down rapidly. From that day, when election/budge are done, Optoin Writer starts making money. From that day you can start adding SHORT positions to your overall strategy.

## Vega (ν)

> Measures change in option price when volatility moves.

Its a measure of impact of `changes in the underlying volatility` on the premium.
- Its the change in premium for every 1% change in [[#Implied Volatility VIX]] assumption.
	- vega is added to preimium when volatility goes up and vega is subtracted from premium when volatility drops.

### Characteristics

- premium goes up as volatility (VIX) goes up and premium falls as volatility drops.
- Longer term options have a higer vega compared to near term options.
	- Longer term options are more expensive.
	- A 1% change in IV would represent larger $ amount of that premium than an option with a lower premium.

#### Negative Vega (Sideways Market)

When you short an option, it will show (-)ve Vega.

A (-)ve Vega implies...
=> You are shorting Vega
=> You are shorting the volatility
=> Your strategy does not support volatility and it requires it to come down.
=> Your staregy will support sideways movement.

So whenever you create a complex strategy which results in a (-)ve Vega then it implies that your strategy supports sideways market movement.

##### Example

Iron Condor has (-)ve Vega and thats why they fail when there is volatility or market moves too much in one direction.

#### Positive Vega (Volatile Market)

When you long to hedge, it will show (+)ve Vega.

A Neutral to (+)ve Vega implies...
=> You are going long on Vega
=> Your staregy will support volatility.
=> Your strategy is a Debit Strategy i.e. your strategy has more longs than shorts and you have paid more for the hedges.

The farther away the expiry, the more (+)ve will be the Vega.

##### Example

When you apply calendar spread you will find (+) Vega. That is why hedges done via Calendar spread can handle volatility better i.e. if market moves too much in one direction it does not affect your position a lot.

### Hedging Vega
https://finance.zacks.com/hedge-stock-index-futures-4584.html

### Adjusting Vega

## Rho (ρ)

> Measures change in option price when stock price moves.

## Vomma

It measures the sensitivity of [[#Vega]] to the change of the [[#Implied Volatility VIX]]

It is the 2nd Order Greek.

## Vanna

It is the 2nd Order Greek.

## Veta

It is the 2nd Order Greek.

# Greek Ratios

## Delta:Theta (δ:θ) Ratio

{ `δ:θ` < `0.3 to 0.4` } => "You have `No Directoinal Risks`!"

{ `δ:θ` > `0.4` } => "You have `Directional Risks`"

> `δ:θ Ratio` helps traders who aim to earn regular monthly income rather than Long term investment.

## Vega:Theta (𝛾:θ) Ratio

{ `v:θ` < `300% to 400%` } => "You have `No Volatility Risks`!"

# Controling Greeks
[...](https://www.youtube.com/watch?v=Uj1wAy_p_Ko)

=> AKA `Trailing Stop Loss for Strategies`

Hedging by buying OTM options to safeguard 800 point movement on up and downside through V shape recovery.

# Greeks in Strategies
[...](https://youtu.be/9E2PETrQ01M?t=1323)

## Adjusting for Volatility

- If market is going to be sideways then you may keep Vega (-)ve to neutral.
- If market is going to be volatilie you should keep Vega (+)ve.

## Adjusting Credit Strategy

- Have (+)ve Theta
- Convert to `Debit Strategy` (by buying otpions to add hedges) if VIX rises.
- Exit strategy before the day of expiry and be safe from Gamma. Do not hold your positoin beyond 01:00 PM on Thursday.

## Adjusting Debit Strategy

- May have (-)ve Theta
- Convert to `Credit Strategy` (by shorting more otpions) if VIX falls.
- May hang around till the day of expiry in anticipation of a larger directional move. Gamma is your friend!

## Adjusting using Opstra
[ThetaGainers Techniques](https://www.youtube.com/watch?v=Uj1wAy_p_Ko)

### Summary

- With `Credit Strategy` have a (+)ve Theta.
- With `Debit Strategy` then prefer (-)ve Theta.
- If VIX rises adjust strategy to `Debit`.
- If VIX falls adjust strategy to `Credit`.
- Exit `Credit Strategy` before the day of expiry. Do not hold beyond 01:00 PM on Thursday.
- You may hold `Debit Strategy` till expiry in anticipation of a directional move.

![[Option Contract#Moneyness]]