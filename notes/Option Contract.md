# Terminology

The sense of call and put becomes clearer if one thinks of the writer of these options.

>English often adds a preposition to a verb to alter the meaning of a verb.

See Calls and puts from the perspective of the option writer, along with the corresponding prepositions `away` and `to`.

- a stock getting `called away` from the investor (for selling).
- a stock being `put to` the investor (for buying).

## CALLed away

When I write calls my broker will report, "My stock has been called away."

This is a shorthand for "Your (underlying) stock (on which the call was written) has been called away (and you have sold at the option's strike price to the option buyer)." (He could also say, "The call has been exercised" and hope that the option writer is well versed in the mechanics of options.)

Here, the preposition _away_ tells me the direction of the stock's motion: It is _away_ from me, the call writer.

> "Called away" is the term used to describe the elimination of a contract due to the obligation of delivery. This occurs if an option is exercised, if a redeemable bond is called before maturity or if a short position held in a security requires delivery. [...](http://www.investopedia.com/terms/c/calledaway.asp)

##### Example

Imagine an investor who owns 100 shares of INFY and has written a call with a strike of ₹1600. And suppose that INFY is at ₹1700 on expiration day. What happens?

INFY gets `called away` from the investor at ₹1600.

> As a call buyer you have the `choice (an option)` to `call` the `strike price` you want to buy an asset for.

## PUT to

When I write puts my broker will report, "The stock has been put to you."

This is shorthand for "The put buyer has exercised his right to sell the underlying stock to you, the put writer, at the option's strike price."

Here, the preposition _to_ tells you the direction of the stock's motion: It is _to_ me, the put writer.

##### Example

Imagine an investor who has written a cash-covered put on stock INFY with a strike of ₹1600. And let's suppose that ABC falls to ₹1500.

INFY will be `put to` the investor at ₹1600.

> As put buyer you have the `choice` to `put` your `asset for sale` at the `strike price` you want.

# Definitions

## Call Option

A call option gives the holder of the option the right to buy an asset by a certain date for a certain price.

## Put Option
A put option gives the holder the right to sell an asset by a certain date for a certain price.

# Strategies

### Buy Low Sell High

| If your view is   | but definitely NOT | then to profit | how?       | when?     | with     |
|-------------------|--------------------|----------------|------------|-----------|----------|
| bullish today     | in future          | buy            | @ discount | today     | Short PE |
| bullish in future | today              | buy            | @ discount | in future | Long CE  |
| bearish today     | in future          | sell           | high       | today     | Short CE |
| bearish in future | today              | sell           | high       | in future | Long PE  |

Buying options is like buying an insurance and an option seller/writer is like an Insurance Broker.

## Long Call

It allows the call owner to buy shares at a discount on a future date (i.e. expiration) if it has intrinsic value at expiration i.e. the spot price is above the strike price by a good amount (that difference is the discount).

> Buying at a discount in future.

## Short Call

Selling Call @ OTM Strike is like Shorting shares at a higher price than the market was initially offering.

> Selling at a higher price today.

##### Example

- ABC is trading at ₹100 today i.e. on 23-July.
- Your view on ABC is not bullish in the near future i.e. till 29-July expiry.
- As per your analysis ABC will trade sideways, trend down, or may slightly go up but not substantially to rally beyond ₹120.
- You think ₹120 level can act as a strong resistance where sellers would take charge.
- If your analysis is correct then you can benefit from this situtation by `selling a Call @ OTM strike`.
- When you short `120CE 7/29 (6d)` at ₹5 you are obligated to sell ABC @ ₹120 on 29-July if it gains intrinsic value.
- But, in today's context, when ABC is trading at ₹100 you are getting to sell ABC at a higher price of ₹120 and also get to collect ₹5 premium just by selling the Call. And you don't even need to own ABC to short it.
- By selling an OTM Call option you make money when market trades sideways, goes down, or even goes up but stays below ₹120. You only loose when market rallies beyond ₹120 by 29-July. Your Probability of success is high.

## Long Put

It allows the put owner to sell his shares at a higher price than the market on a future date (expiration) if it has intrinsic value at expiration. Buying a Put is a good insurance against a potential downtrend.

> Selling at a higher price in future.

## Short Put

Selling Put @ OTM Strike is like owning shares at a lower price than what the stock was trading initially. In this case you would own shares at its strike price instead of the old market price and still keep the premium you collected for selling the put in the first place.

> Buying at a discount today.

##### Example

- ABC is trading at ₹100 today i.e. on 23-July.
- Your view on ABC is not bearish in the near future i.e. till 29-July expiry.
- As per your anlaysis ABC will trade sideways, trend up, or may slightly go down but not substantially to crash below ₹80.
- You think ₹80 level can act as a strong support where buyers would jump in to prevent further drop in price.
- If your analysis is correct then you can benefit from this situtation by `selling a Put @ OTM strike`.
- When you short `80PE 7/29 (6d)` at ₹7 you are obligated to buy ABC @ ₹80 on 29-July if it gains intrinsic value.
- But, in today's context, when ABC is trading at ₹100 you are getting to buy ABC at a far lower price of ₹80 and also get to collect ₹7 premium just by selling the Put.
- By selling an OTM Put option you make money when market trades sideways, goes up, or even goes down but stays above ₹80. You only loose when market trends below ₹80 by 29-July. Your Probability of success is high.

# Moneyness

## ITM

## ATM

## OTM

##### Tip

If you are an option buyer and you are holding your position till expiry then you must ensure that you exit at ITM to avoid facing huge losses.

# Why Option Contract?
https://www.youtube.com/watch?v=D0I-VXz3FcI

You can make money by doing the following:

- Option Buying
	- Do not do option buying if you have 5 Lakh or less.
- Option Selling
	- Do this if you are beginner or have less than 5 lakhs.
- Option Hedging
	- Do this if you have less than 5 lakhs.

# Tips
[...](https://tastytradenetwork.squarespace.com/tt/blog/-tastytrade-trading-commandments)

- You must trade ITM options on the day of expiry. In Long positions, one red candle can wipe out 60% capital with just one red candle. [...](https://youtu.be/2fPVlSa5wYE?t=2244)

- Trading is about emotional intelligence rather than logic intelligence.

- Beginners should not trade Options. Stick to futures. With futures S.L. managment is easier.

- You can start trading options once you become an advanced trader and can comfortably watch winning and losing trades without becoming too fearful or excited.

# Stop Loss

- In options trading S.L. is to be put on the premium chart.
- Premium chart is different for every strike price so the actual Stop Loss can only be tracked on Spot/Index chart.
- You must consider the logical Stop Loss on the Index/Spot Chart as the real Stop Loss and the physical Stop Loss on the premium chart is to be tracked and adjusted in tandem with the logical stop loss on the index/spot chart.
- While tracking S.L. level on Spot/Index charts, the price should not just touch S.L, the candle should also get closed on or beyond that S.L. level. [...](https://youtu.be/2fPVlSa5wYE?t=2871)
- Note that its very difficult to put S.L. accurately on the Premium Chart due to the dynamic interplay of greeks in the calculation. If you are an option buyer then there is a `Theta Decay` on the premium chart where as price action is normal on the Sport/Index chart.
- Again, you should hold & respect the logical `Stop Loss` on the index chart while tracking the actual Stop Loss on the premium chart by shifting it gradually in tandem approximation with index/spot chart. [...](https://youtu.be/dQ2jM5ATqIg?t=2000)
- Once you become emotionally stable you must decide that as soon as the price touches the S.L and closes there on the Spot/Index chart, you will exit your position on the Premium chart.
- This is the reason you should only risk 8% to 10% of your entire `Trading Account Capital` into Options Trading.
- Place S.L. on the Spot/Index chart, track it and as soon as price comes at that level and closes on/beyond it, you exit the position.
- If you still want to put S.L. put it far away.

![[Stop Loss#Quit moving stops too soon]]

# Rules

## Expiry Day Rules

Volatility is very high on expiry days and premium value vanishes very fast. Even with one S.L. hit it takes away over 50% of your position.

- Only enter the highest probability trade. Plan such trades well in advance and only then enter.
- If you face loss, do not enter another new trade on the expiry day. If your S.L. is hit then close your trade. On other days you can close your trade after 2nd S.L.
- Do not enter-exit-enter-exit the trade back and forth. Enter just once with full conviction. Do not exit and enter again. You can do this on other days.

## Hedging Rules (Unverified!)

To reduce the initial margin requirement cover your option sell position by going Long on the reverse option contract at OTM strike price.

For covering the Short option contract with a Long contract pick a strike price which has premium around 50% of the premium for ShortING the main option contract. [...](https://youtu.be/M3Bz_IZpN6Q?t=750)

> Do not buy a `far OTM` options for hedging. [...](https://youtu.be/M3Bz_IZpN6Q?t=722)

Example:

You have a bearish view of NIFTY and would like to go Short a CALL option. To minimize initial margin requirement you will create a cover by going Long on the CALL at an OTM strike price which is not too far and is 50% of the premium required for Shorting the CALL.

`Market View:` Bearish. You think nifty will not go above 15000
`Strategy:` Go `Short` on `15,000 CE` @ `269` premium
`Initial Margin:` 1,35,000 INR

Create cover to reduce the Initial Margin requirement:

Calculate 50% of the premium to be paid for Shorting 15000 CE
=> 134.5 INR

Open `Option Chain` and find an `OTM` `CALL` strike price around 134.5 INR and go `Long` on that.