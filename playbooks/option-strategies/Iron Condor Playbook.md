[https://www.youtube.com/watch?v=kdGIe6J194A](https://www.youtube.com/watch?v=kdGIe6J194A)

- It is a better to use `Double Diagonal Calendar Spread` instead of `Iron Condor` for weekly options.
- It works better when VIX is between 17 to 25.

# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

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

# Step 4. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 5. Adjust position

## Possibility 1. When stock trends up

Reduce loss on the call side in 2 stages.

### Stage 1. Adjust upon breach of range (resistance)
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=519)

#### Roll down the hedged long call

First decrease losses by collecting more credit to offset losses.

Make the strategy more debit by increasing hedges on the side being tested. Roll down the long call side like so:
1. Close the existing long call. You will receive some profit.
2. Long a call closer to the resistance being breached.

Now the t+0 blue line in opstra will become flat and reduce your Max Loss by almost 50%.

> If the stock reverses then you can revert this action by spending a little more on transactions.

### Stage 2. Adjust upon breach of breakeven
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=681)

Next wait for the breach of breakeven point and after 1-2 day when market settles down then roll up the short put.

#### Roll up the short put

On the side that is not being tested short a put option at the breakeven point or far OTM for more safety to offset losses from the short call.

## Possibility 2. When stock trends down
[...](https://youtu.be/kdGIe6J194A?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=772)

> Note that on the down side there is a higher probability that stock consolidates rather than a sharp plunge.

### Stage 1. Adjust upon breach of range (support)

#### Roll up the hedged long put

First decrease losses by collecting more credit to offset losses.

Make the strategy more debit by increasing hedges on the side being tested. Roll up the long call side like so:
1. Close the existing long put. You will receive some profit.
2. Long a put closer to the support being breached.

Now the t+0 blue line will become flat and reduce your Max Loss by almost 50%.

> If the stock reverses then you can revert this action by spending a little more on transactions.

### Stage 2. Adjust upon breach of breakeven

Next wait for the breach of breakeven point and after 1-2 day when market settles down then roll up the short put.

#### Roll down the short call

On the side that is not being tested short a call option at the breakeven point or far OTM for more safety to offset losses from the short put.
