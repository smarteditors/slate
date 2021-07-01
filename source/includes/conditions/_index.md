## Get All Conditions

> `GET http://localhost:3000/api/v6/meta/conditions`

> Example response

```json
[
  {
    "uuid": "87808deb-9732-4617-a7fd-7cf12345678",
    "name": "good",
    "label": "Good",
    "description": null,
    "colour": null,
    "is_default": false
  },
  {
    "uuid": "3d24662a-0ecb-4ef0-9b08-21451234567",
    "name": "fair",
    "label": "Fair",
    "description": null,
    "client_id": null,
    "colour": null,
    "is_default": false
  }
]
```

This endpoint retrieves all Item Conditions.

### HTTP Request

`GET http://localhost:3000/api/v6/meta/conditions`
