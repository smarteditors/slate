## Get All Cients

> `GET http://localhost:3000/api/v6/clients`

> Example response

```json
[
  {
    "uuid": "38f5d5a1-52e6-4091-b9cf-2d9bc34efc3f",
    "name": "Dummy client",
    "slug": "dummy-client",
    "can_link": false,
    "device_limit": null,
    "reuse_me_email": null,
    "include_global_itemables": true,
    "logo": {
      "url": null
    }
  }
]
```

This endpoint retrieves all Clients for the current user.

### HTTP Request

`GET http://localhost:3000/api/v6/clients`
