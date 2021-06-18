## Get Store Me Groups

```ruby
params = {
  client_id: Integer
}

api = EDi::APIClient
api.store_me_groups(params)
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": "ccca3584-ddeb-4a57-8e41-344a2efaff58",
    "name": "test",
    "client": "Baumbach LLC",
    "stores": [
      {
        "id": "a26a0c1a-6625-4497-93c4-de2a73885022",
        "name": "and again"
      },
      {
        "id": "d8531da9-85a3-4c57-9ffc-66f9f24c7a9b",
        "name": "s"
      }
    ]
  }
]
```

This endpoint retrieves all Store Me Groups for the current client.

### HTTP Request

`GET http://localhost:3000/api/v6/store_me_groups`

### Query Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | -------- | -------
client_id | current client id | Return Store Me Groups linked to a specific client | int | false