[3 Leg Calendar Spread](https://www.youtube.com/watch?v=ckLoa_et1qg)

- References
	- [3 Leg Calendar Spread](https://www.youtube.com/watch?v=ckLoa_et1qg)
	- [3 Leg Calendar Spread Back Testing](https://www.youtube.com/watch?v=R9fgH7XEmYA)
	- [Triple Calendar Spread](https://tradersfly.com/blog/building-a-triple-calendar-spread-options-trade-live-planning-a-trade/)
# Step 1. Define legs

`Multi Leg Calendar Spread` (MCS) is formed by combining 1 long option of near expiry, 2 short option of next expiry, and 1 long option for far expiry.

# Step 2. Deploy strategy

This strategy can be deployed on any day of the month.

- Deploy strategy on Monday @ 10:30 AM.
- Exit strategy next week on Thursday @ 9:20 AM.

## Position Size

1. Look at the blue t+0 line in opstra.
2. Move your cursor over the t+0 line at the lowermost breakeven point.
3. Note down the loss.
4. If this `loss` is ≤ `2% of total trading capital` only then deploy the strategy.
5. If `loss` > `2% of the total trading capital` then skip and wait for the next opportunity.

# Step 3. Monitor position

