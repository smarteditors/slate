## Validate an Asset code

```ruby
params = {
  code: String
}

api = EDi::APIClient
api.assets.validate_code(params)
```

> The above command returns JSON structured like this:

```json
{
  "success": true,
  "in_use": false
}
```

This endpoint checks whether an Asset code is in use or not.

### HTTP Request

`GET http://localhost:3000/api/v6/validate_code`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
code | null | The Asset code to validate 