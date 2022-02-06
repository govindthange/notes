[...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=592)

# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 2. Cover range
[[Strategy Builder Playbook#Step 2 Cover range]]

Make straddle exactly at the middle of the range.
- You need not short call and put at the exact same strike. Its fine to go slightly diagonal i.e. shorting at slightly different strikes.
- You may also short ATM instead of middle of the range.

# Step 3. Define risk

Hedge naked straddle using Iron Fly.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive 10k in credit, then only debit 10k for hedging.
	- Its fine to pay slightly extra.
2. Use one of the following 2 approaches to hedge:
	1. Either use `breakevens` to pick strikes for hedging.
		- Use the received credit to buy put and call at the breakeven (approx).
		- By buying PE & CE options at the breakeven will reduce the breakeven range.
	2. Or pick the strikes corresponding to the credit received from the sold options.
3. By buying PE & CE options will increase breakeven range.

# Step 4. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 5. Adjust position
