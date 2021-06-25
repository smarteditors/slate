## Get All Assets For a Location

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
      "id": 27,
      "client_id": 1,
      "condition_id": 3,
      "status_id": 23,
      "code": "6e6ce1459d4d78780f88",
      "usage": "in_use",
      "project": "sdd",
      "catalogue_item_id": "1",
      "slug": "6e6ce1459d4d78780f88",
      "uuid": "6f6e1ce5-24d0-4a5c-8e19-28dfa31537be",
      "created_at": "2021-05-28T10:49:11.000+01:00",
      "updated_at": "2021-06-04T12:14:24.000+01:00",
      "location_id": 1,
      "x": null,
      "y": null,
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
      "photo": null,
      "photo_url": null,
      "photo_large_url": null,
      "archiveds": false,
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

This endpoint retrieves all Assets for a location.

### HTTP Request

`GET http://localhost:3000/api/v6/meta/items`

### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
location_id | null | The uuid of the locaton for which you want the assets | String |Yes
per_page | 10 | Number of items on each page of items returned | Integer | No
page | 1 | The page of paginated items returned | Integer | No
limit | 10 | The total number of items returned. Ignored if :per_page is submitted | Integer | No
ignore_current_client | false | Ignore the client and return items from all clients | Integer | No

