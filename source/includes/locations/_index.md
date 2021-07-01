## Get All Locations

> `GET http://localhost:3000/api/v6/meta/locations`

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
  "success": true,
  "locations": [
    {
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
      "address": "full address"
    }
  ],
  "meta": {
    "pagination": {
      "Link": {
        "first": "http://localhost:3000/api/v6/locations?page=1",
        "last": "http://localhost:3000/api/v6/locations?page=1"
      },
      "Current-Page": "1",
      "Page-Items": "10",
      "Total-Pages": "1",
      "Total-Count": "1"
    }
  }
}
```

This endpoint retrieves all root locations for the current client, or all child locations of a root location.

### HTTP Request

`GET http://localhost:3000/api/v6/meta/locations`

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

