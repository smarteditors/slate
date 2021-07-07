## Get a Specific Client

> `GET http://localhost:3000/api/v7/clients/38f5d5a1-52e6-4091-b9cf-2d9bc34efc3f`

> Example response

```json
{
  "request_id": "1f6de039-0899-4ac9-bbcc-135e8aeba5a2",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "client": {
    "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "device_limit": null,
    "include_global_itemables": true,
    "logo": {
      "url": null
    },
    "name": "Baumbach LLC",
    "slug": "baumbach-llc"
  }
}
```

This endpoint retrieves a specific client.

### HTTP Request

`GET http://localhost:3000/api/v7/clients/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the Client to retrieve