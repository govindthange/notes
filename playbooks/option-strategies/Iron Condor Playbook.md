[...](https://www.youtube.com/watch?v=4QzubqTgtcc) | [https://www.youtube.com/watch?v=kdGIe6J194A](https://www.youtube.com/watch?v=kdGIe6J194A)

- It is a better to use `Double Diagonal Calendar Spread` instead of `Iron Condor` for weekly options.
- It works better when VIX is between 17 to 25?????

# Step 1. Wait for the setup

- VIX should be low.
	- Below 18.
	- Iron Condors are successful in low VIX because market moves less.

> Iron Condors are never bad as long as your timing is correct. Don't use Iron Condors in monthly when VIX is high. It is generally safe to use in weekly expiry. [...](https://youtu.be/4QzubqTgtcc?t=398)

# Step 2. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

Prefer calculating range using VIX or IV.
- [[Option Greeks#Calculating Expected Move or Range using IV]]
- When VIX is small then it means VIX is low.
- When VIX is low then chances of market moving high is low. Which in turn means high probability of Iron Condor becoming successful.

# Step 3. Cover range
[[Strategy Builder Playbook#Step 2 Cover range]]

# Step 4. Define risk
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=246)

Hedge naked strangle using Iron Condor.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive 10k in credit, then only debit 10k for hedging.
2. Use `breakevens` to pick strikes for hedging.
	- Use the received credit to buy put and call at the breakeven (approx).
	- By buying PE & CE options at the breakeven will reduce the breakeven range.
3. Adjust so that `Vertical Call Spread Width` and `Vertical Put Spread Width` are same.

> In monthly trades, for first 10 days use future spot price for picking strikes. Later towards the end of month you can use normal spot price for picking strikes. [...](https://youtu.be/A-zpeOlgtOY?t=1697)

# Step 5. Deploy strategy

- For weekly Iron Condor, if VIX is high, deploy this strategy on Tuesday @ 3 PM and exit within next 2 days.

## Calculations

Max Profit `or` Initial Credit => (`Difference between call side premiums` + `Difference between put side premiums`)

Max Loss => `Vertical Spread Width` - Credit Received

Put Side Breakeven => `Long Put Strike` - `Initial Credit`

Call Side Breakeven => `Long Call Strike` + `Initial Credit`

# Step 6. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 7. Adjust position

Act when market breaks through an overhead resistance or underlying support.

## Approach 1. Switch to Iron Fly or roll inwards | Weekly Strategy w/ 2 DTE
[...](https://youtu.be/4QzubqTgtcc?t=441)

Assuming a weekly strategy is deployed on Tuesday @ 3 PM w/ 2 DTE.

### Scenario 1. When stock trends up

- When market rallies...
	- Greed increases.
	- When greed increases VIX goes down or remain flat.
		- VIX rises when there is fear.

==Do not roll up put when VIX is high!==

> When VIX is high, rolling up puts does not help because the premium will not drop enough to result in enough gains.

#### Stage 1. Spot price breaches the short call strike
[...](https://youtu.be/4QzubqTgtcc?t=476)

When price is about to breach the short call strike then that means...
- Price has just formed a new underlying support and now moving up.
- The price is going up because their is a buying force coming from the underlying support.

##### Action: Convert to Iron Fly
[...](https://youtu.be/4QzubqTgtcc?t=550)

> Iron Fly (Straddle) loss is less than the Iron Condor (Strangle loss).

1. Wait till spot price is about to breach the short call strike.
2. Shift short put to the short call strike.
	1. Exit from the existing short put.
	2. Sell a new put at short call strike.
3. Slide up the long put by few points.
	1. Exit from the existing long put.
	2. Buy a new put at a strike with the same spread width.
4. Exit once Iron Fly breakeven is breached.
	- There is no point in adjusting when an option strike is ITM.

Upon forming the Iron Fly...
1. Max Profit will increase.
2. Max Loss will reduce.
3. Probability of Profit will go down.
	- This is due to the decreased breakeven range.

==No adjustment after Iron Fly fails!==

> We don't roll up the put side on the way up when IV is high and VIX is either sideways or falling down because put premium won't fall much as you continue selling as you shift up. [...](https://youtu.be/4QzubqTgtcc?t=1308)

### Scenario 2. When stock trends down
[...](https://youtu.be/4QzubqTgtcc?t=756)

When market goes down...
- It creates fear.
- When fear increases VIX rises.
- When the VIX is high the premium goes up. This is not good for option seller!

#### Stage 1. Spot price breaches the short put strike
[...](https://youtu.be/4QzubqTgtcc?t=936)

Since VIX is rising, IV will go up, with rising IV premiums will go up too. You can collect better premiums by shifting call side.

##### Action: Roll down call side

1. Wait till spot is about to breach the short put strike.
2. Slide down the short call by few points.
	1. Exit from the existing short call.
	2. Sell a new call at a strike 0.75% inward.
3. Slide down the long call by few points.
	1. Exit from the existing long call.
	2. Buy a new call at a strike 0.75% inward.
4. Wait for the breach of short put or next underlying support.
5. Upon breach revaluate scenario
	1. `If` further shifting results in an Iron Fly `then` Exit.
		- ==Don't convert to an Iron Fly== on the way down in a high VIX environment.
		- If you convert into an Iron Fly and price dumps then it will cause major losses.
	2. `Else` jump to step 2 as premium goes down.
		- Shift slowly by few points only (0.5% to 0.75%).
		- Shift by 50 points in Nifty.

## Approach 2. Slide inwards, sell extra and roll | Weekly

Reduce loss on the call side in 2 stages.

### Scenario 1. Stock trends up

#### Stage 1. Spot price breaches the resistance on chart
[...](https://youtu.be/kdGIe6J194A?t=519)

##### Action: Roll down the hedged long call

- To decrease loss make this strategy more debit.
- Slide down the `call side hedge 0.55% to 0.75% inside breakeven`.
	1. Exit the existing long call position.
		- Since the market is going up you will benefit from the profit.
	2. Buy a new call with strike 0.55% to 0.75% inwards from the breakeven.
		- Create this call inwards.
			- It will be closer to the resistance being breached.
			- 0.75% is 100 points in Nifty.
			- 0.55% is 200 points in Bank Nifty.
		- You will pay more than what you paid the last time you longed call.
	3. Observe the payoff chart again.
		- The t+0 blue line in opstra will become flat.
		- It may reduce your Max Loss by almost 50%.
	4. Revert step 1 and 2 if stock reverses.
		- You may have to spend little more on transactions.

#### Stage 2. Spot price breaches the call side breakeven
[...](https://youtu.be/kdGIe6J194A?t=681)

Next wait for the breach of breakeven point and after 1-2 days when market settles down then short an extra put.

##### Action: Sell an extra put and roll

- Offset losses from short call by collecting more credit.
	- Your max loss is defined and fixed in Iron Condor.
	- By selling extra put you further reduce this loss.
- For this sell an extra put on the side not being tested.
	- Sell at the breakeven point or far OTM as per your risk appetite.
	- You may sell this after 1-2 days when the market settles down.
	- Doing this will safe guard your position from the upside move.
	- It will also offset losses from the short call.

==Do not roll up put when VIX is high!==

> When VIX is high, rolling up puts does not help because the premium will not drop enough to result in enough gains.

### Scenario 2. Stock trends down `in high VIX`
[...](https://youtu.be/kdGIe6J194A?t=772)

Note that on the down side there is a higher probability that stock consolidates rather than crashing down.

#### Stage 1. Spot price breaches the short put strike

Next wait for the breach of breakeven point and after 1-2 day when market settles down then short an extra call.

##### Action: Sell an extra call and roll

- Offset losses by collecting more credit.
	- Your max loss is defined and fixed in Iron Condor.
	- By selling extra call you further reduce this loss.
- For this sell an extra call on the side not being tested.
	- Sell at the breakeven point or far OTM as per your risk appetite.
	- You will be able to sell new calls at better prices due to high VIX.
	- Doing this will safe guard your position from the downside move.
	- It will also offset losses from the short put.

#### Stage 2. Spot price breaches the breakeven
[...](https://youtu.be/kdGIe6J194A?t=846)

##### Action: Roll up the hedged long put

Roll up the long put side like so:
1. Exit the existing long put position.
	- You will receive some profit.
2. Buy a put closer to the support being breached.
	- Buy a new put at a strike 0.75% inward.
	- You will pay more than what you paid the last time you longed put.

### Scenario 3. Stock trends down in `low/normal VIX`

#### Stage 1. Adjust upon breach of range (support)

##### Action: Roll up the hedged long put

Make the strategy more debit by shifting hedges up on the side being tested.

Roll up the long put side like so:
1. Exit the existing long put position.
	- You will receive some profit.
2. Buy a put closer to the support being breached.
	- Buy a new put at a strike 0.75% inward.
	- You will pay more than what you paid the last time you longed put.

Now the t+0 blue line will become flat and reduce your Max Loss by almost 50%.

> If the stock reverses then you can revert this action by spending a little more on transactions.

#### Stage 2. Adjust upon breach of breakeven

Next wait for the breach of breakeven point and after 1-2 day when market settles down then short the call.

![[#Action Sell an extra call and roll]]

## Approach 3. Adjust position w/ delta | Weekly Expiry

#### Setup

Wait for VIX to come between 15 to 20.
- 15+ VIX gets better premiums even for strikes that are far from ATM.
- Avoid Iron Fly for 15+ VIX due to high volatility around ATM.

### Approach 1. Adjust upon delta imbalance
[...](https://youtu.be/szT7slKc4Vc?t=255)

#### Deployment

1. Create an Iron Condor like so:
	- Sell ≤ 20Δ strike call & put.
	- Buy ≤ 10Δ strike call & put as hedges.
2. Adjust strikes so that `Vertical Call Spread Width` and `Vertical Put Spread Width` are same.
3. Deploy on Monday with 10 DTE.

#### Adjustment

1. Track positional delta upon every 15 min candle close.
2. Wait for positional delta to go below 15Δ.
	- When positional delta is negative that means market is going up.
	- When positional delta is positive that means market is going down.
3. Adjust the untested side like so:
	- `If` positional delta is between 0Δ to -15Δ `then`
		- Exit long & short put positions.
		- Sell a new put option with delta that of current short call.
		- Buy a new put option with delta that of current long call.
	- `Else if` positional delta is between 0Δ to +15Δ `then`
		- Exit long and short call positions.
		- Sell a new call option with delta that of current short put.
		- Buy a new call option with delta that of current long put.
4. Confirm the neutral delta.
	- As and when we do adjustments the breakeven range will reduce.
5. Stop adjustment when position converts to `Iron Fly`.
	- Once we reach `Iron Fly` position then follow [[Iron Fly Playbook#Step 7 B Adjust position w delta]] or exit.
6. Go to step 1.

### Approach 2. Adjust upon breakeven breach
[...](https://www.youtube.com/watch?v=rnYRlexnc0Y)

#### Deployment

1. Create an Iron Condor like so:
	- Sell ≤ 30Δ call & put.
	- Buy ≤ 20Δ call & put as hedges.
2. Deploy this trade with 50% margin only.

#### Adjustment

1. Wait for spot price to breach breakeven.
2. Upon breach calculate the normalized/outstanding delta of the tested side.
	- Add delta of short and long option of the tested side to find outstanding delta.
	- We will use this outstanding delta to balance delta.
3. `First Adjustment:` Short an option with the outstanding delta like so:
	- `If` the outstanding delta is negative `then` short a call to balance.
	- `Else` short a put to balance.
4. Wait for imbalance in delta.
5. Upon delta imbalance calculate the normalized/outstanding delta of the tested side.
6. `Last Adjustment:` Short an option with the outstanding delta like so:
	- `If` the outstanding delta is negative `then` short a call to balance.
	- `Else` short a put to balance.
