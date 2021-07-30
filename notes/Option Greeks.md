# Greeks
[...](https://www.youtube.com/watch?v=9E2PETrQ01M)

The option premium changes as:
- volatility changes (Vega)
- spot price changes. (Delta)
	- spot moves away or towards the strike. (Gamma)
- time pases (Theta)

## Delta

It is the rate of change of `Premium` w.r.t `Spot Price`.
- It reflects the increase/decrease in premium in response to 1 point movement in spot.
- It is between 0 to +1 for CE.
- It is between 0 to -1 for PE.

### Characteristics

- It depends on the market momentum.
- It depends on [[#Implied Volatility VIX]].
- It drops when VIX is falling and [[#Theta]] is nearing expiry.

#### Example

A 0.2 means for every 100% movement in the underlying the premium will move by 20%.

## Gamma

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

## Theta

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

## Implied Volatility (VIX)

It is a measure of predicted future movement.
- It increases when there is uncertainity or anticipated news.
- It decreases in times of calm.

### Characteristics

#### Increasing VIX

- 70% of the time VIX increases when the market is going down.
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

- 70% of the time VIX decreases when the market is going up.
- This favours Option Writers.
- When VIX and Market both are rising you should SHORT PE to hedge your position.

> When VIX drops `SHORT PE`.

When VIX is decreasing you will `add more SHORT positions` in your overall Option Strategy.
- When market is going up, it will test your CE so you should short more PEs.

##### Example

When elections/budget days are coming closer VIX increases and only Option Buyers make money until the day before the election/budget day. Option Writer do not make money until the day before election/budget day.

And on the day of election/bundge, as soon as Finance Minister starts speaking, the VIX starts to go down rapidly. From that day, when election/budge are done, Optoin Writer starts making money. From that day you can start adding SHORT positions to your overall strategy.

## Vega

Its a measure of impact of `changes in the underlying volatility` on the premium.
- Its the change in premium for every 1% change in [[#Implied Volatility VIX]] assumption.
	- vega is added to preimium when volatility goes up and vega is subtracted from premium when volatility drops.

### Characteristics

- premium goes up as volatility goes up and premium falls as volatility drops.
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

## Vega:Theta (v:θ) Ratio

{ `v:θ` < `300% to 400%` } => "You have `No Volatility Risks`!"


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

### Summary

- With `Credit Strategy` have a (+)ve Theta.
- With `Debit Strategy` then prefer (-)ve Theta.
- If VIX rises adjust strategy to `Debit`.
- If VIX falls adjust strategy to `Credit`.
- Exit `Credit Strategy` before the day of expiry. Do not hold beyond 01:00 PM on Thursday.
- You may hold `Debit Strategy` till expiry in anticipation of a directional move.