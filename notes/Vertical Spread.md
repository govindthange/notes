[...](https://www.youtube.com/watch?v=h5Z_Yh3riwg) [...](https://www.youtube.com/watch?v=HaoM4nqxYhU)

`Definition:`
- You buy and sell a `CE` (or `PE`) at different strikes of the same expiry to create a spread.
- The action you take with the `Front Option` (i.e. option that is closest to the spot price) determines the direction of the trade.
- `Width of the Spread` determines the amount of profit you will make of the spread.
	- The difference between the long strike and short strike is the `Spread Width`.
	- No matter how high a given spread goes, the profit can never go beyond `the lot size times the width` of the spread.
	- So wider the width, more profit you make but you also take that much increased risk.
- `Spreads` (i.e. having a vertical component so created) have some interesting benefits compared to just buying or selling a standalone option (aka `Naked Options`). You start to become more precise with your trades like:
	- Defining risks.
	- Defining how much money you want to make out of this trade.

> `Nake Trading` is level 1, `Spread Trading` is level 2.

# Debit Spread
=> Buying a vertical spread.

## Buying Vertical Call Spreads

Our view is bullish!

-  Buying a call spread is a `bullish` trade.
-  Creating a spread `defines the risk` of the trade compared to buying a naked call option.
- The most we make, our profit, is the width of the spread, minus the amount we pay to buy the spread.
	- You can certainly make profit, but then you will have to widen the spread width and be ready to pay more and therefore risk more.
- The most we loose, our risk, is the amount we pay to buy the spread.
- Creating a spread is `cheaper` than just buying a naked call option. Buying call is like a buying a Call opton for discount.
- Unlike in a naked call option max profit in a spread is limited.

The action you take with the `Front Option` (i.e. option that is closest to the spot price) determines the direction of the trade.
- So here the strike price closer to the spot is the CE which we are longing and it means we are bullish and we want price to trend upward.

`Lot Size` = 100
`Buy` a `$175 CE 1/19 (71d)` @ $5.65 (Payable)
`Sell` a `185 CE 1/19 (71d)` @ $2.22 (Receivable)
`Spread Width` => $185 - $175 => $10

`Incurred Spread Cost` => `Lost Size` x (`Paid $5.65` - `Received $2.22`) => $343
`Max Risk` => `Incurred Spread Cost` => $343
`Max Profit` => (`Spread Width` x `Lot Size`) - `Incurred Spread Cost`
 		  => ($10 x 100) - $343 => $657

# Credit Spread
=> Selling a vertical spread.

> Credit Spread opposite of Debit Spread; just flip everything you did.

## Selling Vertical Call Spreads

Our view is bearish!

> Although we are bearish we don't need a big move to the downside. We just need the market to stay below the strike we sold `CE` at (a resistance level) till the expiry.

==This is why we say, you could be wrong but right with the option trading.==


- Selling a call spread is a bearish trade.
- Creating a spread defines the risk of the trade compared to selling a naked call option.
- The most we make, our profit, is what we sell the spread for.
- The most we loose, our risk, is the width of the spread, minus the credit we receive for selling it.

Note that if you sell a naked call, there is an unlimited risk.

The action you take with the `Front Option` (i.e. option that is closest to the spot price) determines the direction of the trade.
- So here the strike price closer to the spot is the CE which we are shorting and it means we are bearish and we want price to stay below this strike price.

`Lot Size` = 100
`Sell` a `$175 CE 1/19 (71d)` @ $5.90 (Receivable)
`Buy` a `185 CE 1/19 (71d)` @ $2.45 (Payable)
`Spread Width` => $185 - $175 => $10

`Received Spread Cost` => `Lost Size` x (`Received $5.90` - `Paid $2.45`) => $345
`Max Risk` => (`Spread Width` x `Lot Size`) - `Received Spread Cost`
 		=> ($10 x 100) - $345 => $655
`Max Profit` => `Received Spread Cost` => $345

### Put Spread

Use this if the market is far away from the mean.
Many positoins will close fast if the market is strongly trending (either up/down).
