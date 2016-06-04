# vf:Stock

Stock can contain 0 or more resources of particular type.

## Object Properties
(relationships)

### vf:contains
relates stock to a resouce it contains

## Examples

### Bicycles

Each bike has an IRI to identify it, and the stock contains many bikes. For example of single bike see [Bike](https://github.com/valueflows/resource/blob/master/Resource.md#bicycle).

```yaml
'@context': https://w3id.org/valueflows/v1
'@id': https://cohouse.example/inventory/bicycles#stock
'@type':
  - vf:Resource
  - prodont:Bicycle
'skos:note': our shared pool of bicycles
'vf:currentLocation': http://sws.geonames.org/2654675/
'vf:quantity':
  '@type': qudt:QuantityValue
  'qudt:unit': unit:Each
  'qudt:numericValue': 4
'vf:contains':
  - https://cohouse.example/inventory/0030b345-c9f9-4e3a-a5a6-b45a8137aa05#resource
  - https://cohouse.example/inventory/49fc39ff-be2b-4653-87ff-b18e2f20063b#resource
  - https://cohouse.example/inventory/a64f0db3-4a62-404e-b46e-4753fb886ea3#resource
  - https://cohouse.example/inventory/40f5148b-710c-4215-ab4d-fee66d8d4f96#resource
```
