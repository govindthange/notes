[...](https://www.youtube.com/watch?v=BquDGE9KxZQ)

Karen, an Options Trader, makes $105MM profit in the NDX, SPX & RUT.

# Karen's favorite products

Karen started of with stocks and used to manage 30 positions at a time but later she reduced to 10. She faced lot of problem with stocks during Earnings Months and gave up trading stocks and stuck to Indices ever since.

She only trades in indices like S&P500, Russel2000 (RUT) as they are highly liquid and importantly not affected by [[Market Calendar#Earning Events]] too much.

Question: Would you consider different product?
Karen: No.

# Karen's trading style

- Karen's approach is very simplistic.
	- she trades with very few underlyings (primarily indices)
	- She is very low-key on the analytics stuff.
	- She has a very low-key approach to the market in general. No over analyzing the market, no outside noise, no news etc.
	- Very little technicals.
- Karen trades very actively. [...](https://youtu.be/BquDGE9KxZQ?t=552)
- As far as trading goes she is mainly a theta trader using time decay as her main strategy.
	- She mainly puts contracts on of next month
	- Closes contracts for profit and put them back on.
	- When the position gets into the current month, she let them expire and she is already out in the next month's contract depending on the volatility.
	- If the volatility is high, they flip them (they call it Churning) i.e. just sell and buy back. Selling and buying back as long as they can pull as much time value out of it as possible and then when that dries up they usually let them expire worthless.

There is a term called Laddering. Which means Nov-12 is 30 days, Dec-12 is 56 days and Jan-13 is 90 days from now. This is Laddering out position. How much time Karen choose for her position you may ask.

Karen looks for the maximum time value such as 56 days to expiration but she wants that to start decaying. Theta generally starts decaying in around 45 days. She tries to get as much time value but she don't like to get way out in the future. So if we are on Oct 27 and Decemer is getting close. We will be trading December 1st of next week but we dont want to get into January yet.

The longer you go out, the more you define your risk. Its little less risky when you go out a little bit further because you can get a little wider.

# Karen's strategy

## [[Short Strangle]]

Karen does use weekly options. They are not big fan of weekly though. If the volatility is low they can consider it.

56 days expiry is her bread and butter. [...](https://youtu.be/BquDGE9KxZQ?t=818)

- We trick our self into thinking that market has fallen.
	- Note that market does not crash up, it crashes down. So we need to protect ourselves on the downside.
	- We say that the market is lower than what it really is.
		- From where the current number is, we pretend that the number has already dropped.
		- Right now the market is at 1450 but we pretend it is at 1370. We make up this fictional 1370.
	- Then we drop it down 12% below that i.e. 1205 (approx). Which generally takes you to an `ITM Probability` of 5%.
	- We will then short 1220PE which has `ITM Probability` of 5%.
	- Then we trade very actively around this December contract (56d for expiry) and turn that 2 or 3 times.

When you sell those puts will you also sell corresponding calls because it does not require any additional capital?
- We will leg into each side. we will sell calls but doing it today will be bad because market was up today.
	- Being contrarian we sell calls on upswing and we sell puts on downswing so that we can get further out; we are trying to widen as much we can. We have bollinger bands on our SPX chart at 2 standard deviations
	- We want to be out from that.
	- The upside is a much greater challenge than the downside. She is not worried about if the market falls down. Handling upside is tough.
	- On the upside, we will probably little closer in and looking more around `ITM Probability` of 10% on the upside. So we will look at 1540CE and we also look at the charts where we find strong resistance level was. We would make sure we get above that resistance level so all that comes into play when we are looking at the upside.

Would you sell equal number of upside and downside?
No, not necessarily. We are liitle softer on the upside. We will sell more on the put side and make more money and be safer and be out further.

### Karen's Short Strange Approach

Karen is little uneven when it comes to the amount of shorts she has on both sides of the market. Her focus is more on the premium collection rather than on the mechanics of being equal on both sides of the market.

Karen: It is driven by the analysis; where we are 10% up from the current position and where we are 12% down from the current position. We watch that. That is compared to our net lick and we just dont want to be pushing up close to that net lick. So that drives us much more than the number of contracts or whether our positions are even or not.

So Karen is managing her buying power reduction as it relates to her net lick more than managing some kind of mechanics around a specific standard deviation move.

### Karen's old strategies which she quit

Karen used to do following strategies but then quit using them:

- [[Iron Condor Spread]]
- [[Vertical Spread#Credit Spread]]
- Naked Strangles

# Karen's risk management

- She scaled her logic big time.
- She commits around 50%. Sometimes 70% - 80% depending on the situtation.
- She never put Stop Losses. She hates it. She wants to manage her account herself, she dont want anything happening automatically.

What does Karen do when a trade goes against her?

- Karen is more all-in but much further out; thats how she justifies it in her mind.
- Staying out with `ITM Probability` of 5% (sometimes 1% Prob. ITM) is her key strategy.
	- Now if `ITM Probability` moves up to 30% then she asks what is the problem here? What is happening to the market? Could this position get into trouble quickly? etc.
	- If Karen is not comfortable leaving the position where it is, she tweaks it. She moves pieces of it. Rolls a part of it up. Lets say its a call then she would roll a part of it up when its tested to the upside and then put on some more puts in a position. She knows where she feels safe. She makesup for the difference.

"Since we are selling premium, once we get the money we are not giving it back" - Karen

## Karen's trading scenario
[...](https://youtu.be/BquDGE9KxZQ?t=1444)

- SPX is at 1454.92
- Karen looks for an OTM strike that has `ITM Probability` of 10%
- Karen shorts the `1540CE DEC 12`
- The trade goes against Karen as market starts to rally up.
- When the `ITM Probability` on `1540CE DEC 12` goes from 15% to 30% then that acts as trigger for Karen to jump in and take control.
- Karen watches the `ITM Probability` as it moves up.
- At this point Karen needs to re-evalute her assumptions and check whether her position needs tweaking either by rolling up the calls or selling more puts.
- If her position gets in trouble, say it bought in $1000 and she is required to spend $2000 to roll it up and get it out of trouble. She needs to get money through premium by rolling up the side which got tested and make up for the difference on the put side i.e. place a few more contracts on the call side "further out" and also sell some puts.
- The adjustment she makes is as follows:
	- either rolling out in time to reduce delta risk.
	- or cover some of that position which costs her some money.
		- To makeup for that she sells more of the other side (in this case Puts) so that theoretically when everything expires you are back into the same spot.
- When the market is moving up like that, the PE that had `ITM Probability` of 5% are now down to 1%. With that Karen can now place more puts on higher side i.e. with 10% Prob. ITM.
- So when it costs Karen to get the call out of trouble she makes up for the difference. Karen just looks at the numbers and adjusts without emotions.

`Tom:` Is there a Delta number, an amount of directional risk where you start to get uncomfortable or is it all tied to that `30% ITM Probability`?
`Karen:` Its all tied into that 30% `ITM Probability`. It just works for us and she don't wish change anything in it. If it ain't broke don't fix it.

### The 5% ITM Probability

This represents 1.64 standard deviations, which encompasses 90% of data points around the mean.

# Karen's Challenges

Going from high-volatility environment to a low-volatility environment and vice-versa is the real challenge. That makes Karen nervous. When that switch takes place and you are loaded up on the downside, and you have one of those days it makes life difficult.

Those are some dangerous ground which are time consuming.

# How Karen scale things?
[...](https://youtu.be/BquDGE9KxZQ?t=2238)

If volatility goes from 25% to 15% then no issues but if all of a sudden Volatility (VIX) goes from 15% to 25% to 40% then as you are laddering out your positions 55 days at what point you are saying we should be all-in at 28% or we should be 20% in? How do you scale?

We don't think it that way. As the money comes in we just increase the number of contracts. We are still playing the same game, we are still in the same position we just increase the number of contracts.

As the money rolls over we just keep doing it.

`Karen:` We pretend as if the market has already dropped [...](https://youtu.be/BquDGE9KxZQ?t=2300)
- We start at a minimum 100 points down.
- If the market falls, the idea is that we've got time to start adjusting our positions, reduce our positions, react to the situation and manage it.
- So basically we go to 10% Probability of ITM to the upside and 5% to the down side.

`Tom:` Generally for trading indices we advice traders to maintain a short premium and a short delta. This means you have some sort of directional protection on you. Karen, you somehow got to this same setup through your own approach. You always short a little delta and short a premium and the assumption is if the volatility expands the velocity of the down move is going to protect her.

- Karen's focus in not in P&L. They don't focus on how much money they are making; it becomes money when the paychecks are written.
- Her focus is on her numbers (Standard Deviation, Probability of ITM etc.)
- She looks at her net lick at the end of the month more than her net risk. Karen focuses more on how much she can make rather than on how much she is risking.
- Karen set around 15% as a target for her position of that 55 day period.

In 2009-2010 Karen migrated from risk-defined spreads to undefined risks.
It made more sense to her to get further out of the money (OTM) and still make the same premium that one can make in iron condors and can get much safer and make the same premium.

> If you define your profitability, you increase your probability of success. -Tastytrade

`Tony:` Are you all in at 56 days? [...](https://youtu.be/BquDGE9KxZQ?t=2825)
`Karen:` 50 to 70% depending on the situtation.

`Tony:` Will you have multiple months on if you're at a comfort levels... like you have Oct. and Dec now or Nov. and Dec?
`Karen:`
- We will have a current month and out month.
- We are in Mid October, so by the time we get on 30th Oct, we would have closed most of our November positions down and brought the realized income back into october.
- So by the time we get on november there is very little exposure there. Whats left is just so worthless we just ignore it. It also takes up our buying power. We like cleaning that current month out and then we get into December.