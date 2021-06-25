## Get a Specific Location

> `GET http://localhost:3000/api/v6/locations/7dd46282-929f-4899-bb71-141d8c688454`

> Example response

```json
{
  "id": 6,
  "client_id": 7,
  "parent_id": null,
  "sort_order": null,
  "name": "test",
  "address_one": "riverlea",
  "address_two": "pool road",
  "address_three": null,
  "town": "newtown",
  "county": "powys",
  "post_code": "SY16 3AN",
  "latitude": null,
  "longitude": null,
  "uuid": "7dd46282-929f-4899-bb71-141d8c688454",
  "slug": "test-7f8fff95-fc9b-461b-b0be-1bf35424c67d",
  "created_at": "2021-01-07T13:19:52.000+00:00",
  "updated_at": "2021-01-07T13:19:52.000+00:00",
  "store": true,
  "x": null,
  "y": null,
  "color": null,
  "absolute_path_name": "test",
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
  "has_children": false,
  "floorplan": {
    "id": 3,
    "location_id": 6,
    "folder_id": 6,
    "file": {
      "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/3/floorplan.png",
      "thumb": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/3/thumb_floorplan_thumb.png"
      },
      "png": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/3/png_floorplan_png.png"
      }
    },
    "width": 400,
    "height": 310,
    "main": true,
    "uuid": "ae4ac21e-51e2-4319-8c38-b89544f42bc4",
    "created_at": "2021-01-07T13:19:52.000+00:00",
    "updated_at": "2021-01-07T13:19:52.000+00:00",
    "file_tmp": null
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
