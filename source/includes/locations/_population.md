## Population

> `GET http://localhost:3000/api/v6/locations/d8531da9-85a3-4c57-9ffc-66f9f24c7a9b/population`

> Example response

```json
[
  {
    "id": 27,
    "code": "6e6ce1459d4d78780f88",
    "color": "#000000",
    "x": null,
    "y": null,
    "uuid": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be"
  },
  {
    "id": 28,
    "code": "39c29f4d7d8fd42c84ee",
    "color": "#000000",
    "x": null,
    "y": null,
    "uuid": "168d1e9c-8b0f-4f28-974f-494c92d93405"
  }
]
```

This endpoint retrieves items stored at a specific location.

### HTTP Request

`GET http://localhost:3000/api/v6/locations/<ID>/population`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the location from which to retrieve all items
