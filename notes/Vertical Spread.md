[...](https://www.youtube.com/watch?v=h5Z_Yh3riwg) [...](https://www.youtube.com/watch?v=HaoM4nqxYhU)

`Definition:`
- You buy and sell a `CE` (or `PE`) of the same expiry at different strikes to create a spread.
- The action you take with the `Front Option` (i.e. option that is closest to the spot price) determines the direction of the trade.
- `Width of the Spread` determines the amount of profit you make.
	- The difference between the long strike and short strike is the `Spread Width`.
	- No matter how high a given spread goes, the profit can never go beyond `the lot-size times the spread-width` (i.e. lot-size x spread-width).
	- So wider the width, more profit you make but you also take that much more risk.
- `Spreads` (i.e. having a vertical component so created) have some interesting benefits compared to just buying or selling a standalone option (aka `Naked Options`). You start to become more precise with your trades like:
	- Defining risks.
	- Defining how much money you want to make out of this trade.

> `Nake Trading` is level 1, `Spread Trading` is level 2.

# Debit Spread
=> Buying a vertical spread.

## Long Vertical Call Spreads
=> Our view is bullish!

> We are looking for a larger move but we want to buy this spread at a discount in exchange of limiting the profit and risk.

-  Buying a call spread is a `bullish` trade.
-  Creating a spread `defines the risk` of the trade compared to buying a naked call option.
- The most we make, our profit, is the width of the spread, minus the amount we pay to buy the spread.
	- For more profit widen the spread width, pay more for the spread and risk more.
- The most we loose, our risk, is the amount we pay to buy the spread.
- Creating a spread is `cheaper` than just buying a naked call option. Buying call is like a buying a Call opton for discount.
- Unlike in a naked call option max profit in a spread is limited.

The action you take with the `Front Option` (i.e. option that is closest to the spot price) determines the direction of the trade.
- So here the strike price closer to the spot is the CE which we are longing and it means we are bullish and we want price to trend upward.

### Example

#### Spread

LONG `175CE 1/19 (71d)` @ $5.65 (Payable)
SHORT `185CE 1/19 (71d)` @ $2.22 (Receivable)
`Spread Width` => 185 - 175 => 10
`Incurred Spread Cost` => `Lost Size` x (`Paid $5.65` - `Received $2.22`) => $343

#### P&L

`Spot Price` = 173.33
`Exit Price` = ?

`Lot Size` = 100
`Max Risk` => `Incurred Spread Cost` => $343
`Max Profit` => (`Spread Width` x `Lot Size`) - `Incurred Spread Cost`
 		  => (10 x 100) - $343 => $657

# Credit Spread
=> Selling a vertical spread.

When you sell a spread, you receive credit.

> A `Credit Spread` opposite of a `Debit Spread`; just flip everything you did.

## Short Vertical Call Spreads

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

### Example

#### Spread

SHORT `175CE 1/19 (71d)` @ $5.90 (Receivable)
LONG `185CE 1/19 (71d)` @ $2.45 (Payable)
`Spread Width` => 185 - 175 => 10

`Lot Size` = 100
`Received Spread Cost` => `Lost Size` x (`Received $5.90` - `Paid $2.45`) => $345

#### P&L

`Spot Price` = 173.33
`Exit Price` = ?

`Max Risk` => (`Spread Width` x `Lot Size`) - `Received Spread Cost`
 		=> (10 x 100) - $345 => $655
`Max Profit` => `Received Spread Cost` => $345

### Put Spread

Use this if the market is far away from the mean.
Many positoins will close fast if the market is strongly trending (either up/down).
