# Python library for working with the DeDust API.

## Installation

```shell
pip install pydedustapi
```

import example:
```python
from pydedustapi import Dedust

api = Dedust()
```

## Methods Dedust()

### get_liquidity_providers_v1
The endpoint is used to get a list of liquidity providers for a pair.

| Parameter | Information |
|---------|-------------|
| address | address |

Ex:
```python
api.get_liquidity_providers_v1(address)
```


### get_accounts_assets
The endpoint is used to get the list of user assets.

| Parameter | Information |
|---------|-------------|
| address | address |

Ex:
```python
api.get_accounts_assets(address)
```


### get_accounts_trades
The endpoint is used to get the list of trades of an account.

| Parameter | Information |
|---------|-------------|
| address | address |

Ex:
```python
api.get_accounts_trades(address)
```

### get_assets
The endpoint is used to get the list of available assets.

Ex:
```python
api.get_assets()
```


### get_assets_symbol
| Parameter | Information |
|---------|-------------|
| symbol | symbol |

Ex:
```python
api.get_assets_symbol(symbol)
```


### get_gcko_pairs
Provides a summary on trading pairs available to CoinGecko.

Ex:
```python
api.get_gcko_pairs()
```


### get_gcko_tickers
Provides 24-hour pricing and volume information on each available market pair to CoinGecko.

Ex:
```python
api.get_gcko_tickers()
```

### get_gcko_trades
The endpoint is used to return data on historical completed trades for a given market pair.

| Parameter | Information |
|---------|-------------|
| ticker_id | id |
| type | buy or sell |
| limit | example: 200 |

Ex:
```python
api.get_gcko_trades(ticker_id, type, limit)
```


### get_jettons_metadata
The endpoint is used to get metadata of the jetton.

| Parameter | Information |
|---------|-------------|
| address | jetton address |

Ex:
```python
api.get_jettons_metadata(address)
```


### get_pools
The endpoint is used to get the list of available pools.

Ex:
```python
api.get_pools()
```


### get_pools_metadata
The endpoint is used to get metadata of the pool.

| Parameter | Information |
|---------|-------------|
| address | pool address |

Ex:
```python
api.get_pools_metadata(address)
```

### get_pools_trades
The endpoint is used to get the list of trades in a pool.

| Parameter | Information |
|---------|-------------|
| address | pool address |

Ex:
```python
api.get_pools_trades(address)
```

### get_prices
The endpoint is used to get the latest price of external assets.

Ex:
```python
api.get_prices()
```

## Methods Tokens()

### get_token_price
| Parameter | Information |
|---------|-------------|
| symbol | token symbol |

Available tokens: AAVE, BTC, DAI, ETH, MATIC, SOL, TON, TRX, TUSD, UNI, USDC, USDT, WBTC, stTON, hTON, wsTON.

Ex:
```python
api.get_token_price('TON')
```