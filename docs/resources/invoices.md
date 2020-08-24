# Invoices Resources
This document describes basic information about invoice resources

### Create Invoice
Returns status HTTP "201 Created"

POST /invoices

```json
{
  "number": 102034,
  "model": "1",
  "serie": "D-1",
  "cfop": "60487",
  "invoice_at": "2019-05-23T00:00:00+04:00",
  "amount": 1.00
}
```

### Update Invoice
Returns status HTTP "200 OK"

PUT /invoices/:id

```json
{
  "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
  "number": 102034,
  "model": "1",
  "serie": "D-1",
  "cfop": "60487",
  "invoice_at": "2019-05-23T00:00:00+04:00",
  "amount": 1.00
}
```

### List all Invoices with Items, if it exists
Returns status HTTP "200 OK"

GET /invoices

```json
[
  {
    "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
    "number": 102034,
    "model": "1",
    "serie": "D-1",
    "cfop": "60487",
    "invoice_at": "2019-05-23T00:00:00+04:00",
    "amount": 1.00,
    "items": [
       {
         "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
         "quantity": 12,
         "amount": 100.00,
         "unit_measure": "UN",
         "description": "Explosive Tennis Balls"
       }
    ]
  }
]
```

### List Invoice by Id, if it exists

Returns status HTTP "200 OK" or status HTTP "204 No Content"

GET /invoices/:id

```json
{
  "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
  "number": 102034,
  "model": "1",
  "situation": "00",
  "serie": "D-1",
  "cfop": "60487",
  "invoice_at": "2019-05-23T00:00:00+04:00",
  "amount": 1.00,
  "items": [
     {
       "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
       "quantity": 12,
       "amount": 100.00,
       "unit_measure": "UN",
       "description": "Explosive Tennis Balls"
     }
  ]
}
```

### List Items by Invoice Id
Returns status HTTP "200 OK" or status HTTP "204 No Content"

GET /invoices/:id/items

```json
[
  {
    "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
    "quantity": 12,
    "amount": 100.00,
    "unit_measure": "UN",
    "description": "Explosive Tennis Balls",
  }
]
```
