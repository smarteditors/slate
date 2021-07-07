## Create An Item

> `POST http://localhost:3000/api/v7/items`

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
        image: String
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
  "request_id": "867fa162-eff8-4fbb-9e3f-6c35d47c9e2d",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "item": {
    "uuid": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be",
    "action_date": "2021-06-04T00:00:00.000+01:00",
    "action_id": "ca72f768-0f94-4536-9a51-90b5891df4a7",
    "archiveds": false,
    "asset_type": "asset",
    "catalogue_item_id": "7e9fe938-f2db-4cd5-8259-f22db5806a9c",
    "client": {
      "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "name": "Baumbach LLC"
    },
    "code": "6e6ce1459d4d78780f88",
    "color": "#000000",
    "colour": "#000000",
    "condition": {
      "uuid": "cb274607-0af0-40a1-96c9-3324d0639982",
      "name": "poor"
    },
    "condition_details": null,
    "in_storage": false,
    "installation_date": null,
    "item_attributes": [],
    "item_attributes_count": 0,
    "life_expectancy": 0.0,
    "location": {
      "uuid": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
      "name": "location name"
    },
    "photo": null,
    "photo_large_url": null,
    "photo_url": null,
    "pre_charged_for_disposal": false,
    "project": "sdd123465",
    "purchase_date": "2021-06-08T00:00:00.000+01:00",
    "purchase_price_cents": 123,
    "purchase_price_currency": "£",
    "reuse_action_id": null,
    "room": "new",
    "sale_price": 120.0,
    "slug": "6e6ce1459d4d78780f88",
    "stamps_count": 11,
    "status": {
      "uuid": "69bd2c6f-7311-421c-b956-4c55955ebe63",
      "name": "waiting_regeneration"
    },
    "usage": "in_use",
    "warranty": 15,
    "warranty_info": "vjk",
    "x": null,
    "y": null,
    "years_remaining": 0
  },
  "notes": [
    {
      "uuid": "7e51e0d2-1d62-4e94-b1d7-1654b51517f4",
      "body": "A note",
      "created_at": "2021-07-07T12:27:47.000+01:00",
      "item_id": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be",
      "note_type": null,
      "updated_at": "2021-07-07T12:27:47.000+01:00",
      "user_id": "5656d494-b4f8-4ee9-a48d-d3286d954a45"
    }
  ],
  "stamps": [
    {
      "uuid": "74e36833-09ae-4189-8df1-6d5f771851dd",
      "action_stamp": "estate_reused_and_refreshed",
      "action_stamp_type": 0,
      "created_at": "2021-06-01T09:17:55.000+01:00",
      "item_id": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be",
      "location_id": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
      "previous_location_id": null,
      "purchase_price_cents": null,
      "purchase_price_currency": "GBP",
      "status_id": "13c99ef3-70df-43b9-9638-5a5303a0ce81",
      "wear_off_date": "2021-09-01T01:00:00.000+01:00"
    }
  ]
}
```

This endpoint creates a new Item.

### HTTP Request

`POST http://localhost:3000/api/v7/items`

### Item Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
location_id | nil | The uuid of the location of the item | String | Yes
condition_id | nil | The uuid of the item's condition | String | Yes | See the Conditions endpoint
status_id | nil | The uuid of the item's status | String | Yes | See the Statuses endpoint
action_id | nil | an Action uuid | String | No | See the Actions endpoint
code | nil | A free text code identifier | String | Yes
usage | nil | Whether the Item is in use or unused | String | Yes | 'in_use', 'unused'
project | nil | A free text project identifier | String | No
x | nil | The x position of the item on its location's floorplan | Decimal | No | 0 to 1
y | nil | The y position of the item on its location's floorplan | Decimal | No | 0 to 1
purchase_date | nil | The purchase date | Date | No
purchase_price_cents | nil | The purchase price of the item in pence | Decimal | No
room | nil | A free text room identifier | String | No
warranty | nil | The warranty length in years | Integer | No
warranty_info | nil | Free text warranty information | Integer | No
installation_date | nil | Installation date | Date | No
life_expectancy | nil | The life expectancy of the item in years | Float | No
catalogue_item_id | nil | ??? | ??? | No
condition_details | nil | Free text information about item condition | String | No


### Nested Photo Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
image | nil | A file upload | String | No |

### Supported Media Types

multipart/form-data

### Nested Notes Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
user_id | nil | The uuid of a user | String | Yes |
body | nil | The note content | Text | No ??? |

### Nested Item Attributes Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
catalogue_association_id | | | | |
catalogue_attribute_id | | | | |
catalogue_attribute_name | | | | |
catalogue_attribute_type | | | | |
value | | | | |
