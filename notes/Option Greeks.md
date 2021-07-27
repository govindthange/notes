[...](https://www.youtube.com/watch?v=9E2PETrQ01M)

# Vega

- Its a measure of how fast an option premium can change. The speed/rate at which an option premium changes.
- When you short an option, it will show (-)ve Vega.
- When you long to hedge, it will show (+)ve Vega.

## Negative Vega (Sideways Market)

A (-)ve Vega implies...
=> You are shorting Vega
=> You are shorting the volatility
=> Your strategy does not support volatility and it requires it to come down.
=> Your staregy will support sideways movement.

So whenever you create a complex strategy which results in a (-)ve Vega then it implies that your strategy supports sideways market movement.

Example:
- Iron Condor has (-)ve Vega and thats why they fail when there is volatility or market moves too much in one direction.

## Positive Vega (Volatile Market)

A Neutral to (+)ve Vega implies...
=> You are going long on Vega
=> Your staregy will support volatility.
=> Your strategy is a Debit Strategy i.e. your strategy has more longs than shorts and you have paid more for the hedges.

The farther away the expiry, the more (+)ve will be the Vega.

Example:
- When you apply calendar spread you will find (+) Vega. That is why hedges done via Calendar spread can handle volatility better i.e. if market moves too much in one direction it does not affect your position a lot.

# VIX/IV

# Delta

It tells how much premium should change w.r.t its underlying.

Example:
- A 0.2 means for every 100% movement in the underlying the premium will move by 20%.

# Gamma

Gamma is a catalyst for Delta.
Gamma is extremely powerful on the day of expiry.

# Theta