## Get A List Of Items

> `GET https://smartedi2.smarteditors.co.uk/api/v7/meta/items`

```ruby
example_params = {
  query: String,
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
  "request_id": "7a571cde-7904-4462-a30b-6a6638304d66",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "items": [
    {
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
      "item_attributes_count": 0,
      "life_expectancy": 0.0,
      "location": {
        "uuid": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
        "name": "location name"
      },
      "photo_large_url": null,
      "photo_url": null,
      "pre_charged_for_disposal": false,
      "project": "sdd",
      "purchase_date": "2021-06-08T00:00:00.000+01:00",
      "purchase_price_cents": 123,
      "purchase_price_currency": "£",
      "reuse_action_id": null,
      "room": "new",
      "sale_price": 120.0,
      "slug": "6e6ce1459d4d78780f88",
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
    }
  ],
  "meta": {
    "pagination": {
      "Link": {
        "first": "https://smartedi2.smarteditors.co.uk/api/v7/items?page=1",
        "next": "https://smartedi2.smarteditors.co.uk/api/v7/items?page=2",
        "last": "https://smartedi2.smarteditors.co.uk/api/v7/items?page=4"
      },
      "Current-Page": "1",
      "Page-Items": "10",
      "Total-Pages": "1",
      "Total-Count": "1"
    }
  }
}
```

This endpoint retrieves all Items for a client, with options to filter by location, 

### HTTP Request

`GET https://smartedi2.smarteditors.co.uk/api/v7/meta/items`

### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
query | nil | A string used to filter on the name and address fields of location | String | No
location_id | nil | The uuid of the locaton for which you want the items | String | No
per_page | 10 | Number of items on each page of items returned | Integer | No
page | 1 | The page of paginated items returned | Integer | No
limit | 10 | The total number of items returned. Ignored if :per_page is submitted | Integer | No

