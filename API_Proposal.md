# 3040 Crypto Convertor API

## API description

An API that converts from a crypto from this:

- BitCoin
- Dogecoin.
- American Dollar.
- Canadian Dollar.

## List of endpoints with parameters (see below for requirements)

Endpoints and Parameters: Describe 1-3 endpoints. If you have one endpoint, include at least 3 parameters. If you have two endpoints, include at least 2 parameters. If you have 3 endpoints, include at least 1 parameter.
Note: If you want to keep it simple, these endpoints could all be GET methods.

GET `api/converter`

```JSON
{
    "amount": 1,
    "from": "validCoins",
    "to": "validCoins",
}
```

## Description of resources - formatted as JSON

Resources: one or two resources (think object instance in an object-oriented programming language)

### Bitcoin Resource

```JSON
{
    "type": "bitcoin",
    "id": "1",
    "amount": "1.0",
}
```

### Dogecoin Resource

```JSON
{
    "type": "Dogecoin",
    "id": "2",
    "amount": "1.0",
}
```


## Sample request with sample response
