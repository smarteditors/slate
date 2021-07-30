## Create An Catalogue Item

> `POST http://localhost:3001/api/v6/items`

```ruby
example_params = {
  item: {
    name: String,
    type_id: String,
    code: String,
    client_id: String,
    archived: Boolean,
    confirmed: Boolean,
    sfg: String,
    status: String,
    attribute_associations_attributes: [
      {
        attribute_id: String,
        value: String,
        position: Integer
      }
    ]
  }
}
```

> Example response

```json
{
  "request_id": "577487cf-c9b8-4217-af8d-fe9c662a091e",
  "authority": {
      "email": "ian@eastenders.com"
  },
  "item": {
    "uuid": "b39709d1-d080-436d-96c3-e98d8348b16f",
    "archived": false,
    "catalogue": {
      "uuid": "91eef228-5a8d-4eb5-9a44-22af1c6307d0",
      "name": "dvzdv"
    },
    "category": {
      "uuid": "d55010cb-5d05-4749-b6b4-f08070cc21bb",
      "archived": false,
      "catalogue_id": "91eef228-5a8d-4eb5-9a44-22af1c6307d0",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "colour": "#000000",
      "depreciation_rate": 1.0,
      "depreciation_term": 0,
      "icon_content_type": null,
      "icon_file_size": null,
      "icon_updated_at": null,
      "name": "test category",
      "slug": null
    },
    "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "code": "123besfgd",
    "confirmed": false,
    "csr_confirmation": false,
    "cubic": 2.0,
    "cubic_size": 0.0,
    "depreciation_rate": 0.0,
    "depreciation_term": 0,
    "description": null,
    "display_status": "Awaiting Decision",
    "embedded_co2": null,
    "from_edi": false,
    "house_position": "",
    "locking_user_id": null,
    "locking_user_name": null,
    "material": null,
    "max_stock_level": -1,
    "min_stock_level": -1,
    "name": "Remove my NULL",
    "photo": "/images/missing.jpg",
    "photo_content_type": null,
    "photo_file_name": null,
    "photo_file_size": null,
    "photo_updated_at": null,
    "price_as_new": null,
    "rate": 1.0,
    "sale_or_donation": "",
    "sales_reference": "S000010",
    "sfg": "vdsdefv",
    "slug": null,
    "snd_max_price": null,
    "snd_min_price": null,
    "status": "awaiting_decision",
    "status_locked": false,
    "status_locked_at": null,
    "status_unlocked_at": null,
    "supplier_id": null,
    "term": 0,
    "type": {
      "uuid": "19b8af37-6dbc-49c3-9333-6e79b77980b0",
      "archived": false,
      "category_id": "d55010cb-5d05-4749-b6b4-f08070cc21bb",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "cubic_size": 2.0,
      "depreciation_rate": 0.0,
      "depreciation_term": 0,
      "icon_content_type": null,
      "icon_file_name": null,
      "icon_file_size": null,
      "icon_updated_at": null,
      "name": "new chair",
      "slug": null
    },
    "used_for": null,
    "weight": null
  },
  "attribute_associations": [
    {
      "uuid": "d8f4b105-51a4-46c0-ac04-85bdd3bb9387",
      "_value": [
        "plastic",
        "nylon",
        "wood"
      ],
      "attribute_id": "c4461f7f-0766-4432-9cd3-8954cf3f02b4",
      "attribute_type": "colour",
      "owner_attribute": {
        "uuid": "c4461f7f-0766-4432-9cd3-8954cf3f02b4",
        "field_name": "base_colour",
        "field_type": "colour",
        "field_values": "",
        "name": "base colour"
      },
      "owner_id": "b39709d1-d080-436d-96c3-e98d8348b16f",
      "owner_type": "Item",
      "position": 0,
      "required": true,
      "value": [
        "plastic",
        "nylon",
        "wood"
      ],
      "variable": false
    }
  ]
}
```

This endpoint creates a new Item. If an Item uuid is provided, the item will be updated instead.

### HTTP Request

`POST http://localhost:3001/api/v6/items`

### Item Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
archived | false | Whether the Item is archived or not | Boolean | No
client_id | nil | The uuid of the Client the Item belongs to | String | Yes
code | nil | A free text code identifier | String | Yes
confirmed | false | Whether the Item is confirmed or not | Boolean | No
name | 'Remove my NULL??? | The uuid of the location of the item | String | No
sfg | nil | An SFG20??? code | String | No
status | nil | The item status | String | No | 'estate_reuse', 'awaiting_decision', 'non_estate_reuse', 'for_review'
type_id | nil | The uuid of the Item's Type | String | Yes | See the Statuses endpoint
uuid | nil | The uuid of an Item. If a uuid is prvided the Item will be updated instead of a new one created. | String | Yes | See the Statuses endpoint


### Nested Attribute Associations Attributes Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
attribute_id | nil | The uuid of attribute to be linked to the Item by the AttributeAssociation | String | Yes |
value | nil | The value of the Attribute | String | No |
position | nil | The position of the AttributeAssociation in the list | Integer | No |
