## Client

> `GET http://localhost:3000/api/v6/sessions/client`

> Example response

```json
{
  "success": true,
  "client": {
    "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "name": "Baumbach LLC",
    "slug": "baumbach-llc",
    "can_link": false,
    "device_limit": null,
    "reuse_me_email": null,
    "include_global_itemables": true,
    "logo": {
        "url": null
    }
  },
  "status": 200
}
```

This endpoint returns the current Client.

### HTTP Request

`GET http://localhost:3000/api/v6/sessions/client`
