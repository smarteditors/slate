## Get All Actions

> `GET http://localhost:3000/api/v7/meta/actions`

> Example response

```json
[
  {
    "id": 1,
    "name": "regenerate",
    "label": "Regenerate",
    "description": null,
    "uuid": "91e8f48c-bee6-41d8-b451-73b94b8d6342",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "client_id": null
  },
  {
    "id": 2,
    "name": "sales_donation_window",
    "label": "Sales/Donation Window",
    "description": null,
    "uuid": "2fe56353-34dd-4274-aa71-ef9c5729c653",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "client_id": null
  }
]
```

This endpoint retrieves all Actions.

??? explain what actions are ???

### HTTP Request

`GET http://localhost:3000/api/v7/meta/actions`
