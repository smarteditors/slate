## Get a Specific Location

> `GET http://localhost:3000/api/v6/locations/7dd46282-929f-4899-bb71-141d8c688454`

> Example response

```json
{
  "uuid": "7dd46282-929f-4899-bb71-141d8c688454",
  "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
  "parent_id": null,
  "sort_order": null,
  "name": "a location",
  "address_one": "a house",
  "address_two": "a street",
  "address_three": null,
  "town": "a town",
  "county": "a county",
  "post_code": "postcode",
  "latitude": null,
  "longitude": null,
  "slug": "test-7f8fff95-fc9b-461b-b0be-1bf35424c67d",
  "store": true,
  "x": null,
  "y": null,
  "color": null,
  "absolute_path_name": "",
  "items_count": 2,
  "transit": false,
  "from_location_uuid": null,
  "to_location_uuid": null,
  "transit_info": null,
  "archived": false,
  "levels": null,
  "stacked_level": null,
  "cubic_capacity": 0.0,
  "sub_location_type": null,
  "storage_type_id": null,
  "previous_location_id": null,
  "_store_me_groups_for_transit": null,
  "items_total_count": 0,
  "address": "full address",
  "has_children": false,
  "floorplan": {
    "uuid": "17373e48-addf-4d81-a090-3b350c2d8641",
    "folder_id": 6,
    "width": 400,
    "height": 310,
    "main": true,
    "file_tmp": null,
    "file": {
      "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/3/floorplan.png",
      "thumb": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/3/thumb_floorplan_thumb.png"
      },
      "png": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/3/png_floorplan_png.png"
      }
    }
  }
}
```

This endpoint retrieves a specific location.


### HTTP Request

`GET http://localhost:3000/api/v6/locations/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the location to retrieve
