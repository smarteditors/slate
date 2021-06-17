## Get All Cients

```shell
curl "http://localhost:3000/api/v6/clients" \
  -H "token: meowmeowmeow"
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 6,
    "logo": {
      "url": null
    },
    "name": "Dummy client",
    "slug": "dummy-client",
    "uuid": "38f5d5a1-52e6-4091-b9cf-2d9bc34efc3f",
    "created_at": "2020-11-09T13:09:18.000+00:00",
    "updated_at": "2020-11-09T13:09:18.000+00:00",
    "can_link": false,
    "device_limit": null,
    "reuse_me_email": null,
    "include_global_itemables": true
  }
]
```

This endpoint retrieves all Clients.

### HTTP Request

`GET http://localhost:3000/api/v6/meta/clients`
