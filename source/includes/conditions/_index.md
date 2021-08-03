## Get All Conditions

> `GET https://smartedi2.smarteditors.co.uk/api/v7/meta/conditions`

> Example response

```json
{
  "request_id": "a6e62255-6675-4bfc-b528-cd60d623beaf",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "conditions": [
    {
      "uuid": "87808deb-9732-4617-a7fd-7cf6cce6dd42",
      "colour": null,
      "description": null,
      "is_default": false,
      "label": "Good",
      "name": "good"
    }
  ]
}
```

This endpoint retrieves all Item Conditions.

### HTTP Request

`GET https://smartedi2.smarteditors.co.uk/api/v7/meta/conditions`
