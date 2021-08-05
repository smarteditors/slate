## Validate an Item code

> `GET https://smartedi2.smarteditors.co.uk/api/v7/validate_code`

```ruby
example_params = {
  code: String
}
```

> Example response

```json
{
  "request_id": "bda19bfb-8fdd-4a75-90fd-8dd40a847fc9",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "in_use": false
}
```

Item codes must be unique. This endpoint checks whether an Item code is already in use or not.

### HTTP Request

`GET https://smartedi2.smarteditors.co.uk/api/v7/validate_code`

### Query Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
code | nil | The Item code to validate, by checking uniqueness | String | Yes  