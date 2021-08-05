## Set the Current Client

> `PUT https://smartedi2.smarteditors.co.uk/api/v7/clients/set_current_client`

```ruby
example_params = {
  "client_id": Integer
}
```

> Example response

```json
{
  "request_id": "1f6de039-0899-4ac9-bbcc-135e8aeba5a2",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "message": "Client successfully set.",
  "client": {
    "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "device_limit": null,
    "include_global_itemables": true,
    "logo": {
      "url": null
    },
    "name": "Baumbach LLC",
    "slug": "baumbach-llc"
  }
}
```

This endpoint sets the current Client.

### HTTP Request

`PUT https://smartedi2.smarteditors.co.uk/api/v7/clients/set_current_client`

### Query Parameters

Parameter | Default | Description | Required?
--------- | ------- | ----------- | ---------
ID | nil | The uuid of the Client to set | Yes