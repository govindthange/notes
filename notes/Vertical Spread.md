[...](https://www.youtube.com/watch?v=h5Z_Yh3riwg) [...](https://www.youtube.com/watch?v=HaoM4nqxYhU)

Buying Vertical Spread = Debit Spread

Selling Vertical Spread = Credit Spread

Bull Put Spread = Short Put Spread = Put Credit Spread

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

# Case Studies

## Weekly earning 8% with Put Credit Spread
[...](https://www.youtube.com/watch?v=YfYjNovwph8)

### Transcript

- If I think VIX is going to pop during the week then I wont use all the collateral in my account.
- Leave 20% on the table and exit. Do not risk bombing your account when VIX is going to go high.
- Track position by doing following calculations:
	- Where the stock has gone i.e. how much it has risen?
	- What precent of the expected move is still available to the stock? Do TA to know this. If the stock only has 10% of the move left then I am not going to do a credit spread on that because of lot of risk.
- I trade around .10 to .12 Delta. If it rises to .20 - 0.25 then I know my spread is gaining value (resulting in loss) then I cap that loss really quick.
- When your Deltas are around 0.70 then there is a 70% of chance position going ITM. If you are in the middle of the week then get out of your position and clear your mind and get ready for the next week.
- Worst part of trading spreads is the facts that Futures are going to dictate what happens to the ETFs in the after hours. If you see a massive gains in the futures then you know that you are gain a lot of profits on the the open. If you see a massive drop then you are going to refer to CNBC to see where ETF is going to open.

Executing Put Credit Spread [...](https://youtu.be/YfYjNovwph8?t=1456)

- When you trade Put Credit Spread you have to think like you are the bank.
- When you get the collateral, its like a loan given to you. And you are going to get a small percent back.

- Right now `SPY` is trading at $326.54
- Pick a `-0.12 Delta` strike which is `SPY 300PE, 6 NOV 20`
	- The entry shows 86.51% Probability of OTM.
	- The entry shows $1.5 as `mark` (=Premium)
- Now you have to think that __SPY is not going to hit $300__ by the end of next week i.e. by Friday, 6 Nov 20. $300 is the support and SPY will stay above it.
- You get $26 runway with $326 spot and $300 strike.
- Now right click, Select `Sell` -> `Vertical`
- Do not create a wide spread. Keep `Spread Width` in between 5 to 8. [...](https://youtu.be/YfYjNovwph8?t=3539)
	- If you make it a $20 wide by SHORTing `SPY 315PE (6 NOV 20)` @ $3.735 mark with 70.52% Prob. OTM.
	- You will collecting $2.23 per spread
	- That is $2,230 Max Gain.
	- But you will be putting up $12,783 for that spread. Which is your `Buying Power Effect` or `Max Loss`. This is a too much leverage for a position which will give you too little.
	- If your Delta rises from 0.75 to 0.85, you will get hurt big time.
- Do not make your trades as valuable as they can be but do everything to roll the probabilities in your favor. Try to diversify your positoin by taking other positions instead of adding more to this same position.
- The goal of a trader should be capital preservation.
- Hold with conviction.
	- Hold on to your position till expiration or atleast till friday to collect as much as you can because you are at such a high probability of OTM.
	- Sometimes you take these spreads with 90% Prob. OTM and these positions will be at 99% Prob. OTM in next few days.
	- You better hold on to such positions till expiration without caring what happens at after hours.
	- Say in our below example, the 99% Prob. OTM is at 225 strike. If SPY index drops from 326.54 to $225 then we have much bigger problem then market.

SHORT `SPY 300PE (6 NOV 20)` @ $1.5 mark (Receivable) with 86.51% Prob. OTM
LONG `SPY SPY 295PE, 6 NOV 20` @ $1.15 mark (Payable)
`Spread Width` => 300 - 295 => 5
`Lot Size` = 100
`Quantity` = 10

`Received Credit`
=> `Received $1.5` - `Paid $1.15`
=> 1.5 - 1.15
=> $0.35

`Total Received Credit`
=> `Received Credit` x `Quantity` x `Lot Size`
=> $0.35 x 10 x 1000
=> $350

`Max Gain` = `Total Received Credit`

`Max Loss`
=> (`Spread Width` x `Quantity` x `Lot Size`
=> 5 x 10 x 100
=> 5000

`Total Collateral` = Max Loss = $5000


`Break Even Stock Prices`
=> `SPY 300PE (6 NOV 20)` Strike - `Received Credit`
=> 300 - $0.35
=> $299.65

`Cost of Trade`
=> `Total Received Credit` - `Commissions` - `Fees`
=> $350.00 - $13.00 - $0.33
=> $336.67

`Buying Power Effect`
=> `Total Collateral` - `Cost of Trade`
=> $5,000 - $336.67
=> $4,663.00

`Resulting Buying Power for Stock` = $5,098.67
`Resulting Buying Power for Optoins` = $2,965.89

### Tips

- Do not create Spreads using ATM strikes. That will give you a 50% Probability of OTM.
- Bid Size, Ask Size
	- Look at the volume of Bid-Ask spread indicating a high acceptance. Look for the bracket of acceptance i.e. there should be massive volume around the strikes your position is. If it is low it will be a problem. Trade in a highly liquid instruments that don't have low liquidity or high bid/ask spread.
- Delta
	- If the given option were to become ITM and the underlying stock goes up by 1$ how much will the option increase?
	- You can think this in terms of `ITM Probability` calculation i.e. if your Delta = 0.20 then read it as there is 20% chance of option becoming ITM. If Delta rises to 0.8 then there is 80% chance you will be ITM.
- Probability of OTM
	- Its the derivative of `Black-Scholes-Mertin Option Pricing Model`
- Mark
	- Mid point of Bid and Ask quote
	- The average price of that spread leg will get filled.
		- Say Mark for  `SPY 301PE (6 NOV 20)` is $1.605 and Mark for  `SPY 300PE (6 NOV 20)` is $1.505
		- Then that means you will get filled for that spread on an average around 1.105
- % Change and Net Change
	- You need to see it in (-)ve when trading spreads. It should fall as days pass by.
	- If you see this in (+)ve like say 6.. then it means your deltas are moving up into the money (ITM).
	- Basically the options you have chosen should be going down and not up.

### Ideal Put Credit Spread Setup

You enter position based off of on probabilities alone. like if there is a 92% chance of win then just get into the position.

You don't need FA or TA just 2 numbers.

#### 1. Open, Close and Range of the last candle in a Weekly Chart

- Open a 3 year weekly chart.
- See OHLC and Range of the last weekly candle.
- Do this every week, before going on to the next week.
- Say the last weekly candle close was on 26th October (i.e. last Friday)
- Then for the next week, you will note down the difference between OPEN & CLOSE and Also the RANGE (i.e. low - high).
- Say the range was $20.38.
- Then for the next week's Put Credit Spread, you need to plan your position with $20.38 strike difference lower from the current price. For example if the currently SPY is at $326.54 and the last week's candle range is of $20.38 then you need to position strike at around $300 (326.54 - 20.38 = 306.16)
- Essentially you want to be outside of a 1 Standard Deviation move to the downside.
- By doing this you want to put yourself at a % probability that you are outside of a 1 Standard Deviation move of the stock.

I only use Range of the last weekly candle and do not track S/R levels on weekly charts. To me it makes little sense as its subjective.

#### 2. [[Option Greeks#Implied Volatility VIX]]
[...](https://youtu.be/YfYjNovwph8?t=2973)

On the Monday morning check the IV(VIX) of the instrument you want to take position in.

Lets say IV of `SPY` is 50.11% (±16.54)

> `TODO:` check whether the ±16.54 is a Vega value.

Then on monday do as follows:

`Vega` => `Opening Price of SPY` x  `Implied Volatility of SPY on Monday` x √(`Days until Expiration` ÷ 365)
=> 326.54 x 50.11% x √(5÷360)
≈ ±16.543

This implies:
- SPY will potentially move ±16.54, to the up/down side, 68.2% of the times.
- ±16.543 is only a half σ move of the SPY.
- A 1 σ move of the SYP is going to be around 86%.
- A 1.5 σ Standard Deviation is around 89.47% at $295 Strike for SPY. This is what I prefer!

### Conclusion

Once you start trading Credit Spreads you would open yourself up to a whole new world of options trading; you would know how the other option strategies work, you would understand the Deltas and Thetas, then you can start to look at how buying along options is a net losing strategy but can be used to hedge against the limited profitability of a credit spread.

So its recommended that you start with the credit spread, it will be really lucrative. Its safest when you use 90% OTM Prob but it gets extremely dangerous if you trade it really tight.

This strategy gives a high probability credit spread because:

- You are outside of 1.5 σ move.
- You are outside of the expected move range.
- You are outside of the candle range of the last week.

With SPY currently at $326.54, the strike price of $295 gives you a really long runway to know whats going to happen to SPY over the course of the trade.

Beginners can start with 2 σ, then graduate to 1.75 σ and finally to 1.5 σ.

Trading spreas will make you money over time you just have to cap your losses quick and limit it to 25% or below because if you take a full 100% loss on a spread then even if you have 90% probability of winning trades, the profits from 90 out of 100 trades would be lesser than losses from remaining 10 trades.

Spread has an excellent win rate but has a very poor risk to reward ratio if you don't know how to control it fast.

The biggest thing about credit spread is:
- Knowing how to take your high probability chances.
- And knowing when to exit.

### Risk Management
[...](https://youtu.be/YfYjNovwph8?t=4380)

#### Delta

My risk management is based off of Deltas.

I exit the trade if the spread value increases by 15% to 20%.

#### Earning Seasons
[...](https://youtu.be/YfYjNovwph8?t=4520)

Either avoid Earning Seasons or

Or do following calculations using MMM value:

I take the `IV value (VIX)` (±16.543 as calculated above) and add it to `Market Maker Move (MMM)` value (±12.3) to it. So you will add ±28.853 to spot price to get the desired strike price.

### Going Next Level
[...](https://youtu.be/YfYjNovwph8?t=4652)

Do this if you have capital and you are willing to take risk to maximize  profits.

If you think market has become directional in its move.

#### Going LONG Delta
i.e. buying options and opening yourself to Delta decay against you.


##### Reverse Jade Lizard

Take a Put Credit Spread running at 90% OTM probability.
Gain that money in credit.
Put up some of that credit to long ATM CALL above the Put Credit Spread (i.e. outside of the Put Credit Spread) to collect any money that goes to the upside. Jack the number of contracts.

One problem with the Put Credit Spread is that if the stock were to shoot up really far away, you are only going to gain the credit between the two options that you have sold.

Reverse Jade Lizard is a great way to gain extra exposure to the upside with the Put Credit Spread.

### My Schedule
[...](https://youtu.be/YfYjNovwph8?t=4829)

In simple words my style is a bracket trading with credit spread underneath the brackets. My positoin on monday is a half Iron Condor which I complete later depending on the market condition.

So essentially it is an Iron Condor which is more dynamic, sperated by time, sometimes skewed to the upside sometimes skewed to the downside depending on what happens to the stock based on what happens on Monday when I am opening my position.

I take the Call Credit Spread if the Put Credit Spread on an average are about 60% profit on the thursday (USA) morning. If the Put Credit Spread is losing then don't take the calls coz then you are just going to put yourself too tight as your spread/option-chain becomes constricted.

| Schedule           | USA               | India                |
|--------------------|-------------------|----------------------|
| Put Credit Spread  | Monday - Friday   | Friday - Thursday    |
| Call Credit Spread | Thursday - Friday | Wednesday - Thursday |

You enter Call Credit Spread when you are already in the Put Credit Spread, the stock is moving up and down.

When you see a put credit spread number below the ±18.6 level (IV/Vega), this number is going to change rapidly. By the time you reach Thursday (USA) this ±18.6 could become ±6, so when you make an Iron Condor you are opening yourself up to not knowing this...

You might know how much risk is there to the downside but may you have no idea what your risk to the upside coz that ±18.6 could increase to ±20 etc..
Iron condor on monday will get you more credit but doing this with a delay is a safer bet.

The biggest thing about the iron condor though is that on the call credit side I have no Buying Power Reduction. It just adds more risk to your portfolio but its only for a short amount of time.

Continued [...](https://youtu.be/YfYjNovwph8?t=4910)

### Q&A
[...](https://www.youtube.com/watch?v=C7Xs8j1pXIk&list=PLbEa4ew-NWP_0YAc-CY99KN8awyZbqMiN&index=30)

`Logan Lajin:` When not to trade this setup?

`Mazurati:` 2 things:
- VIX over 25: Trading with VIX above 25 is a dead deal for me because you trade spreads when its non directional. With Vix above 25 makes it a directional bet and it takes away runway from you. So with 25 VIX I usually don't trade that week or trade with an extremly small amount.
- Credit to Collateral: If you have to put up $2000 to make $10 then I don't take that deal. Putting $2000 to make $100 is fine but nothing lesser than that ratio. Then you can scale that up.

`Logan Lajin:` Once you are already in the spread trade and you are observing the vix and it pops later in the week (say you are on wednesday, and VIX pops 8 bucks overnight but everything else looks smooth), so what is your vix target price? Is there any certain number on the vix at that point when we are like halfway through the week? [...](https://youtu.be/C7Xs8j1pXIk?list=PLbEa4ew-NWP_0YAc-CY99KN8awyZbqMiN&t=128)

`Mazurati:` Once we are already half way into the week then...
- I'll look at the mark of the index that we are trading. If I sold spread at mark 174. If it is at 181. The runway is of 7... if the runway is greater than 5.. i usually find it safe.. Anything less than 5 (like 2 or 3) then its risky.
- I look at the delta and make adjustments to spreads around the delta of 0.25.
- I focus on the actual mark of the underlying and compare it to where I took the spread at, so thats the runway.

`Logan Lajin:` When doing spreads why do you choose to do 5 strikes or more wide? Is it to protect the collateral if the short leg goes ITM?

`Mazurati:` The width of the spread is completly up to investor's discretion based off of how much buying power you have in your account. To me 5 strike wide is the sweet spot for credit to collateral ratio for my account. This is my way of scaling up the strategy by taking 40 contracts of usually a $2000 position.

`Logan Lajin:` When monitoring your runway when do you start to worry or wait for the short leg to go ITM or do you close your position only when it goes ITM.

`Mazurati:` I usually close my positoin when I am a 1 away i.e. my runway is less than 1 or I'm ITM or the premiums on the positoin are higher about 25% so the spreads got increased in price by 25% thats when I usually do a manual close. Note that having to close the position manually is not a good situation you want to be in.

`Logan Lajin:` When doing spread do you leave any money on the sideline in case one goes against you? Is there a number?

`Mazurati:` I usually go 95% into the buying power. I don't go into Calls until I can diversify the number of positions that I'm in. Taking calls on Thrusday is the most risky because the stock can also just shoot up randomly.

`Audience:` Which technical indicators to use?

`Mazurati:` Best thing about spreads is that you do not need indicators.
- Its a non directional play. [...](https://youtu.be/C7Xs8j1pXIk?list=PLbEa4ew-NWP_0YAc-CY99KN8awyZbqMiN&t=637)
- When you are taking spreads, you are only talking probabilities.
- You just need to know VIX (+/- Vega). i.e. if `Spot` = 180.27, `IV (VIX)` = 64.41% then `Vega` => 180.27 x 64.41% x √(7÷360) => ±14.485 (approx)


`Audience:` What is your exit strategy when your spread is in the danger zone? When would you close it and what could that cost you?

`Mazurati:` 3 things:
- Runway less than 1: You are in a danger zone when your runway is less than 1. In that case you just want to get your position off the table and book a loss. But if you have other positions open that can counteract that loss and you could still potentially finish the week in green then you can take that chance.
- Delta to be between 0.9 to 0.12. I exit the position if the delta rises to 0.25.
- Also look at the bid/ask spread. If the difference between bid and ask is rising that means premiums are rising too. You exit the position.
- I sometimes set trigger orders like so:
	- `Take Profit` = -95% of the shorted premium
	- `Stop Loss` = +125% of the shorted premium

`Logan Lajin:` Why you trade weekly versus longer expiration?

`Mazurati:`  I think with weekly I have a higher probability of knowing that TQQQ or SPY is not going to hit a certain strike next week. I am exploring Calendar Spreads for 56 days expiry.

`Audience:` What key variables you track?

`Mazurati:` Open, Close and the range of the week to track the expected move of the following week.

https://www.youtube.com/playlist?list=PLbEa4ew-NWP_0YAc-CY99KN8awyZbqMiN

### Demo
[...](https://youtu.be/C7Xs8j1pXIk?list=PLbEa4ew-NWP_0YAc-CY99KN8awyZbqMiN&t=1653)

# Wheel Strategy

Selling cash secured puts and then if you get assigned you sell covered calls against those shares.
