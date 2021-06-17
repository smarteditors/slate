## Set the Current Client

```shell
curl -X PUT -H "Content-Type: application/json" -d '{"id":"6"}' \
  "http://localhost:3000/api/v6/clients/set_current_client" \
  -H "Authorization: meowmeowmeow"
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