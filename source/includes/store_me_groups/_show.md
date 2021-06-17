## Get a Specific Store Me Group

```shell
curl "http://localhost:3000/api/v6/store_more_groups" \
  -H "token: meowmeowmeow"
```

> The above command returns JSON structured like this:

```json
{
  "id": 22,
  "client_id": 1,
  "parent_id": 1,
  "sort_order": null,
  "name": "s",
  "town": "esf",
  "county": "esf",
  "post_code": "ffff",
  "latitude": null,
  "longitude": null,
  "uuid": "d8531da9-85a3-4c57-9ffc-66f9f24c7a9b",
  "slug": "s",
  "created_at": "2021-04-09T16:42:51.000+01:00",
  "updated_at": "2021-06-17T14:00:53.000+01:00",
  "store": true,
  "x": null,
  "y": null,
  "color": null,
  "absolute_path_name": "sergio marrocoli -> s",
  "items_count": null,
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
  "root": false,
  "child": true,
  "leaf": true,
  "is_store": false,
  "has_children": false,
  "population": [],
  "address": "sdfefs, esf, esf, esf, ffff",
  "floorplan": {
    "id": 6,
    "location_id": 22,
    "folder_id": 22,
    "file": {
      "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/6/20210217_081919.jpg",
      "thumb": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/6/thumb_20210217_081919_thumb.png"
      },
      "png": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/6/png_20210217_081919_png.png"
      }
    },
    "width": 3264,
    "height": 2448,
    "main": true,
    "uuid": "a8e2eacb-9d4b-456a-a101-f19fc0fa53fd",
    "created_at": "2021-04-09T16:42:51.000+01:00",
    "updated_at": "2021-04-09T16:42:51.000+01:00",
    "file_tmp": null
  },
  "items": [],
  "children": []
}
```

This endpoint retrieves a Store Me Group for ????

### HTTP Request

`GET http://localhost:3000/api/v6/store_me_groups/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the location to retrieve

### Query Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | -------- | -------
store_me_group_id | nil | ??? | int | true |