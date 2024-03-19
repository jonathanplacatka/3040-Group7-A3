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


## Sample Request For Get Wallet Balence
```json

{
    "userid": "exampleid",
    "password": "exampleuser_password",
    "cryptocurrency": "Bitcoin"
}
```

## Sample Response For Get Wallet Balance
```json

{
  "balance": 5.23,
  "currency": "BTC"
}

```

## Sample Request For Get Cryptocurrency Value

```json

{
  "cryptocurrency": "Bitcoin",
  "outputcurrency": "USD"
}
```

## Sample Response For Get Cryptocurrency value

```json
{
  "value": "62971$"
}
```
