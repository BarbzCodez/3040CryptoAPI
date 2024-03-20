# 3040 Crypto Convertor API

## API description

An API that converts from one crypto currency to a different currency.

Here is a list of valid currencies:

- BitCoin
- Dogecoin.
- American Dollar.
- Canadian Dollar.

when we refer to a {validCurrency}, it has to be the same as the one on the list

## List of endpoints with parameters (see below for requirements)

> WHICH ONE TO USE

GET `api/convertCurrency/json?from={ValidCoin}&to={ValidCoin}&amount={number}`

## Description of resources - formatted as JSON

### Crypto Currency Resource

The response will have 3 parameters:

- **currency** (string): the name of the currency that you converted had the amount the original amount.
- **amountConverted** (number): with the amount converted  to the currency.

Example:

```JSON
{
    "currency": "DogeCoin",
    "amountConverted": 0.5,
}
```

## Sample request with sample response

The API request looks like this:

GET `api/convertCurrency/json?from=DogeCoin&to=Bitcoin&amount=1`

A successful response looks like this:

```JSON
{
    "amountConverted": 0.5,
    "from": "DogeCoin",
    "to": "Bitcoin",
}
```
