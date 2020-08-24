# Invoices Items Resources
This document describes basic information about invoice items resources

### Create Items
Returns status HTTP "201 Created"

POST /invoices/:id/items

```json
{
  "quantity": 12,
  "amount": 100.00,
  "unit_measure": "UN",
  "description": "Explosive Tennis Balls"
}
```

### Create Items
Returns status HTTP "200 OK" 

POST /invoices/:id/items

```json
[
  {
    "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
    "quantity": 12,
    "amount": 100.00,
    "unit_measure": "UN",
    "description": "Explosive Tennis Balls"
  }
]
```
### Update Item
Returns status HTTP "200 OK"

PUT /invoices/:id/items/:id

```json
{
  "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
  "quantity": 12,
  "amount": 100.00,
  "unit_measure": "UN",
  "description": "Explosive Tennis Balls"
}
```

### List all Item
Returns status HTTP "200 OK" 

GET /invoices/:id/items

```json
[
  {
    "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
    "quantity": 12,
    "amount": 100.00,
    "unit_measure": "UN",
    "description": "Explosive Tennis Balls"
  }
]
```

### List Item by Id
Returns status HTTP "200 OK" or status HTTP "204 No Content"

GET /invoices/:id/items/:id

```json
{
  "id": "f54f6088-d7b1-43be-b0a3-cf6b00b9bc7f",
  "quantity": 12,
  "amount": 100.00,
  "unit_measure": "UN",
  "description": "Explosive Tennis Balls"
}
```