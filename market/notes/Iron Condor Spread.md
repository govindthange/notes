[...](https://www.youtube.com/watch?v=6HwsyxyOw2Y&t=625s)

> Many newbies begin with `Iron Condor` but the interesting fact is even the most professional traders who have years of experience regularly trade Iron Condor. By understanding this one strategy you won't be just scratching the surface but be above the curve and at a level of the people who have been doing this forever. For professional traders, this is there go to strategy for just about everything they do.


- Iron Condor is a side ways market strategy where `Vega` is negative.
- Iron Condor Spread has extremely `poor R/R`.

# Long Iron Condor
=> Our view is a big move to the up or down side. We sell this strategy to someone who expects a no price move and price trades in a range.

# Short Iron Condor
=> Our view is neutral. We sell our strategy to someone who expects a big move to the up/down side.

- A Short Iron Condor is a directionally neutral strategy.
- Its created by simulataneously `selling` two [[Vertical Spread]] i.e. a `Vertical Call Spread` and a `Vertical Put Spread` of the same expiry.
	- When we are selling a `Call Spread` component we only want price to stay below a certain strike (the resistance). We don't really expect a big move to the downside though. 
	- When we are selling a `Put Spread` component we only want prices to stay above a certain strike (the support. We don't really expeect a big move to the upside though.
- Iron Condors take advantage of the `passage of time` and `high option prices`.

You want the following:
- Price to stay in a given range.
- Time passes by and the spread expires worthless.
- Collect higher premium and make profit.

When you create an Iron Condor pay attention to how wide are the strikes in an individual call and put spread.
- You want to know how wide a call spread is and how much we are collecting on that call spread.

## Example

Your analysis says that market is more likely to stay somewhere between 160 and 185 rather than above $190 or below $155.

### Vertical Call Spread

SHORT `185CE 1/19 (64d)` @ $1.57 (Receivable)
LONG `190CE 1/19 (64d)` @ $0.93 (Payable)
`Spread Width` => 190 - 185 => 5

`Lot Size` = 100
`Received CE Spread Cost` => `Lost Size` x (`Received $1.57` - `Paid $0.93`) => $64

### Vertical Put Spread

SHORT `160PE 1/19 (64d)` @ $1.86 (Receivable)
LONG `155PE 1/19 (64d)` @ $1.15 (Payable)
`Spread Width` => 160 - 155 => 5

`Lot Size` = 100
`Received PE Spread Cost` => `Lost Size` x (`Received $1.86` - `Paid $1.15`) => $71

### P&L

`Spot Price` = 171.58
`Exit Price` = ??

`Total Received Spread Cost` => `Received CE Spread Cost` + `Received PE Spread Cost` => $64 + $71 => $135
`Max Loss` => (`Spread Width` x `Lot Size`) - `Total Received Spread Cost`
 		=> (5 x 100) - $135 => $365
`Max Gain` => `Total Received Spread Cost` => $135

### Note

If you widen the `Spread Width` then your `Max Gain` goes down and `Max Loss` increases. Its all about balance.

# Adjusting Position
[...](https://www.youtube.com/watch?v=cUfJ3-6uHiM)

Keep adjusting position by rolling over the winning side of the spread till the `Iron Condorl` becomes [[Iron Fly]]

## Plan of Action

- On `1 Hr Chart` Draw Trends and Ranges as per [[Market Structure#The Lay of The Land]]
- As soon as the market structure breaks (i.e. Price breaks trendline or S/R level) rollover position like so:

### Shift by matching Premium

### Shift by matching Δ

## Example

As per your analysis Nifty would stay between 11050 and 12400 rather than above 12550 or below 10900.

### Vertical Call Spread

SHORT `12400CE 11/12 (7d)` @ ₹28.25 (Receivable)
LONG `12550CE 11/12 (7d)` @ ₹13 (Payable)
`Spread Width` => 12550 - 12400 => 150

`Lot Size` = 75
`Received CE Spread Cost` => `Lost Size` x (`Received ₹28.25` - `Paid ₹13`) => ₹1143.75

### Vertical Put Spread

SHORT `11050PE 11/12 (7d)` @ ₹29.7 (Receivable)
LONG `10900PE 11/12 (7d)` @ ₹14.2 (Payable)
`Spread Width` => 11050 - 10900 => 150

`Lot Size` = 75
`Received PE Spread Cost` => `Lost Size` x (`Received ₹29.7` - `Paid ₹14.2`) => ₹1162.5

### P&L

`Spot Price` = 171.58
`Exit Price` = ??

`Total Received Spread Cost` => `Received CE Spread Cost` + `Received PE Spread Cost` => ₹1143.75 + ₹1162.5 => ₹2306.25
`Max Loss` => (`Spread Width` x `Lot Size`) - `Total Received Spread Cost`
 		=> (150 x 75) - ₹2306.25 => ₹8943.75
`Max Gain` => `Total Received Spread Cost` => ₹2306.25


### Adjustment Steps
[...](https://youtu.be/cUfJ3-6uHiM?t=715)

