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
- Our max gain (profit) is the width of the spread, minus the amount we pay to buy the spread.
	- For more profit widen the spread width, pay more for the spread and risk more.
- Our max loss (risk) is the amount we pay to buy the spread.
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
`Max Loss` => `Incurred Spread Cost` => $343
`Max Gain` => (`Spread Width` x `Lot Size`) - `Incurred Spread Cost`
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
- Our max gain (profit) is what we sell the spread for.
- Our max loss (risk) is the width of the spread, minus the credit we receive for selling it.

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

`Max Loss` => (`Spread Width` x `Lot Size`) - `Received Spread Cost`
 		=> (10 x 100) - $345 => $655
`Max Gain` => `Received Spread Cost` => $345

### Put Spread
```
Use this if the market is far away from the mean.
Many positoins will close fast if the market is strongly trending (either up/down).
```

# Deciding Debit vs Credit Spread

Say your view on `IWM` is bullish and its `IV Percentile` is 67%.

#### Which spread you would plan? Debit spread or Credit spread?

- When `IV Percentile` is over 50% then we want to `sell` so that takes out the choice of Buying Calls or Buying Call Spreads; that leaves you with Selling `Put Spread`.

- Since you are selling you will choose something with NO `Intrinsic Value`

#### What kind of Credit you would expect to earn?
[...](https://youtu.be/LNtjyfgZWcA?t=755)

Lets say we want better than 50-50 chance of success (i.e. 50% POS). What kind of Credit we would want to receive? Over $0.50 or under $0.5?
- Its under $0.50.
	- You want to risk more since its a $1 wide spread.
	- You want to risk more moeny than you can make so that you have a higher POS.

[...](https://youtu.be/LNtjyfgZWcA?t=799)
![[Pasted image 20210727132719.png]]


## Tips

- When you are selling you DO NOT WANT any `Intrinsic Value` whereas when you are buying you DO WANT an Intrinsic Value today.

- When you are selling you DO WANT `IV Percentile` to be over 50% so that you can receive more credit or be able to go further away from the money.

# Deciding Spread Width
[...](https://www.youtube.com/watch?v=KPlhiq_j76Q)

| Narrow Spreads       | Wider Spreads       |
|----------------------|---------------------|
| Greekless            | Less Binary         |
| Higher % of max loss | Lower % of Max Loss |
| Worse Breakeven      | Better Breakeven    |
| Slow Moving          | Faster Moving       |


# Lingo

## Debit Spread Lingo

```
Debit Spread with $1 Wide Strikes

Debit $0.5 => 50% POS
Debit $0.7 => 70% POS
Debit $0.3 => 30% POS
```

- How much you can loose if you are paying $0.5?
	- $0.5
- How much you can loose if its a 1$ wide strike and it can go upto $100 when I am paying $0.5 (i.e. $50)
	- $50 (i.e $0.5 x 100 as 1 lot = 100 units)
- How much you can loose if you are paying $0.7 for a $1 wide spread?
	- $0.7

With `Debit $0.7 => 70% POS` you are risking $0.7 to make $0.3 so you better have a better than 50-50 chance of winning or you rather buy a `Debit $0.5 => 50% POS`. If both have the same chance of winning then you might aswell pay  less (i.e. $0.5).

So if you pay $0.7 for a $1 wide Debit Spread that can only go to a $1 (i.e. 100 considering the lot size) then your probability is 70%.

### Warning!

Many new traders choose to pay less for a wider spread. Say they will pay $03 for $1 wide Debit Spread.

- How much you can loose if you are paying $0.3 for a $1 wide spread?
	- $0.3 (i.e. $30)
- How much you can make?
	- $0.7 (i.e. $70)
- Now you are risking less to make more, so what is the catch here?
	- Your probability of success is going to be lower!

- What does Probability of Success (POS) really mean?
	- It means the spread that you bought for $0.50 is worth atleast $0.51 at expiration.
	- It means the spread that you bought for $0.70 is worth atleast $0.71 at expiration.

## Credit Spread Lingo

```
Credit Spread with $1 Wide Strikes

Credit $0.5 => 50% POS
Credit $0.7 => 30% POS
Credit $0.3 => 70% POS
```

If you sell a $1 wide spread for $0.70...
- What is your risk?
	- $0.3 (i.e. $30)
- Since you are risking less for making more What will be your PoS?
	- 30% <-- its already stated!

A lot many times new traders think they are risking less money but essentially they are risking more. If you sell something for $0.7 and it can only go to a $1 max then your probability of success is 30%. Meaning, you are going to be able to buy it back at expiration for less than $0.70. But if you sell comething for $0.30 your max gain is $0.30 against a max loss of $0.70; you are definitely risking more money coz you are losing $0.70 and making only $0.30, you have to have a better than 50% probability of success otherwise there is no reason to make that trade. Therefore with 70% PoS you are selling it for that much less (i.e. $0.30); you are selling something that has no intrinsic value.

# Q&A
[...](https://www.youtube.com/watch?v=LNtjyfgZWcA)

`Question:` @tastytrade @ [6:08](https://www.youtube.com/watch?v=LNtjyfgZWcA&t=368s) says if I sell a $1 width credit spread for $0.70(max gain), so the risk (max loss) is $0.30; this makes sense as max gain is what you sell the credit spread for and max loss is the spreads width - net premium received. Then at [6:30](https://www.youtube.com/watch?v=LNtjyfgZWcA&t=390s) he says if I sell a spread at $70 (AKA $0.70 contract) I can only make $0.30? Does he mean if I BUY something (AKA buy a debit spread) for $0.70 and I can only make $0.30? If you sell a 1 dollar width spread for $0.70 your max gain isn't 0.30, its 0.70


`Question:` For selling a Vertical Put you used a credit of $0.27 for a $1 spread. And then risk $0.73 to make $0.27. As you say these gives you 73% prob of success. The ratio of risk/reward = 2.7 to 1 or risking $3 to make $1. So if I wanted to sell 5 contracts, my risk is $385 to make $135. My question is this: why would one want to risk $3 to $1? Why no use a R/R ratio around 1 to 1?
`Answer:` When you are risking 1 to make 1, you will only have a probability of success of about 50%. Instead, we prefer to risk 3 to make 1 and have a 75% probability of success. We use these probabilities to increase our win rate and look to manage our winning trades quickly so that we can avoid losses of any kind.
- `Question:` I don't understand the probability thing: surely the likelihood of a successful trade depends on my choosing an underlying that is moving the right way - not on the prices I pay/receive for the options contracts? Can't get my head around that one...
- `Answer:` In general, stocks have a 50% chance of going up or down in any given day, so it is very difficult to accurately predict a stock’s direction over a large number of occurrences. The probabilities stem from the option prices, which are determined by buyers and sellers in a market. The lower the probability, the lower the option’s price will be. Conversely, the higher the probability, the higher the option’s price will be. However, we can’t only look at an option’s absolute price and compare it to other prices, because all stocks have different expected movement (implied volatility) and different prices (high-priced stocks vs. low-priced stocks). For example, a call worth $10 in PCLN doesn’t have a higher probability of expiring in-the-money than a call worth $1 in YHOO. This is why we look at the probabilities of each respective option as opposed to the actual price.

`Question:` When you short a vertical spread and let's say that it expires in 30 days, if you are already in day 5 (25 days left) and it is in red numbers and it keeps losing value as the days pass by, you are losing money but the POP still shows that you are most likely to win on this trade, what should you do? Take the loss and long the vertical spread before it keeps going into ever greater losses or do you trust the POP that it'll eventually turn around and start giving you good outcomes?
`Answer:` Specifically with defined risk credit spreads, we know that our max loss is defined from the beginning, so if the trade goes against us right away and we still have a lot of time left, we typically hold onto it since we can only lose so much more, and we have everything to gain back over the course of the remaining cycle. Totally up to you, but from a risk:reward perspective, it may make sense to hold defined risk trades that are underwater rather than close them, since our risk is defined up front and we may already be close to that max loss value that won't change.

`Question:` If we have a 30% chance of $70 profit and a 70% chance of a $30 loss, then after fee's, we lose over time. Can you explain the MATHS behind how an options trader can profit from vertical spreads please? is it an expectation of IV reduction or something else?
`Answer:` We will be profitable due to a number of factors. First is that Implied Volatility is more often overstated. This means that our win rate will be higher than the 70% that the market is pricing in. Additionally, by managing our winners, we are able to increase our win rate even higher. This will put our win rate above 90% and thus make the strategy profitable.