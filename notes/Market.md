
# Badla System (India)

Long = Badla (Byaj) i.e. Contango
Short = Ulta Badla i.e. Backwardation

A unique system of carry forward of transaction involving 4 parties:
1. Long Buyer
2. Financer (stepped in to contribute capital in case of mismatch in purchase position)
3. Short Seller
4. Stock Lender (stepped in to contribute stock in case of mismatch in sale position)

Investor protection was the weakest link. There was no mechanism to protect the interests of small investors.

# Over-the-counter (OTC)

OTC markets are where companies agree to do derivatives transactions without exchanges.

## OTC Functions

[[#Exchange Functions]]

### Credit Risk

### Clearing Transactions

Collateral Agreement and Margining System significantly reduces the collateral risk in the bilaterally cleared OTC market.

Regulations require standard transactions between financial intitutions (like banks, insurance companies, pension funds and hedge funds) to be cleared through CCPs.

Transactions with most nonfinancial corporations and foreign exchange transactions are extempt from the regulations.

#### Bilateral Clearing

##### Margining System

In the past this rarely required initial margin ibut 2016 regulations require both initial and variation margin to be provided for bilaterally cleared transactions between financial institution.
- The initial margin is posted with a third party and calculated on a gross basis (no netting).
- Initial Margin: margins provided in the form cash usually earns interest.
- Daily Variation Margin: It earns interest when done in the form cash.

##### Master Agreement (Collateral)

- Credit Support Annex (CSA)
	- Collateral Agreement: Its similar to Margining System in Central Clearing.
		- This agreement requires transaction be valued everyday.
		- If transaction valuation between A and B increases by X to A then B needs to offset this increase by providing collateral worth X to A.
- International Swaps and Derivatives Association (ISDA) Master Agreement

#### Central Clearing

A central counterparty (CCP) stands between the two parties.

##### Margining System
- Initial Margin: margins provided in the form cash usually earns interest.
- Daily Variation Margin: It earns interest when done in the form cash.
- Guarantee Funds

## Exchange Tools

Companies take positions in derivatives to offset an exposure to the price of an asset.

### Forward Contracts

Forwards are private arrangements between two parties whereas futures are traded on exchanges.

A forward contract is a private non-standardized contract between two parties with a spcified delivery date and is settled at the end of contract. There is no standard contract size or standard delivery arrangements. Unlike in futures, there is only a single delivery date.

Unlike futures contracts, forward contracts are traded in OTC and are customizable to meet user's need.

Forward contracts are settled at the end of its life.

> In India the legislation (Securities Contract Regulation Act 1956) that governs derivatives trading only legalizes exchange based trading and does not mention anything about trades done on OTC. So credit risks are not mitigated in any manner i.e. there is no legal remedy in case one of the counterparty in a forward contract defaults.

## Participants

### Central Counterparties (CCP)

OTC transactions are routed through CCP. There are multiple CCPs.

It takes on the credit risk of the 2 parties by becoming a counterparty to both.
- So if A agrees to buy an asset from B in one year for a certain price then they both present this transaction to CCP so that CCP becomes the counterparty.
- By becoming a counterparty to this the CCP would essentially buy the asset from B in one year for the agreed price and sell the asset to A in one year for the agreed price.

### CCP Members

### OTC Market Participant

# Exchange
[...](https://www.youtube.com/watch?v=AFJ5Il_C4EY)

Exchange standardizes the contracts.

As the two parties don't know each other it provides a mechanism that gives two parties a guarantee that the contract will be honoured.

## Exchange Types

### Regional Exchanges (Single Product)

### National Exchanges (Multi-Commodity Exchanges)

## Participants

### Exchange Clearing House
[...](https://youtu.be/AFJ5Il_C4EY?t=770)

`Margin Account Operation:`

### Clearing House Members

A clearing house member must keep a margin account with the exchange clearing house.

`Margin Account Operation:`

### Brokers

A broker must be a Clearing House Member or maintain a margin account with a clearing house member.

`Margin Account Operation:`

### Traders

To protect against the possibility of a default a trader keeps a margin account with his broker. The account is adjusted daily to reflect gains/losses and from time to time are required to be topped up if adverse price movements takes place.

- [[#Hedgers]]
- [[#Speculators]]
- [[#Arbitrageurs]]

## Exchange Functions

- Organize trading so that contract defaults are avoided (through marins)

### Price Discovery

### Price Risk Transfer

### Price Dissemination

## Exchange Tools
[...](https://youtu.be/AFJ5Il_C4EY?t=263)

Exchange needs tools to implement its 3 critical functions.

The above 3 Exchange Functions rely on the following 2 basic instruments to separate the risk element from any commodity and allow that risk to be reassigned. This process of risk transfer is called as [[Hedging]].

Companies take positions in derivatives to offset an exposure to the price of an asset.

### Futures

Futures contracts are standardized and traded in exchanges.

Futures contracts are settled daily (via MTM). Unlike forward contracts there is a range of delivery dates specified.

What distinguishes futures from the forward contracts is the aspect of daily settlement.

A futures contract precisely specifies the following:
- What (The asset name),
- How much
	- Total quantity per contract,
- When
	- Delivery month
	- Delivery period in the month
	- When trading in a particular month begins
	- The last day of trading i.e. typically a few days before the delivery date)
- Where i.e. the location where the asset can be delivered.
- The grade (exchange stipulated quality for commodities)
- The alternatives grade
- The alternative location
- The price quotation (either dollar or cents)
- Daily Price Limit for ceasing trading (limit-up, limit-down, limit-move)
- Position Limit (max number of contracts a speculator can hold)

Forward/Futures contracts are designed to `neutralize the risk by fixing the price` that hedger will pay or receive for the underlying asset.

Futures contracts are free.

The disadvantage of futures is that the hedger no longer gains from the favorable movement in prices.

### Options on Futures
[...](https://youtu.be/AFJ5Il_C4EY?t=603)

Options contracts are designed to provide `insurance` by protecting investors from adverse price movement in future while allowing them to benefit from the favorable price movement.

Option contracts costs some upfront fee.

[[Option Contract]]

### Comparison

Futures and Contracts are similar in which they both provide a way in which a type of leverage can be obtained.

The difference is that potential loss and gain in futures is unlimited whereas in option the loss is limited but gains are unlimited.

# Hedging
[...](https://youtu.be/AFJ5Il_C4EY?t=279)

The purpose of hedging is to reduce the risk. There is no guarantee that the outcome with hedging will be better than the outcome without hedging.

By hedging the business can `lock in today's prices to meet tomorrow's goals` regardless of any change in the world which affects price.

# Contract Execution
[...](https://youtu.be/AFJ5Il_C4EY?t=712)

# Market Participants (Traders)

## Hedgers

Hedgers avoid exposure to the adverse price movement of an asset.

## Speculators

Speculators take position to bet on the direction of the market (i.e. price).

Speculators are important market participants because they add liquidity to the market.

## Arbitrageurs

Arbitrageurs take advantage of discrepancy between prices in two different markets. 

Arbitrageurs lock in riskless profit by simultaneously entering into transactions in two or more markets.

# Comparison of Forward and Futures

[[1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018 | Page #52, Table 2.6]]