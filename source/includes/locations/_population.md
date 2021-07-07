## Population

> `GET http://localhost:3000/api/v7/locations/d8531da9-85a3-4c57-9ffc-66f9f24c7a9b/population`

> Example response

```json
{
  "request_id": "49647ac4-84f7-4d6d-bfc1-2171a0c28438",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "items": [
    {
      "uuid": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be",
      "asset_type": null,
      "code": "6e6ce1459d4d78780f88",
      "color": "#000000",
      "x": null,
      "y": null
    },
    {
      "uuid": "168d1e9c-8b0f-4f28-974f-494c92d93405",
      "asset_type": null,
      "code": "39c29f4d7d8fd42c84ee",
      "color": "#000000",
      "x": null,
      "y": null
    }
  ]
}
```

This endpoint retrieves items stored at a specific location.

### HTTP Request

`GET http://localhost:3000/api/v7/locations/<ID>/population`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the location from which to retrieve all items
