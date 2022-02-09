[...](https://www.youtube.com/watch?v=4QzubqTgtcc) | [https://www.youtube.com/watch?v=kdGIe6J194A](https://www.youtube.com/watch?v=kdGIe6J194A)

- It is a better to use `Double Diagonal Calendar Spread` instead of `Iron Condor` for weekly options.
- It works better when VIX is between 17 to 25.

# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

Prefer calculating range using VIX or IV.
- [[Option Greeks#Calculating Expected Move or Range using IV]]

# Step 2. Cover range
[[Strategy Builder Playbook#Step 2 Cover range]]

# Step 3. Define risk
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=246)

Hedge naked strangle using Iron Condor.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive 10k in credit, then only debit 10k for hedging.
2. Use `breakevens` to pick strikes for hedging.
	- Use the received credit to buy put and call at the breakeven (approx).
	- By buying PE & CE options at the breakeven will reduce the breakeven range.

# Step 4. Deploy strategy

- Deploy only when VIX is below 18.
- If VIX is high deploy this strategy on Tuesday @ 3 PM and exit within next 2 days.

# Step 5. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 6. Adjust position

## Possibility 1. When stock trends up

Reduce loss on the call side in 2 stages.

### Stage 1. Adjust upon breach of range (resistance)
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=519)

#### Roll down the hedged long call

First decrease losses by collecting more credit to offset losses.

Make the strategy more debit by increasing hedges on the side being tested. Roll down the long call side like so:
1. Close the existing long call. Since the market is going up you can book some profit.
2. Buy a call option closer to the resistance being breached.

Now the t+0 blue line in opstra will become flat and reduce your Max Loss by almost 50%.

> If the stock reverses then you can revert this action by spending a little more on transactions.

### Stage 2. Adjust upon breach of breakeven
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=681)

Next wait for the breach of breakeven point and after 1-2 day when market settles down then roll up the short put.

#### Roll up the short put

On the side that is not being tested short a put option at the breakeven point or far OTM for more safety to offset losses from the short call.

==Do not roll up put when VIX is high!==

> When VIX is high, rolling up puts does not help because the premium will not drop enough to result in enough gains.

### Stage 3. Convert to Iron Fly

- As you rollup the short put, you will reach a point where strangle becomes straddle.
- At this point...
	1. Max Profit will increase.
	2. Max Loss will reduce
	3. Probability of Profit will go down.
- Exit once Iron Fly breakeven is breached.

==No adjustment after Iron Fly fails!==

## Possibility 2. When stock trends down

### Case 1. VIX is high
[...](https://youtu.be/4QzubqTgtcc?t=756)

When the market goes down in high VIX times the premium rises fast.

#### Stage 1. Adjust upon breach of short put strike

Next wait for the breach of breakeven point and after 1-2 day when market settles down then roll up the short put.

##### Roll down the short call

On the side that is not being tested short a call option at the breakeven point or far OTM to offset losses from the short put.
	- You will be able to sell new calls at better prices due to high VIX.
	- Roll down calls very slowly, cover few points only. Don't roll fast!
	- Keep rolling down till Iron Fly is not formed.

==Don't convert to Iron Fly!==

### Case 2. VIX is normal or low
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=772)

Note that on the down side there is a higher probability that stock consolidates rather than crashing down.

#### Stage 1. Adjust upon breach of range (support)

##### Roll up the hedged long put

First decrease losses by collecting more credit to offset losses.

Make the strategy more debit by increasing hedges on the side being tested. Roll up the long call side like so:
1. Close the existing long put. You will receive some profit.
2. Long a put closer to the support being breached.

Now the t+0 blue line will become flat and reduce your Max Loss by almost 50%.

> If the stock reverses then you can revert this action by spending a little more on transactions.

#### Stage 2. Adjust upon breach of breakeven

Next wait for the breach of breakeven point and after 1-2 day when market settles down then roll up the short put.

##### Roll down the short call

On the side that is not being tested short a call option at the breakeven point or far OTM for more safety to offset losses from the short put.
