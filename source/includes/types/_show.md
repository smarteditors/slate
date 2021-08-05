## Get A Specific Type

> `GET https://catalogue.smarteditors.co.uk/api/v6/types/d55010cb-5d05-4749-b6b4-f08070cc21bb`

> Example response

```json
{
  "request_id": "1922c3f4-bf12-407e-adb0-c7d89b7059ae",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "type": {
    "uuid": "19b8af37-6dbc-49c3-9333-6e79b77980b0",
    "archived": false,
    "category_id": "d55010cb-5d05-4749-b6b4-f08070cc21bb",
    "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "cubic_size": 2.0,
    "depreciation_rate": 0.0,
    "depreciation_term": 0,
    "icon_content_type": null,
    "icon_file_name": null,
    "icon_file_size": null,
    "icon_updated_at": null,
    "name": "new chair",
    "slug": null
  },
  "attribute_associations": [
    {
      "uuid": "b345adb5-fa72-409f-9d2c-082c552b21af",
      "_value": [
        "plastic",
        "nylon",
        "wood"
      ],
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
        "nylon",
        "wood"
      ],
      "variable": false
    }
  ]
}
```

This endpoint retrieves a specific Type.

### HTTP Request

`GET https://catalogue.smarteditors.co.uk/api/v6/types/<ID>`
