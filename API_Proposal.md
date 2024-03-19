# 3040 Crypto Convertor API

## API description

An API that converts from a crypto from this:

- BitCoin
- Dogecoin.
- American Dollar.
- Canadian Dollar.

## List of endpoints with parameters (see below for requirements)

Note: If you want to keep it simple, these endpoints could all be GET methods.

GET `api/convertCurrency/json?from={ValidCoin}&to={ValidCoin}&amount={number}`

## Description of resources - formatted as JSON

Resources: one or two resources (think object instance in an object-oriented programming language)

### Crypto Currency Resource

convertCurrency

```JSON
{
    "type": "string",
    "id": "1",
    "name": "DogeCoin",
    "amount": "1.0",
}
```

## Sample request with sample response

The API request looks like this:

```JSON
GET `api/convertCurrency`

{
    "amount": 1,
    "from": "DogeCoin",
    "to": "Bitcoint",
}
```

A successful response looks like this:

```JSON
{
    "amountConverted": .5,
    "from": "DogeCoin",
    "to": "Bitcoint",
}

```