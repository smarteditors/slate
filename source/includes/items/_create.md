## Create An Item

> `POST http://localhost:3000/api/v6/items`

```ruby
example_example_params = {
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
    "id": 76,
    "client_id": null,
    "condition_id": 3,
    "status_id": 23,
    "code": "0000123asd",
    "usage": "unused",
    "project": null,
    "catalogue_item_id": null,
    "slug": "123asd",
    "uuid": "3b287f98-d824-4727-8c20-1128ee099d91",
    "created_at": "2021-06-18T09:32:31.000+01:00",
    "updated_at": "2021-06-18T09:32:31.000+01:00",
    "location_id": 22,
    "x": null,
    "y": null,
    "actions": [
      {
        "status": "69bd2c6f-7311-421c-b956-4c55955ebe63",
        "date": "2021-06-18T09:32:31.034+01:00",
        "location": "d8531da9-85a3-4c57-9ffc-66f9f24c7a9b"
      },
      {
        "status": "created",
        "date": "2021-06-18T09:32:31.000+01:00",
        "location": "d8531da9-85a3-4c57-9ffc-66f9f24c7a9b"
      }
    ],
    "warranty": null,
    "warranty_info": null,
    "purchase_price_cents": 0,
    "purchase_price_currency": "GBP",
    "purchase_date": null,
    "action_id": null,
    "action_date": null,
    "room": null,
    "colour": null,
    "reuse_action_id": null,
    "stamps_count": 0,
    "item_attributes_count": 0,
    "in_storage": true,
    "sale_price": null,
    "installation_date": null,
    "life_expectancy": 0.0,
    "asset_type": "asset",
    "condition_details": null,
    "pre_charged_for_disposal": false,
    "catalogue_item": null,
    "photo": null,
    "years_remaining": 0,
    "photo_url": null,
    "photo_large_url": null,
    "archiveds": false,
    "location": {
      "id": 22,
      "client_id": 1,
      "parent_id": 1,
      "sort_order": null,
      "name": "s",
      "address_one": "sdfefs",
      "address_two": "esf",
      "address_three": null,
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
      "absolute_path_name": "parent location -> this location",
      "items_count": 1,
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
      "decorate": {
        "id": 22,
        "client_id": 1,
        "parent_id": 1,
        "sort_order": null,
        "name": "this location name",
        "town": "a town",
        "county": "a county",
        "post_code": "postcode",
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
        "absolute_path_name": "parent location name -> this location name",
        "items_count": 1,
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
    "notes": [],
    "task_items": [],
    "item_attributes": [],
    "stamps": []
  },
  "status": "created"
}
```

This endpoint creates a new Item.

### HTTP Request

`POST http://localhost:3000/api/v6/items`

### Item Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
location_id | nil | The ID of the location of the item | Integer | Yes
condition_id | nil | The ID of the item's condition | Integer | Yes | See the Conditions endpoint
status_id | nil | The ID of the item's status | Integer | Yes | See the Statuses endpoint
code | nil | A free text code identifier | String | Yes
usage | nil | Whether the Item is in use or unused | String | Yes | 'in_use', 'unused'
project | nil | A free text project identifier | String | No
x | nil | ??? The x position of the item on its location's floorplan. pixels or 0 to 1? ??? | Decimal | No
y | nil | ??? The y position of the item on its location's floorplan. pixels or 0 to 1? ??? | Decimal | No
purchase_date | nil | The purchase date | Date | No
purchase_price_cents | nil | The purchase price of the item in pence | Decimal | No
room | nil | A free text room identifier | String | No
warranty | nil | The warranty length in years | Integer | No
warranty_info | nil |  | Integer | No
action_id | nil | an Action ID | Integer | No | See the Actions endpoint
installation_date | nil | Installation date | Date | No
life_expectancy | nil | The life expectancy of the item in years | Float | No
catalogue_item_id | nil | ??? | ??? | No
condition_details | nil | ??? Free text ??? | String | No


### Nested Photo Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
image | nil | A photo of the item | ??? | No | ???

<!-- ??? remove ???
### Nested Task Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
completed | nil | Whether the task has been completed | Boolean | Yes |
completed_date | nil | Date the task was completed | Date | No |
completed_by_id | | | | | ??? needs removing from params as attribute doesn't exist on tasks ??? -->

### Nested Notes Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
user_id | nil | The id of a user | Integer | Yes |
body | nil | The note content | Text | No ??? |

### Nested Item Attributes Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
catalogue_association_id | | | | |
catalogue_attribute_id | | | | |
catalogue_attribute_name | | | | |
catalogue_attribute_type | | | | |
value | | | | |

<!-- Remove 
### Nested Stamps Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
action_stamp | nil | The type of stamp | Yes | String | See stamps/index
wear_off_date | nil |  | No | Date |
purchase_price_cents | 0 | ??? | No | Integer |

??? doesn't this need :action_stamp_type? ??? -->