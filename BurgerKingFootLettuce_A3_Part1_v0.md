# 3040 Crypto Convertor API

## API Description

This document describes an API that converts one type of currency to a different type of currency. It includes a single GET endpoint that requires 3 parameters. These parameters are the currency that is being converted to and from, and also the amount of currency that is being converted. This API will return a JSON formatted string that includes the converted currency value, and also the to and from parameters.

Below is a list of supported currencies that can be used as the **to** and **from** parameters:

- 3040Coin.
- BitCoin.
- DogeCoin.
- American Dollar.
- Canadian Dollar.

> When we refer to a {validCurrency}, it has to be the same as one of the items in the list

## List of Endpoints with Parameters

### convertCurrency Endpoint

GET `convertCurrency?from={validCurrency}&to={validCurrency}&amount={number}`

The parameters are:

- **from**: must be a string of type {validCurrency}.
- **to**: must be a string of type {validCurrency}.
- **amount**: must be number.

## Description of Resources - formatted as JSON

### convertCurrency Resource

The response will have 3 parameters:

- **amountConverted** (number): The value of the currency after it has been converted to the currency of the *to* parameter.
- **from** (string): The currency type that is being converted. This will be a {validCurrency} type.
- **to** (string): The currency type that the *from* parameter is being converted into. This will be a {validCurrency} type.

Example:

```JSON
{
    "amountConverted": 2,
    "from": "3040Coin",
    "to": "Bitcoin",
}
```

## Sample Request and Response

The API request looks like this:

GET `convertCurrency?from=DogeCoin&to=Bitcoin&amount=1`

A successful response looks like this:

```JSON
{
    "amountConverted": 0.5,
    "from": "DogeCoin",
    "to": "Bitcoin",
}
```
