## Get All Statuses

```ruby
api = EDi::APIClient
api.statuses
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "marked_regeneration",
    "label": "Marked for Regeneration",
    "description": null,
    "status_type": null,
    "uuid": "44f6ff1a-5dd0-43b7-a618-6be681cdb9cc",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "reportable": true,
    "reprocessable": false,
    "archivable": false,
    "icon_name": null,
    "icon_family": null,
    "icon": {
        "url": null
    },
    "width": null,
    "height": null,
    "client_id": null,
    "is_default": false,
    "reusable": false
  }
]
```

This endpoint retrieves all Statuses for the current Client.

### HTTP Request

`GET http://localhost:3000/api/v6/statuses`
