## Set the Current Client

```ruby
params = {
  client_id: Integer
}

api = EDi::APIClient
api.clients.set_current_client(params)
```

> The above command returns JSON structured like this:

```json
{
    "success": true,
    "message": "success",
    "status": "ok"
}
```

This endpoint changes the client.

### HTTP Request

`PUT http://localhost:3000/api/v6/clients/set_current_client`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
ID | null | The ID of the client to you want to switch to