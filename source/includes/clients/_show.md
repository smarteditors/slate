## Get a Specific Client

> `GET http://localhost:3000/api/v6/clients/38f5d5a1-52e6-4091-b9cf-2d9bc34efc3f`

> Example response

```json
{
  "name": "Dummy client",
  "slug": "dummy-client",
  "uuid": "38f5d5a1-52e6-4091-b9cf-2d9bc34efc3f",
  "can_link": false,
  "device_limit": null,
  "reuse_me_email": null,
  "include_global_itemables": true,
  "logo": {
    "url": null
  }
}
```

This endpoint retrieves a specific client.

### HTTP Request

`GET http://localhost:3000/api/v6/clients/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the Client to retrieve