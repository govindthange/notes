[...](https://www.youtube.com/watch?v=IIDfzxJYwuk)

# Debit Spread

- Choose debit spread when VIX is low.
	- With lower VIX you can't collect enough premium by shorting.
	- Wiht lower VIX, you can anticipate higher VIX in future so you can benefit from long option as you can sell them for higher premium later.

# Credit Spread
[...](https://youtu.be/T6uA_XHunRc?t=549) | [...](https://www.youtube.com/watch?v=7pSw_qqyEXk)

- Choose credit spread when VIX is high.
	- With higher VIX you get to collect higher premium by shorting.
	- With higher VIX, you can anticipate lower VIX in future so you can benefit from shorting option as you can buy them at a lesser premium later.
- Short a 30Δ strike to have 70% chance of winning.
- Exit at 50% of the credit received or 21 DTE.

## Manage Trades
[...](https://www.youtube.com/watch?v=lryM4Hb3mhM)

We control our risk on order entry only. So if something does happen then we should be ready to absorb the loss.

|                       | Put Credit Spread | Call Credit Spread |
| --------------------- | ----------------- | ------------------ |
| Assumption            | Bullish           | Bearish            |
| Rolling into Strength | Stock Drops       | Stock Rallies      |
| Roll Timing           | Dance Floor       | Dance Floor        |
| Credit Received       | Possibly Lower    | Possibly Higher    |

### Manage the winners

- No need to manage winners!
	- If you put on a short put spread and the stock goes higher, then it is going to be an easy winner.
	- If you put on a short call spread and the stock goes lower, then it is going to be an easy winner.

- Profit Target
	- 50% of credit received.
	- Close the trade.
	- Look for a new opportunity.

### Manage the losers
[...](https://www.youtube.com/watch?v=IIDfzxJYwuk)

- 21 days to expiration
	- Roll position to the next monthly cycle. It gives us more time to be right.
	- Only roll forward for a credit.
		- You keep the same strikes.
		- You buy the option to define the risk.
		- You may have to pay more if the volatility skew is going against you.
		- Roll out in time for a credit if the intention is to stay in the trade.
			- Your objective should be to stay in the trade and have time on your side.
			- Less "drag" on the short optoin's decay.
	- Do not roll spread out for debit.
		- This is when our stock price has breached both of our strikes ( the long and short).
		- The problem with this is that we pay a debit, increase our risk, reduce our profit, and our strikes are now ITM.
		- Do not pay debit for rolling the position forward because it will add risk to the position. When you roll you end up paying more for defining the risk by going long on option.
		- Note that you will have to pay the debit if the position is too far gone. In this case you will have to sit and wait.
- Closing trade at a max loss is a worst thing you can do. Since you have defined the risk, you should give it time.
	- The closers you are to the max loss, the more inclined you should be to hold on to that trade.
	- You can close the position only near the expiration to avoid assignment risks.

### Manage the dance floor

The stock price is on the dance floor when it is closer to the short strike and has not gone too far in the money.

- Don't let the spread go ITM.
	- Focus on extrinsic value in short vs long.
	- When you let the spread go ITM, then your long option has more extrinsic value than your short option.
	- As long as your short option has more extrensic value than your long option...
		- You will be able to roll out in time for credit
		- You can reduce your max loss potential
		- You can increase your max profit potential
		- And adding more time to your trade allows you to have a slower moving trade.
	- Your spread go ITM when there is a gap up/down. There is not much you can do beyond staying alerts.
- Use Implied Volatility Rank (IVR)
	- If IVR is high then consider rolling.
		- IV is a mean reverting entity so if it comes down it will help you reach your profit target.
	- If IVR is low then take the trade off.
		- Consider closing the trade when IVR has collapse.
		- Move on and look for a new opportunity.
- The best time to roll is when stock price is near the short option.
	- Use alerts to ensure stock does not break through spread.
- If we are too late in rolling and stock has breached through the spread, we may be forced to do nothing and let the probabilities play out. This isn't the worst thing to happen as long as we traded small.
