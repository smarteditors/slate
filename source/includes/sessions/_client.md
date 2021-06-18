## Client

```ruby
api = EDi::APIClient
api.sessions.client
```

> The above command returns JSON structured like this:

```json
{
  "success": true,
  "client": {
    "id": 1,
    "logo": {
        "url": null
    },
    "name": "Baumbach LLC",
    "slug": "baumbach-llc",
    "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "created_at": "2020-11-09T13:08:37.000+00:00",
    "updated_at": "2020-11-09T13:08:37.000+00:00",
    "can_link": false,
    "device_limit": null,
    "reuse_me_email": null,
    "include_global_itemables": true
  },
  "status": 200
}
```

This endpoint returns the current Cslient.

### HTTP Request

`GET http://localhost:3000/api/v6/sessions/client`
