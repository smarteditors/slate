## Get All Locations

> `GET http://localhost:3000/api/v7/meta/locations`

```ruby
example_params = {
  id: Integer,
  resource: String ['stores', 'transits'],
  client_id: Integer,
  asset_id: Integer,
  query: String,
  per_page: Integer,
  page: Integer,
  limit: Integer
}
```


> Example response

```json
{
  "request_id": "41258d5f-9cb4-41e8-be15-92686f85d042",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "locations": [
    {
      "uuid": "5509613e-ee0e-403e-9de9-dc9f500c3dd3",
      "_store_me_groups_for_transit": null,
      "absolute_path_name": "test location",
      "address": "line 1, line 2, town, county, SY16 3AN",
      "address_one": "line 1",
      "address_three": "line 3",
      "address_two": "line 2",
      "archived": false,
      "client": {
        "uuid": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
        "name": "Baumbach LLC"
      },
      "color": null,
      "county": "county",
      "cubic_capacity": 0.0,
      "from_location_uuid": null,
      "items_count": 37,
      "items_total_count": 37,
      "latitude": null,
      "levels": null,
      "longitude": null,
      "name": "test location",
      "parent_id": null,
      "post_code": "SY16 3AN",
      "previous_location_id": null,
      "slug": "test-location",
      "sort_order": null,
      "stacked_level": null,
      "storage_type_id": null,
      "store": false,
      "sub_location_type": null,
      "to_location_uuid": null,
      "town": "town",
      "transit": false,
      "transit_info": null,
      "x": null,
      "y": null
    }
  ],
  "meta": {
    "pagination": {
      "Link": {
        "first": "http://localhost:3000/api/v7/locations?page=1",
        "last": "http://localhost:3000/api/v7/locations?page=1"
      },
      "Current-Page": "1",
      "Page-Items": "10",
      "Total-Pages": "1",
      "Total-Count": "3"
    }
  }
}
```

This endpoint retrieves all root locations for the current client, or all child locations of a root location.

### HTTP Request

`GET http://localhost:3000/api/v7/meta/locations`

### Query Parameters

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | -------- | -------
id | nil | A location ID. If provided the endpoint returns the child locations of the parent location specified | Integer | No
resource | nil | Used to specify the type of location required. Store and transit locations are only returned if specified with this param | String | No | [stores, transits]
client_id | current client id | Return locations linked to a specific client | Integer | No
asset_id | nil | An Item ID. If no client_id is submitted, the client_id from this Item is used | Integer | No
query | nil | A search parameter applied to location fields | String | No | 
per_page | 10 | Number of items on each page of items returned | Integer | No | max 100
page | 1 | The page of paginated items returned | Integer | No | 
limit | 10 | The total number of items returned. Ignored if :per_page is submitted | No | No | 

