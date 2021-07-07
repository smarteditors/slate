## Get All Statuses

> `GET http://localhost:3000/api/v7/statuses`

> Example response

```json
{
  "request_id": "3c8b796e-3926-4a0e-8d66-846240908eb8",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "statuses": [
    {
      "uuid": "44f6ff1a-5dd0-43b7-a618-6be681cdb9cc",
      "archivable": false,
      "client_id": null,
      "description": null,
      "height": null,
      "icon": {
        "url": null
      },
      "icon_family": null,
      "icon_name": null,
      "is_default": false,
      "label": "Marked for Regeneration",
      "name": "marked_regeneration",
      "reportable": true,
      "reprocessable": false,
      "reusable": false,
      "status_type": null,
      "width": null
    }
  ]
}
```

This endpoint retrieves all available item Statuses.

### HTTP Request

`GET http://localhost:3000/api/v7/statuses`
