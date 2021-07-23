## Get A List Of Attributes

> `GET http://localhost:3001/api/v6/attributes`

> Example response

```json
{
  "request_id": "0e1d83ea-3cf7-40f8-8e2f-f8cf0716a292",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "attributes": [
    {
      "uuid": "c4461f7f-0766-4432-9cd3-8954cf3f02b4",
      "field_name": "base_colour",
      "field_type": "colour",
      "field_values": "",
      "name": "base colour"
    },
    {
      "uuid": "201f0912-c111-4b2b-98e7-8fbfef6a976c",
      "field_name": "upholstery_colour",
      "field_type": "colour",
      "field_values": "",
      "name": "upholstery colour"
    },
    {
      "uuid": "43e45bf6-6033-497b-b27f-864d4869a22b",
      "field_name": "upholstery_material",
      "field_type": "multiple_select",
      "field_values": "plastic,nylon,wood",
      "name": "upholstery material"
    }
  ]
}
```

This endpoint retrieves a list of Atrributes for the current client. 

### HTTP Request

`GET http://localhost:3001/api/v6/attributes`
