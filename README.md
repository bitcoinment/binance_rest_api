![binance_rest_api](https://raw.github.com/bitcoinment/binance_rest_api/master/binance_rest_api.gif)

# Best API for Binance.com (2018)

Getting fresh orders in real time. 
Documentation for the Binance APIs and Streams.

[Check out the Interactive Demo](http://kupi.net/p/docs-api)

With this module, you can develop your own crypto-bots, analyze crypto-markets and of course, make money.

Our web-service works 24 hours and keeps high loads

The data of all exchanges come in a single format and contain extended information (links for switching to trading pairs, best asks and bids, exchange rates and much more).

---

- FREE!
- The actuality of orders is 5-30 seconds!
- Data from most exchanges
- Round-the-clock support


### Installation Instructions
    $ pip3 install binance-rest-api==4.0.1

### Init example
```python
from binance_rest_api import binance_rest_api
```

### Stocks API
```python
# Get all stocks
binance_rest_api.KUPINET('freeApi').Stocks().getList()

# Get orders by Stock name
binance_rest_api.KUPINET('freeApi').Stocks('Binance').getOrders('ETH','BTC')

# Get all pairs from the Stock
binance_rest_api.KUPINET('freeApi').Stocks('Binance').getAllPairs()
```
### Pairs API
```python
# Find best prices for Pair in all Stocks
binance_rest_api.KUPINET('freeApi').Pair('LTC','ETH').getBestPrices()
```
### Find Best Prices API
```python
# Find best ASK
binance_rest_api.KUPINET('freeApi').BestPrices('LTC').Ask()

# Find best BID
binance_rest_api.KUPINET('freeApi').BestPrices('LTC').Bid()
```
### Cryptocurrency Converter (Calculator) API
```python
# Coins list
binance_rest_api.KUPINET('freeApi').Calc().Data()

# Convert Coin to Coin
binance_rest_api.KUPINET('freeApi').Calc('LTC','ETH').Amount(10)
```

## In the future
- Unloading historical trade data
- Multi-trading through a single terminal
- Tool for crypto arbitrage
- API for JavaScript, PHP, C#
- Launch of a decentralized exchange
- Widget (calculator) for integration with sites


## About us
 We are a team of crypto developers. Our goal is to make the most convenient crypto services possible.
[Contact with us](http://kupi.net/p/support)