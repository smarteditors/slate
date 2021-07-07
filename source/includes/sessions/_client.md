## Client

> `GET http://localhost:3000/api/v7/sessions/client`

> Example response

```json
{
  "request_id": "513bb3be-31d1-466a-a751-3dff9047601b",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "client": {
    "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "can_link": false,
    "device_limit": null,
    "include_global_itemables": true,
    "logo": {
      "url": null
    },
    "name": "Baumbach LLC",
    "reuse_me_email": null,
    "slug": "baumbach-llc"
  }
}
```

This endpoint returns the current Client.

### HTTP Request

`GET http://localhost:3000/api/v7/sessions/client`
