Not used???

## Search

> `GET http://localhost:3000/api/v7/meta/locations/search`

```ruby
example_params = {
  client_id: Integer,
  store: Boolean,
  from: Integer,
  to: Integer
}
```

> Example response

```json
[
  {
    "id": 8,
    "client_id": 1,
    "parent_id": null,
    "sort_order": null,
    "name": "sc",
    "town": "asc",
    "county": "sac",
    "post_code": "assc",
    "latitude": null,
    "longitude": null,
    "uuid": "f8078fac-6fee-4316-b6f1-e68fa0300905",
    "slug": "sc",
    "created_at": "2021-04-09T14:19:32.000+01:00",
    "updated_at": "2021-04-09T14:19:32.000+01:00",
    "store": false,
    "x": null,
    "y": null,
    "color": null,
    "absolute_path_name": "sc",
    "items_count": 15,
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
    "items_total_count": 14,
    "root": true,
    "child": false,
    "leaf": true,
    "is_store": false,
    "has_children": false,
    "population": [
      {
        "id": 19,
        "code": "0000000213",
        "asset_type": "asset",
        "color": "#000000",
        "x": null,
        "y": null,
        "uuid": "70c86852-36fb-4879-88ed-ff57f29fc492"
      }
    ],
    "address": "sac, asc, asc, sac, assc",
    "floorplan": {
      "id": 5,
      "location_id": 8,
      "folder_id": 8,
      "file": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/5/gg122974214.jpg",
        "thumb": {
          "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/5/thumb_gg122974214_thumb.png"
        },
        "png": {
          "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/5/png_gg122974214_png.png"
        }
      },
      "width": 825,
      "height": 423,
      "main": true,
      "uuid": "254f5675-1ca2-404c-a806-ab7dc2cd868a",
      "created_at": "2021-04-09T16:42:05.000+01:00",
      "updated_at": "2021-04-09T16:42:05.000+01:00",
      "file_tmp": null
    }
  }
]
```

??? Only used in the In Transit part of app. Remove from docs? ???

This endpoint retrieves locations based on search parameters.

### HTTP Request

`GET http://localhost:3000/api/v7/meta/locations/search`

### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
client_id | current client id | A client id, used to return locations linked to a specific client ??? should be uuid ??? | Integer | No
store | nil | If true, returns Store type locations | Boolean | No ??? wrong. if you submit anything it considers it 'true'
from | nil | ??? A location ID (uuid?). Returns transit locations with the origin location specified | Integer | No
to | nil | ??? A location ID (uuid?). Returns transit locations with the destination location specified | Integer | No

??? probably needs changing to check if param == true ??? 