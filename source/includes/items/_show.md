## Get A Specific Item

> `GET http://localhost:3000/api/v6/items/fd4e6d48-db9a-4804-ab59-07cb438b65a8`

> Example response

```json
{
  "uuid": "fd4e6d48-db9a-4804-ab59-07cb438b65a8",
  "client_id": "4a36e9e7-c762-4c5e-a6ac-1ff15554d485",
  "condition_id": "cb274607-0af0-40a1-96c9-3324d0639982",
  "status_id": "69bd2c6f-7311-421c-b956-4c55955ebe63",
  "location_id": "d8531da9-85a3-4c57-9ffc-66f9f24c7a9b",
  "catalogue_item_id": "7e9fe938-f2db-4cd5-8259-f22db5806a9c",
  "action_id": "ca72f768-0f94-4536-9a51-90b5891df4a7",
  "reuse_action_id": null,
  "code": "000002s1s3",
  "usage": "in_use",
  "project": "sdd",
  "slug": "2s1s3",
  "x": null,
  "y": null,
  "warranty": 15,
  "warranty_info": "warranty info text",
  "purchase_price_cents": 123,
  "purchase_price_currency": "£",
  "purchase_date": "2021-06-08T00:00:00.000+01:00",
  "action_date": "2021-06-04T00:00:00.000+01:00",
  "room": "new",
  "colour": "#000000",
  "color": "#000000",
  "stamps_count": 11,
  "item_attributes_count": 0,
  "in_storage": false,
  "sale_price": 120.0,
  "installation_date": null,
  "life_expectancy": 0.0,
  "asset_type": "asset",
  "condition_details": null,
  "pre_charged_for_disposal": false,
  "photo": null,
  "years_remaining": 0,
  "photo_url": null,
  "photo_large_url": null,
  "archiveds": false,
  "actions": [
    {
      "status": "44f6ff1a-5dd0-43b7-a618-6be681cdb9cc",
      "date": "2021-05-28T10:52:04.265+01:00",
      "location": "5509613e-ee0e-403e-9de9-dc9f500c3dd3"
    }
  ],
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
  "client": {
    "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "name": "Baumbach LLC",
    "slug": "baumbach-llc",
    "can_link": false,
    "device_limit": null,
    "reuse_me_email": null,
    "include_global_itemables": true,
    "logo": {
      "url": null
    }
  },
  "location": {
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
  },
  "condition": {
    "uuid": "cb274607-0af0-40a1-96c9-3324d0639982",
    "name": "poor",
    "label": "Poor",
    "description": null,
    "colour": null,
    "is_default": false
  },
  "status": {
    "uuid": "69bd2c6f-7311-421c-b956-4c55955ebe63",
    "name": "waiting_regeneration",
    "label": "Awaiting Regeneration",
    "description": null,
    "status_type": null,
    "reportable": true,
    "reprocessable": false,
    "archivable": false,
    "icon_name": null,
    "icon_family": null,
    "width": null,
    "height": null,
    "client_id": null,
    "is_default": false,
    "reusable": false,
    "icon": {
      "url": null
    }
  },
  "notes": [
    {
      "uuid": "f5b5d194-1608-401d-8f48-79979e3016b1",
      "item_id": "3b287f98-d824-4727-8c20-1128ee099d91",
      "user_id": "8daf62d3-f86e-47bf-9c39-d7cb6babd0b5",
      "body": "new note",
      "note_type": null,
      "created_at": "2021-06-09T14:15:30.000+01:00",
      "updated_at": "2021-06-30T12:17:43.000+01:00"
    }
  ],
  "task_items": [],
  "item_attributes": [],
  "stamps": [
    {
      "uuid": "09d38fc0-8669-4b42-a263-b57c59f4c056",
      "item_id": "70c86852-36fb-4879-88ed-ff57f29fc492",
      "location_id": "f8078fac-6fee-4316-b6f1-e68fa0300905",
      "status_id": "a8ee8239-dc47-4af1-8ae7-faa928d62fac",
      "previous_location_id": null,
      "purchase_price_cents": null,
      "purchase_price_currency": "GBP",
      "action_stamp": "estate_reused_and_refreshed",
      "action_stamp_type": 0,
      "wear_off_date": "2021-09-01T01:00:00.000+01:00",
      "created_at": "2021-06-01T09:17:56.000+01:00"
    }
  ]
}
```

This endpoint retrieves a specific item.

### HTTP Request

`GET http://localhost:3000/api/v6/items/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the Item to retrieve
