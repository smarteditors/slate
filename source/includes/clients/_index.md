## Get All Cients

> `GET https://smartedi2.smarteditors.co.uk/api/v7/clients`

> Example response

```json
{
  "request_id": "1f6de039-0899-4ac9-bbcc-135e8aeba5a2",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "clients": [
    {
      "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "device_limit": null,
      "include_global_itemables": true,
      "logo": {
        "url": null
      },
      "name": "Baumbach LLC",
      "slug": "baumbach-llc"
    }
  ]
}
```

This endpoint retrieves a list of Clients which the current User has access to.

### HTTP Request

`GET https://smartedi2.smarteditors.co.uk/api/v7/clients`
