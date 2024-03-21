# 3040Crypto API

## API Description
The API provides endpoints to retrieve information related to cryptocurrency, including wallet balances and current cryptocurrency values. Users can access their wallet balances and obtain real-time information about the value of various cryptocurrencies.

## List of Endpoints with Parameters

### 1. Get Wallet Balance
- **Endpoint**: `/wallet/balance`
- **Parameters**:
  - `userid` (string): The unique identifier of the user's account.
  - `password` (string): The password associated with the user's account.  
  - `currency_name` (string): The name of the cryptocurrency to retrieve the value for.

### 2. Get Cryptocurrency Value
- **Endpoint**: `/crypto/value`
- **Parameters**:
  - `currency_name` (string): The name of the cryptocurrency to retrieve the value for.
  - `target_currency` (string): The currency in which the user wants to view the value (e.g., USD, CAD).

## Resources
balance:
```
{
  balance: 0.07
  currency_name: BTC
}
```
value:
```
{
  value: 8240.88
}
```


## Sample Requests/Responses

### Get Wallet Balance Request

```GET /wallet/balance```
```json

{
    "userid": "exampleid",
    "password": "exampleuser_password",
    "cryptocurrency": "Bitcoin"
}
```

### Get Wallet Balance Response

```json

{
  "balance": 5.23,
  "currency": "BTC"
}

```

### Get Cryptocurrency Value Request

```GET /crypto/value```

```json

{
  "cryptocurrency": "Bitcoin",
  "outputcurrency": "USD"
}
```

### Get Cryptocurrency Value Response

```json
{
  "value": "62971.00"
}
```
