## Validate an Asset code

> `GET http://localhost:3000/api/v6/validate_code`

```ruby
example_params = {
  code: String
}
```

> Example response

```json
{
  "success": true,
  "in_use": false
}
```

Asset codes must be unique. This endpoint checks whether an Asset code is already in use or not.

### HTTP Request

`GET http://localhost:3000/api/v6/validate_code`

### Query Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
code | null | The Asset code to validate, by checking uniqueness | String | Yes  