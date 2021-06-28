## Set the Current Client

> `PUT http://localhost:3000/api/v6/clients/set_current_client`

```ruby
example_params = {
  "client_id": Integer
}
```

> Example response

```json
{
    "success": true,
    "message": "success",
    "status": "ok"
}
```

This endpoint sets the current Client.

??? currenlty possible to select clients the user isn't linked to ???

### HTTP Request

`PUT http://localhost:3000/api/v6/clients/set_current_client`

### Query Parameters

Parameter | Default | Description | Required?
--------- | ------- | ----------- | ---------
ID | nil | The uuid of the Client to set | Yes