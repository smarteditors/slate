## Get All Statuses

> `GET http://localhost:3000/api/v6/statuses`

> Example response

```json
[
  {
    "uuid": "44f6ff1a-5dd0-43b7-a618-6be681cdb9cc",
    "name": "marked_regeneration",
    "label": "Marked for Regeneration",
    "description": null,
    "status_type": null,
    "reportable": true,
    "reprocessable": false,
    "archivable": false,
    "icon_name": null,
    "icon_family": null,
    "width": null,
    "height": null,
    "client_id": null,
    "is_default": false,
    "reusable": false,
    "icon": {
        "url": null
    }
  }
]
```

This endpoint retrieves all available item Statuses.

### HTTP Request

`GET http://localhost:3000/api/v6/statuses`
