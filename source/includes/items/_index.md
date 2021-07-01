## Get All Items For a Location

> `GET http://localhost:3000/api/v6/meta/items`

```ruby
example_params = {
  location_id: String,
  per_page: Integer,
  page: Integer,
  limit: Integer,
  ignore_current_client: Boolean
}
```

> Example response

```json
{
  "success": true,
  "items": [
    {
      "uuid": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "condition_id": "cb274607-0af0-40a1-96c9-3324d0639982",
      "status_id": "69bd2c6f-7311-421c-b956-4c55955ebe63",
      "location_id": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
      "catalogue_item_id": "7e9fe938-f2db-4cd5-8259-f22db5806a9c",
      "action_id": "ca72f768-0f94-4536-9a51-90b5891df4a7",
      "reuse_action_id": null,
      "code": "6e6ce1459d4d78780f88",
      "usage": "in_use",
      "project": "sdd",
      "slug": "6e6ce1459d4d78780f88",
      "x": null,
      "y": null,
      "warranty": 15,
      "warranty_info": "vjk",
      "purchase_price_cents": 123,
      "purchase_price_currency": "£",
      "purchase_date": "2021-06-08T00:00:00.000+01:00",
      "action_date": "2021-06-04T00:00:00.000+01:00",
      "room": "new",
      "colour": "#000000",
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
      "photo_url": null,
      "photo_large_url": null,
      "archiveds": false,
      "actions": [
        {
          "status": "44f6ff1a-5dd0-43b7-a618-6be681cdb9cc",
          "date": "2021-05-28T10:49:10.787+01:00",
          "location": "5509613e-ee0e-403e-9de9-dc9f500c3dd3"
        },
        {
          "status": "created",
          "date": "2021-05-28T10:49:11.000+01:00",
          "location": "5509613e-ee0e-403e-9de9-dc9f500c3dd3"
        }
      ],
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
        "icon": {
          "url": null
        },
        "width": null,
        "height": null,
        "client_id": null,
        "is_default": false,
        "reusable": false
      },
      "condition": {
        "uuid": "cb274607-0af0-40a1-96c9-3324d0639982",
        "name": "poor",
        "label": "Poor",
        "description": null,
        "client_id": null,
        "colour": null,
        "is_default": false
      },
      "item_attributes": []
    }
  ],
  "meta": {
    "pagination": {
      "Link": {
        "first": "http://localhost:3000/api/v6/items?location_id=1&page=1",
        "next": "http://localhost:3000/api/v6/items?location_id=1&page=2",
        "last": "http://localhost:3000/api/v6/items?location_id=1&page=4"
      },
      "Current-Page": "1",
      "Page-Items": "10",
      "Total-Pages": "4",
      "Total-Count": "36"
    }
  }
}
```

This endpoint retrieves all Items for a location.

### HTTP Request

`GET http://localhost:3000/api/v6/meta/items`

### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
location_id | nil | The uuid of the locaton for which you want the items | String |Yes
per_page | 10 | Number of items on each page of items returned | Integer | No
page | 1 | The page of paginated items returned | Integer | No
limit | 10 | The total number of items returned. Ignored if :per_page is submitted | Integer | No
ignore_current_client | false | ??? Ignore the client and return items from all clients. Need to hide or return items for all clients the user belongs to ??? | Integer | No

