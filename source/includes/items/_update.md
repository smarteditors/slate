## Update An Item

```ruby
example_params = {
  item: {
    location_id: Integer,
    condition_id: Integer,
    status_id: Integer,
    code: String,
    usage: String ['in_use', 'unused'],
    project: Text,
    x: Decimal, 
    y: Decimal,
    purchase_date: Date, 
    purchase_price_cents: Decimal,
    room: String,
    warranty: Integer, 
    warranty_info: Text,
    action_id: Integer,
    installation_date: Date, 
    life_expectancy: Float,
    catalogue_item_id: ???,
    condition_details: String,
    
    photos_attributes: [
      {
        image: String ???
      }
    ],
    
    task_attributes: [ ??? remove? ???
      {
        completed: Boolean,
        completed_date: Date,
        completed_by_id: Integer not present on task?
      }
    ],

    notes_attributes: [
      {
        user_id: Integer,
        body: Text
      }
    ],

    item_attributes_attributes: [
      {
        catalogue_association_id: Integer,
        catalogue_attribute_id: Integer,
        catalogue_attribute_name: String,
        catalogue_attribute_type: String,
        value: Text
      }
    ],

    stamps_attributes: [
      {
        action_stamp: Integer,
        wear_off_date: Date,
        purchase_price_cents: Integer
      }
    ]
  }
}
```

> Example response

```json
{
  "item": {
    "id": 22,
    "client_id": 1,
    "condition_id": 3,
    "status_id": 23,
    "code": "0000123456",
    "usage": "unused",
    "project": "sdd",
    "catalogue_item_id": "1",
    "slug": "21ssdcds3",
    "uuid": "53cf8995-8d85-4339-a522-553bb2426069",
    "created_at": "2021-05-25T16:30:08.000+01:00",
    "updated_at": "2021-06-17T16:25:38.000+01:00",
    "location_id": 8,
    "x": null,
    "y": null,
    "actions": [
      {
        "status": "created",
        "date": "2021-05-25T16:30:08.000+01:00",
        "location": "5509613e-ee0e-403e-9de9-dc9f500c3dd3"
      }
    ],
    "warranty": 15,
    "warranty_info": "fsd",
    "purchase_price_cents": 123,
    "purchase_price_currency": "£",
    "purchase_date": "2021-06-08T00:00:00.000+01:00",
    "action_id": 4,
    "action_date": "2021-06-04T00:00:00.000+01:00",
    "room": "new",
    "colour": "#000000",
    "reuse_action_id": null,
    "stamps_count": 16,
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
      "id": 8,
      "client_id": 1,
      "parent_id": null,
      "sort_order": null,
      "name": "sc",
      "address_one": "sac",
      "address_two": "asc",
      "address_three": null,
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
      "decorate": {
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
    "task_items": [
      {
        "id": 2,
        "task_id": 1,
        "item_id": 22,
        "completed_by_id": null,
        "uuid": "63f40cee-7925-431f-b9d0-05ca1d860d69",
        "completed": null,
        "completed_date": null,
        "created_at": "2021-06-17T15:22:27.000+01:00",
        "updated_at": "2021-06-17T15:22:27.000+01:00",
        "task": {
          "id": 1,
          "assigned_to_id": 2,
          "assigned_by_id": 2,
          "uuid": "87832ba2-2dda-4933-a69c-edc5889e1bed",
          "description": "here is a work request",
          "scheduled_date": "2021-06-16T00:00:00.000+01:00",
          "created_at": "2021-06-17T15:22:27.000+01:00",
          "updated_at": "2021-06-17T15:22:27.000+01:00",
          "completed": null,
          "due_date": "2021-06-18T00:00:00.000+01:00",
          "draft": false,
          "reviewer_id": 2,
          "client_id": 1
        }
      }
    ],
    "item_attributes": [],
    "stamps": [
      {
        "id": 647,
        "item_id": 22,
        "location_id": 8,
        "status_id": 23,
        "previous_location_id": null,
        "purchase_price_cents": 200,
        "purchase_price_currency": "GBP",
        "action_stamp": "estate_reused",
        "action_stamp_type": 0,
        "wear_off_date": "2021-09-07T01:00:00.000+01:00",
        "uuid": "06b558a3-02c3-4dae-8ab7-4abfd42cf054",
        "created_at": "2021-06-07T10:48:56.000+01:00",
        "updated_at": "2021-06-07T10:48:56.000+01:00"
      }
    ],
    "color": "#000000"
  },
  "status": "updated"
}
```

This endpoint updates a specific Item.

### HTTP Request

`PUT http://localhost:3000/api/v6/items/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the Item to update



??? Copy paramaeters from create file, or share file ???