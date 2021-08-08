
# Types

## Outright Forward Contracts

## Non Deliverable Forward Contracts (NDF)

# Segments

## Equity Market

### Index Futures

CNX Nifty, CNX Nifty Mini, CNX IT, Bank Nifty

### Futures on Individual Securities

Any of the 186 NSE approved securities

## Fixed Income Markets

Each contract has following characterisitcs:
- `Per Contract Value:` 2,00,000
- `Lot Size:` 2000
- `Tick Size:` 0.01
- `Maturity Period:` 1 Year with 3 months continuous contracts for the first 3 months and fixed quarterly contracts for the entire year.
- No min/max price ranges.
- Operating range for `Interest Rate Futures Contract` is ±2%

The settlement price is as stipulated by National Secuirities Clearing Corporation Lt.d (NSCCL)

All contracts are cash settled!

### Notional 10-Year bond with 6% coupon

### Notional 10-Year zero coupon bond

### Notional 91-day Treasury Bill

## Commodity Markets

NCDEX, MCX, NMCX

Most of the contracts are cash settled.
- Less than 5% are physically delivered.
- Counterparties agree on the mode of settlement prior to expiry.
- The settlement price takes into account the possibility of differences in quality.
- Counterparties are insured against the quality issues.

## Currency Futures

USD/INR, EURO/INR, GBP/INR, JPY/INR are traded on NSE and MCX.

[[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018 | Page #40]]

# Design Aspects
4433
## Margin Account Operations

The whole purpose of margining system is to ensure that funds are available to pay traders when they make a profit.

- Initial Margin: the amount deposited at the time of entering contract.
	- Generally brokers pay interest on the balance in a margin account.
	- Treasury Bills can be deposited in lieu of cash at about 90% of their face value.
	- Stocks can be deposited in lieu of cash at about 50% of their market value.
	- Minimum magin levels are specified by the exchange clearing house.
	- Minimum margin levels are determined by and directly proportional to the variability of the price of the underlying asset and are revised when necessary.
	- A company that produces the commodity (a bona finde hedger) are subjected to less margin requirements.
	- Day trades and spread transactions (like [[Vertical Spread]]) often give rise to lower margin requirements than do hedge transactions.

- Maintenance Margin: this ensures that margin amount never becomes negative.
	- Usually 75% of the initial margin.
	- This does not earn interest as it constitutes daily settlement.
	- Margin Call: when the amount goes below the maintenance margin the trader receives a margin call from the broker to top up.
	- Top Up: the trader must deposit fund to top up the margin account by end of the next day.
	- Variation Margin: the amount required to bring the account balance up to the initial margin level. 

### Mark to Market (MTM or Daily Settlement)

At the end of each trading day the margin account is adjusted to reflect the trader's gain or loss.

A trade is first settled at the close of the day on which it takes place.

The trade is then settled at the close of trading on each subsequent day.

## Delivery

### Intention to Deliver Notice

## Critical Contract Days

- First Notice Day: the first day on which `Intention to Delivery Notice` can be submitted to the exchange.
- Last Notice Day: the last day on which `Intention to Delivery Notice` can be submitted to the exchange.
- Last Trading Day: a few days before the last notice day.

## Order Types

### Limit Order

### Stop Order

### Stop-Limit Order

As soon as there is a bid/offer price at `Stop Price`, the `Stop-limit Order` becomes a Limit Order at `Limit Price`.

#### Stop-and-limit Order

when Stop Price = Limit Price

### Market-if-touched (MIT) or Board Order

Order is executed after a trade occurs at a specified or more favorable than specified price.

Contrast this with Stop Order. It ensures profits are taken if sufficiently favorable price movements occur.

### Discretionary or Market-not-held Order

### Day Order

Expires at the end of the trading day.

### Time-of-day Order

Specify time period during the day when the order can be executed.

### Open Order or Good-Till-Cancelled Order (GTC)

The order is good until executed or until the end of trading in the particular contract.

### Fill-or-kill order

Execute immediately on receipt or not at all.

# Participants

## Clearing House

### NSCCL

National Securities Clearing Corporation Ltd.

### Traders

#### Types

##### Futures Commission Merchants (FCMs)

Follow client instructions and charge a commission for doing so.

##### Locals

Trade on their own acccount.

#### Categories

##### Hedgers

##### Speculators

- Scalpers: watch for short-term trends and attempt to profit from small changes in the contract price.
- Day Traders: unwilling to take the risk that adverse news will occur overnight.
- Position Traders: hope to make significant profits from major movements in the markets.

##### Arbitrageurs

