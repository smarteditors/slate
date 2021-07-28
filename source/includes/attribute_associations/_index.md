## Get All Attribute Associations

> `GET http://localhost:3001/api/v6/attribute_associations`

> Example response ??? attributes duplicated in json

```json
{
  "request_id": "4a4f24cc-2855-4878-aba3-c90d955abd8a",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "attribute_associations": [
    {
      "uuid": "b345adb5-fa72-409f-9d2c-082c552b21af",
      "attribute_id": "43e45bf6-6033-497b-b27f-864d4869a22b",
      "attribute_type": "multiple_select",
      "owner_attribute": {
        "uuid": "43e45bf6-6033-497b-b27f-864d4869a22b",
        "field_name": "upholstery_material",
        "field_type": "multiple_select",
        "field_values": "plastic,nylon,wood",
        "name": "upholstery material"
      },
      "owner_id": "19b8af37-6dbc-49c3-9333-6e79b77980b0",
      "owner_type": "Type",
      "position": 0,
      "required": true,
      "value": [
        "plastic",
        "nylon"
      ],
      "variable": false
    }
  ]
}
```

This endpoint retrieves all Attribute Associations for the current client or for a specified 'owner'. 
Owners can be ???

### HTTP Request

`GET http://localhost:3001/api/v6/attributes`


### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
id | nil | The uuid of the object that owns the Attribute Association | String | No
owner_type | nil | The class of the object that owns the Attribute Association | String | No