## Get a Specific Asset

```ruby
api = EDi::APIClient
api.items(75)
```

> The above command returns JSON structured like this:

```json
{
  "id": 75,
  "client_id": 1,
  "condition_id": 3,
  "status_id": 23,
  "code": "000002s1s3",
  "usage": "in_use",
  "project": "sdd",
  "catalogue_item_id": "1",
  "slug": "2s1s3",
  "uuid": "fd4e6d48-db9a-4804-ab59-07cb438b65a8",
  "created_at": "2021-05-28T10:52:04.000+01:00",
  "updated_at": "2021-06-04T12:14:25.000+01:00",
  "location_id": 1,
  "x": null,
  "y": null,
  "actions": [
    {
      "status": "44f6ff1a-5dd0-43b7-a618-6be681cdb9cc",
      "date": "2021-05-28T10:52:04.265+01:00",
      "location": "5509613e-ee0e-403e-9de9-dc9f500c3dd3"
    }
  ],
  "warranty": 15,
  "warranty_info": "vjk",
  "purchase_price_cents": 123,
  "purchase_price_currency": "£",
  "purchase_date": "2021-06-08T00:00:00.000+01:00",
  "action_id": 4,
  "action_date": "2021-06-04T00:00:00.000+01:00",
  "room": "new",
  "colour": "#000000",
  "reuse_action_id": null,
  "stamps_count": 11,
  "item_attributes_count": 0,
  "in_storage": false,
  "sale_price": 120.0,
  "installation_date": null,
  "life_expectancy": 0.0,
  "asset_type": "asset",
  "condition_details": null,
  "pre_charged_for_disposal": false,
  "catalogue_item": {
    "id": 1,
    "name": "style 1",
    "status": "awaiting_decision",
    "code": "dvs",
    "confirmed": true,
    "embedded_co2": null,
    "weight": null,
    "uuid": "7e9fe938-f2db-4cd5-8259-f22db5806a9c",
    "description": "",
    "sales_reference": "S000001",
    "price_as_new": null,
    "snd_min_price": null,
    "snd_max_price": null,
    "used_for": [],
    "sfg": "dsv",
    "photo": "https://s3-eu-west-1.amazonaws.com/sassy-catalogue-development/items/photos/000/000/001/original/test2.jpeg?1621954031",
    "display_status": "Awaiting Decision",
    "term": 0,
    "rate": 0.0,
    "cubic": 0.01,
    "catalogue": {
      "id": 7,
      "name": "test"
    },
    "category": {
      "id": 3,
      "name": "test 1",
      "colour": "#000000"
    },
    "type": {
      "id": 2,
      "name": "type 1"
    },
    "store_me_group_limits": [],
    "attribute_associations": [],
    "components": []
  },
  "photo": null,
  "years_remaining": 0,
  "photo_url": null,
  "photo_large_url": null,
  "archiveds": false,
  "client": {
    "id": 1,
    "logo": {
      "url": null
    },
    "name": "Baumbach LLC",
    "slug": "baumbach-llc",
    "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "created_at": "2020-11-09T13:08:37.000+00:00",
    "updated_at": "2020-11-09T13:08:37.000+00:00",
    "can_link": false,
    "device_limit": null,
    "reuse_me_email": null,
    "include_global_itemables": true
  },
  "location": {
    "id": 1,
    "client_id": 7,
    "parent_id": null,
    "sort_order": null,
    "name": "sergio marrocoli",
    "address_one": "riverlea",
    "address_two": "pool road",
    "address_three": null,
    "town": "newtown",
    "county": "powys",
    "post_code": "SY16 3AN",
    "latitude": null,
    "longitude": null,
    "uuid": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
    "slug": "sergio-marrocoli",
    "created_at": "2021-01-05T12:56:14.000+00:00",
    "updated_at": "2021-01-05T12:56:14.000+00:00",
    "store": false,
    "x": null,
    "y": null,
    "color": null,
    "absolute_path_name": "sergio marrocoli",
    "items_count": 36,
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
    "items_total_count": 51,
    "decorate": {
      "id": 1,
      "client_id": 7,
      "parent_id": null,
      "sort_order": null,
      "name": "sergio marrocoli",
      "town": "newtown",
      "county": "powys",
      "post_code": "SY16 3AN",
      "latitude": null,
      "longitude": null,
      "uuid": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
      "slug": "sergio-marrocoli",
      "created_at": "2021-01-05T12:56:14.000+00:00",
      "updated_at": "2021-01-05T12:56:14.000+00:00",
      "store": false,
      "x": null,
      "y": null,
      "color": null,
      "absolute_path_name": "sergio marrocoli",
      "items_count": 36,
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
      "items_total_count": 51,
      "root": true,
      "child": false,
      "leaf": true,
      "is_store": false,
      "has_children": false,
      "population": [
        {
          "id": 27,
          "code": "6e6ce1459d4d78780f88",
          "asset_type": "asset",
          "color": "#000000",
          "x": null,
          "y": null,
          "uuid": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be"
        }
      ],
      "address": "riverlea, pool road, newtown, powys, SY16 3AN",
      "floorplan": {
        "id": 1,
        "location_id": 1,
        "folder_id": 1,
        "file": {
          "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/1/Screenshot_from_2020-11-26_12-44-29.png",
          "thumb": {
            "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/1/thumb_Screenshot_from_2020-11-26_12-44-29_thumb.png"
          },
          "png": {
            "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/floorplan/file/1/png_Screenshot_from_2020-11-26_12-44-29_png.png"
          }
        },
        "width": 3840,
        "height": 1080,
        "main": true,
        "uuid": "17373e48-addf-4d81-a090-3b350c2d8641",
        "created_at": "2021-01-05T12:56:14.000+00:00",
        "updated_at": "2021-01-05T12:56:14.000+00:00",
        "file_tmp": null
      }
    }
  },
  "condition": {
    "id": 3,
    "name": "poor",
    "label": "Poor",
    "description": null,
    "uuid": "cb274607-0af0-40a1-96c9-3324d0639982",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "client_id": null,
    "colour": null,
    "is_default": false
  },
  "status": {
    "id": 23,
    "name": "waiting_regeneration",
    "label": "Awaiting Regeneration",
    "description": null,
    "status_type": null,
    "uuid": "69bd2c6f-7311-421c-b956-4c55955ebe63",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "reportable": true,
    "reprocessable": false,
    "archivable": false,
    "icon_name": null,
    "icon_family": null,
    "icon": {
      "url": null
    },
    "width": null,
    "height": null,
    "client_id": null,
    "is_default": false,
    "reusable": false
  },
  "action": {
    "id": 4,
    "name": "assess",
    "label": "Assess",
    "description": null,
    "uuid": "ca72f768-0f94-4536-9a51-90b5891df4a7",
    "created_at": "2020-11-09T13:08:36.000+00:00",
    "updated_at": "2020-11-09T13:08:36.000+00:00",
    "client_id": null
  },
  "notes": [],
  "task_items": [],
  "item_attributes": [],
  "stamps": [
    {
      "id": 54,
      "item_id": 75,
      "location_id": 1,
      "status_id": 22,
      "previous_location_id": null,
      "purchase_price_cents": null,
      "purchase_price_currency": "GBP",
      "action_stamp": "estate_reused_and_refreshed",
      "action_stamp_type": 0,
      "wear_off_date": "2021-09-01T01:00:00.000+01:00",
      "uuid": "09d38fc0-8669-4b42-a263-b57c59f4c056",
      "created_at": "2021-06-01T09:17:56.000+01:00",
      "updated_at": "2021-06-01T09:17:56.000+01:00"
    }
  ],
  "color": "#000000"
}
```

This endpoint retrieves a specific asset.

### HTTP Request

`GET http://localhost:3000/api/v6/items/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the Asset to retrieve
