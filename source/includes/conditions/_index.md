## Get All Conditions

```ruby
api = EDi::APIClient
api.conditions
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "good",
    "label": "Good",
    "description": null,
    "uuid": "87808deb-9732-4617-a7fd-7cf12345678",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "client_id": null,
    "colour": null,
    "is_default": false
  },
  {
    "id": 2,
    "name": "fair",
    "label": "Fair",
    "description": null,
    "uuid": "3d24662a-0ecb-4ef0-9b08-21451234567",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "client_id": null,
    "colour": null,
    "is_default": false
  }
]
```

This endpoint retrieves all Asset Conditions.

### HTTP Request

`GET http://localhost:3000/api/v6/meta/conditions`
