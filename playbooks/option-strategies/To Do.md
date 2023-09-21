
- Check behavior of option buying w/o hedge.
- Check behavior of option selling w/o hedge.
- Check behavior of spreads.
- Check behavior of calendar spreads.
- Check beahvior of inverse calendar spreads.

# Bollinger Band

## Go Short

### Entry Approach 1
Trigger #1
  - candle #1 candle#1 touches the upper band- DEFAULT (OR closes above the upper band - CONFIGURABLE)
      AND candle #1 low doesn't touch the midline of BB
      AND lower band is far enough for reasonable gains

Trigger #2
  - canlde #2 closes below the low of candle #1 (OR candle #2 closes below the close of candle #1)
      AND candle #2 doesn't touch the upper band
      AND candle #2 doesn't touch the midline of BB

Enter at the open of candle #3 with
  - SL at high of candle #1 (use ATR)
  - Target at 1:2, 1:3 (configurable)

### Entry Approach 2
Trigger #1
  - candle #1 low is above the upper band
      AND lower band is far enough for reasonable gains

Trigger #2
  - canlde #2 closes below the low of candle #1
      AND candle #2 doesn't touch the midline of BB

Enter at the open of candle #3 with
  - SL at high of candle #1 (use ATR)
  - Target at 1:2, 1:3 (configurable)


### Exit Approach 1

Exit when
- Following HOLD/NURTURE criteria satisfies
  - (Do not close for the 1st n candles - make it configurable (n=3 by default) - during this exit only upon SL/Target)
- Candle closes above the previous candle high
- A candle touches the lower band

### Exit Approach 1

Exit when
- Following HOLD/NURTURE criteria satisfies
  - (Do not close for the 1st n candles - make it configurable (n=3 by default) - during this exit only upon SL/Target)
- Candle closes above the previous candle high
- DO NOT EXIT WHEN THE LOWER BAND IS TOUCHED