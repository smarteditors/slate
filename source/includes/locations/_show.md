## Get a Specific Location

> `GET https://smartedi2.smarteditors.co.uk/api/v7/locations/7dd46282-929f-4899-bb71-141d8c688454`

> Example response

```json
{
  "request_id": "a5ec265f-44c0-4a64-a619-f3cf494d6faf",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "location": {
    "uuid": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
    "absolute_path_name": "sergio marrocoli",
    "address": "riverlea, pool road, newtown, powys, SY16 3AN",
    "address_one": "riverlea",
    "address_three": null,
    "address_two": "pool road",
    "archived": false,
    "client": {
      "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "name": "Baumbach LLC"
    },
    "color": null,
    "county": "powys",
    "cubic_capacity": 0.0,
    "from_location_uuid": null,
    "items_count": 37,
    "items_total_count": 37,
    "latitude": null,
    "levels": null,
    "longitude": null,
    "name": "sergio marrocoli",
    "parent_id": null,
    "post_code": "SY16 3AN",
    "previous_location_id": null,
    "slug": "sergio-marrocoli",
    "sort_order": null,
    "stacked_level": null,
    "storage_type_id": null,
    "store": false,
    "sub_location_type": null,
    "to_location_uuid": null,
    "town": "newtown",
    "transit": false,
    "transit_info": null,
    "x": null,
    "y": null
  },
  "population": [
    {
      "uuid": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be",
      "asset_type": "asset",
      "code": "6e6ce1459d4d78780f88",
      "color": "#000000",
      "x": null,
      "y": null
    }
  ]
}
```

This endpoint retrieves a specific location.


### HTTP Request

`GET https://smartedi2.smarteditors.co.uk/api/v7/locations/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the location to retrieve
