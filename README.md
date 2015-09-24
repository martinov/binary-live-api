# binary-live-api

This library is a high-level abstraction over the [Binary.com Developers Portal](https://developers.binary.com)

```
var api = new LiveApi();
api.authorize('yourtoken');
api.getPortfolio();
api.on('portfolio', function(data) {
    // do stuff with portfolio data
});
```


## Utility Functions

```
isReady() - true if connected, false if not yet connected or disconnected
```

```
send(data)
```

## Unauthenticated Calls

```
getMarketHistory(marketHistoryOptions)
```

[Documentation for Tick History API Call](https://developers.binary.com/api/#ticks)

```
getActiveSymbolsBrief()
```

[Documentation for 'Active Symbols' API Call](https://developers.binary.com/api/#active_symbols)

```
getActiveSymbolsFull()
```

[Documentation for 'Active Symbols' API Call](https://developers.binary.com/api/#active_symbols)

```
getContractsForSymbol(symbol)
```

[Documentation for 'Contracts For Symbol' API Call](https://developers.binary.com/api/#contracts_for)

```
getPayoutCurrencies()
```

[Documentation for 'Payout Currencies' API Call](https://developers.binary.com/api/#payout_currencies)

```
getTradingTimes(date = Date.now())
```

[Documentation for 'Trading Times' API Call](https://developers.binary.com/api/#trading_times)

```
ping()
```

[Documentation for 'Ping' API Call](https://developers.binary.com/api/#ping)

```
getServerTime()
```

[Documentation for 'Server Time' API Call](https://developers.binary.com/api/#time)


## Streams

```
subscribeToTick(symbol)
```

[Documentation for 'Tick Stream' API Call](https://developers.binary.com/api/#tick)

```
subscribeToTicks(arrayOfSymbols)
```

[Documentation for 'Tick Stream' API Call](https://developers.binary.com/api/#tick)

```
getLatestPriceForContractProposal(contractProposal)
```

[Documentation for 'Price Proposal' API Call](https://developers.binary.com/api/#proposal)

```
unsubscribeFromTick(symbol)
```

[Documentation for 'Tick Stream' API Call](https://developers.binary.com/api/#tick)

```
unsubscribeFromTicks(symbols)
```

[Documentation for 'Tick Stream' API Call](https://developers.binary.com/api/#tick)

```
unsubscribeFromAllTicks()
```

[Documentation for 'Forget' API Call](https://developers.binary.com/api/#forget)

```
unsubscribeFromAllProposals()
```

[Documentation for 'Forget' API Call](https://developers.binary.com/api/#forget)

```
unsubscribeFromAllPortfolios()
```

[Documentation for 'Forget' API Call](https://developers.binary.com/api/#forget)

```
unsubscribeFromAlProposals()
```

[Documentation for 'Forget' API Call](https://developers.binary.com/api/#forget)


## Authenticated Calls

```
authorize(token)
```

[Documentation for 'Authorize' API Call](https://developers.binary.com/api/#authorize)

```
getBalance()
```

[Documentation for 'Balance' API Call](https://developers.binary.com/api/#balance)

```
getStatement(statementOptions = {})
```

[Documentation for 'Statement' API Call](https://developers.binary.com/api/#statement)

```
getPortfolio(subscribeToUpdates)
```

[Documentation for 'Portfolio' API Call](https://developers.binary.com/api/#portfolio)

```
getPriceForOpenContract(contractId)
```

[Documentation for 'Price Proposal - Open Contract' API Call](https://developers.binary.com/api/#proposal_open_contract)

```
buyContract(contractId, price)
```

[Documentation for 'Buy Contract' API Call](https://developers.binary.com/api/#buy)

```
sellContract(contractId, price)
```

[Documentation for 'Sell Contract' API Call](https://developers.binary.com/api/#sell)
