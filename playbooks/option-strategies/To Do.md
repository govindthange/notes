
- Check behavior of option buying w/o hedge.
- Check behavior of option selling w/o hedge.
- Check behavior of spreads.
- Check behavior of calendar spreads.
- Check beahvior of inverse calendar spreads.
- Try sar+macd+stoch straregy with vertical spreads (not naked option buys)

- Add winning/losing streak counts along with percent gain for winning and losing streaks to the indicator


# Bollinger Band

## Go Short

### Entry Approach 1
Trigger #1
  - candle #1 `touches` the upper band- DEFAULT (OR candle #1 `closes` above the upper band - CONFIGURABLE)
      AND candle #1 low doesn't `touch` the midline/SMA of BB

Trigger #2
  - canlde #2 closes below the `low` of candle #1 (OR candle #2 closes below the `close` of candle #1)
      AND candle #2 doesn't touch the upper band
      AND candle #2 doesn't `touch` the midline/SMA of BB (OR candle #2 doesn't `close` below the midline)

### Entry Approach 2
Trigger #1
  - candle #1 low is above the upper band without touching it.

Trigger #2
  - canlde #2 closes below the low of candle #1
      AND candle #2 doesn't touch the midline/SMA of BB (OR candle #2 doesn't close below the midline)

### Entry Approach 3

Think about using 5 EMA w/ BB

### Entry Approach 3

Entry Approach 1 + Entry Approach 2

### Enter the trade

> Do not enter if the price is below the midline/SMA of BB.

Enter at the open of candle #3 with
  - SL at high of candle #1 (use ATR)
  - Target at 1:2, 1:3 (configurable)

> Try implementing an optional critera that requires the lower band to be sufficiently distant for reasonable gains. Keep this option disabled because enabling it might lead to missing out on substantial moves, as when the Bollinger Bands are flat and narrow, there is a higher likelihood of a significant price movement.

### Exit Approach 1

Exit when
- Following HOLD/NURTURE criteria satisfies
  - (Do not close for the 1st n candles - make it configurable (n=3 by default) - during this exit only upon SL/Target)
- Candle closes above the previous candle `high` (OR candle closes above the previous candle `close`)
  - Use candle close above the previous candle high IN SIDEWAYS MARKET. Use indicators like choppiness index to read consolidation.
  - Use candle close above the previous candle close IN TRENDING MARKET. Use indicators like choppiness index to read consolidation.
- A candle touches the lower band

### Exit Approach 2

Exit when
- Following HOLD/NURTURE criteria satisfies
  - (Do not close for the 1st n candles - make it configurable (n=3 by default) - during this exit only upon SL/Target)
- Candle closes above the previous candle `high` (OR candle closes above the previous candle `close`)
  - Use candle close above the previous candle high IN SIDEWAYS MARKET. Use indicators like choppiness index to read consolidation.
  - Use candle close above the previous candle close IN TRENDING MARKET. Use indicators like choppiness index to read consolidation.
- DO NOT EXIT WHEN THE LOWER BAND IS TOUCHED

### Exit Approach 3

Add a 5 EMA

- Exit when any candle opens, and closes above the 5 EMA without its low touching the 5 EMA.