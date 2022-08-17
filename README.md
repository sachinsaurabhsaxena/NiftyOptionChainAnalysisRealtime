# Nifty Option-Chain Analysis Real-time

    Nifty Option-Chain Analysis in Real-time

[![Codacy Security Scan](https://github.com/cyberjunky21/NiftyOptionChainAnalysisRealtime/actions/workflows/codacy.yml/badge.svg)](https://github.com/cyberjunky21/NiftyOptionChainAnalysisRealtime/actions/workflows/codacy.yml)

Introduction
Simple strategies for trend analysis in stock options data

Stock data analysis is one of the most endearing and exhaustive topics. Endearing because who does not want to earn profits in the stock market. Exhaustive because the length and breadth of this topic are infinite. You can easily get lost and overwhelmed with the amount of information that bounces at you when you explore this topic. So in this article, I will be focusing on one particular type of stock analysis i.e Options Chain analysis using Excel.

Option chain comprises data pertaining to option strikes of a particular stock or index in a single frame. It gives you all the specific data you need while trading in options. In this article, I will list out all the key concepts required to understand the option chain. I will show how to import option data to Excel and build custom reports based on option strategies. These reports will in turn help you to predict trends for options trading.

Key Concepts for Stock Options Chain Analysis
Derivative – is an instrument that derives its value from a specified asset. It is a contract that takes place between two people.

Option Contract – is a type of Derivative. These are of two types, Call (CE) and Put (PE). Option contract takes place between a buyer and a seller (writer). An option contract gives the buyer the right but not the obligation to buy or sell an underlying asset at a specified strike price on a specified date.

Strike Price – is the price at which a specific derivative contract can be exercised.

Expiry Date – is the date at which the option contract expires. Normally every option contract expires on the last Thursday of every month. Based on expiry, the option contract is categorized into 3 groups, Running option contract (nearest expiry), Middle option contract (mid expiry), Far option contract (farther expiry). For example, if for a contract the nearest expiry is last Thursday of March, then mid expiry will be last Thursday of April, and far expiry will be last Thursday of May. Once the contract expires, a new contract for the next month is generated. As a buyer or seller, you can hold the contract till the expiry. Thereafter if you don’t buy or sell then the contract expires, and you will lose the premium amount.

Call option contract – is a contract that gives the buyer the right but not the obligation to buy an asset. A premium amount must be paid to the seller for booking the asset. For example, say the strike price for a contract is Rs.150 when the buyer booked it for a premium of Rs.20. Now, after one month if the price of the asset increases to Rs.200, then the buyer can go ahead and buy and book a profit of Rs.30 after deducting the premium. Suppose if the price decreases to Rs.100 then the buyer is not obligated to buy. Here the buyer only stands to lose the premium amount. This is known as a Call option contract (Right to buy).

Put option contract – is a contract that gives the buyer the right but not the obligation to sell an asset. A premium amount must be paid to the seller for booking the asset. For example, say the strike price for a contract is Rs.200 when the buyer booked it for a premium of Rs.20. Now, after one month if the price of the asset decreases to Rs.150, then the buyer can sell the asset and book a profit of Rs.30 after deducting the premium. Suppose if the price increases to Rs.300 then the buyer is not obligated to sell the asset as the price has risen. Here the buyer only stands to lose the premium amount. This is known as Put option contract (Right to sell).

ATM, ITM, OTM – based on the underlying price of the asset, options contracts can be categorized as In the Money (ITM), At the Money (ATM), and Out of the Money (OTM). If the strike price is less than the market price then it is ITM, if the strike price is equal to the market price then it is ATM, and if the strike price is greater than the market price then it is OTM.

In options trading, contracts are bought or sold in chunks/lots. For example, one contract will comprise 100 shares. So, you always buy or sell in terms of the number of contracts and not the number of shares that each contract has.

Option Chain Deconstructed
An options chain is a listing of all available options contracts for a given index/stock. It provides detailed quotes and price information. It shows all listed puts, calls, their expiration, strike prices, and volume for a single underlying asset within a given maturity period. The option chain is categorized by expiration date and segmented by calls and puts. Here is a screenshot of a portion of the option chain for Nifty taken from the NSE website.

Option Chain Deconstructed
Data in the option chain chart is grouped into 4 quadrants. Two for Calls (Yellow and White) and two for Puts (Yellow and White). The Yellow quadrant data is for In the Money contracts and the White quadrant data is for Out of the Money contracts. This is applicable for both Call and Put, but the meaning of ITM and OTM has reversed accordingly.

Some of the key columns that are required to understand the option chain chart/matrix are:

OI (Open Interest) – is the number of contracts that are traded but not exercised. It indicates the interest of traders for an option at the given strike price. Higher OI means more interest among traders, and hence indicates high liquidity for the buyer/seller to trade their options.

CHNG IN OI – is the change in OI within the expiration period. It indicates the number of contracts that are closed or exercised.

VOLUME – is the total number of contracts that are traded for a specific strike price in a given period. It is calculated on daily basis.

IV (Implied Volatility) – is the indication of how the market reacts to the price movement of an underlying asset.

LTP (Last Traded Price) – is the last traded price or premium price of an option.

CHNG – is the net change in LTP. It is indicated as a positive or negative value. Positive change means a rise in price (shown in green). A negative change means a decrease in price (shown in red).

BID QTY – is the number of orders for buying at a specific strike price. It indicates the current demand for the order.

BID PRICE – is the price for the latest buy order. If this price is higher than the LTP then it indicates higher demand for the option and vice versa.

ASK PRICE – is the price of the latest sell order.

ASK QTY – is the number of sell orders that are open. It indicates the option supply.


Snapshot of the Live Worksheet
![NIFTYRT](https://user-images.githubusercontent.com/44409374/184597635-c7c50157-6b6e-4eb1-83c7-5802917ab898.png)

