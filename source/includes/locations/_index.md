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
      "address": "asc sac assc sac asc"
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
resource | nil | Used to specify the type of location required. Store and transit locations are only returned if specified with this param | String | No | stores, transits
client_id | current client id | Return locations linked to a specific client | Integer | No
asset_id | nil | ??? Looks like it is only used to select a client if no :client_id is submitted | Integer | No
query | nil | A search parameter applied to location fields | String | No | 
per_page | 10 | Number of items on each page of items returned | Integer | No | max 100
page | 1 | The page of paginated items returned | Integer | No | 
limit | 10 | The total number of items returned. Ignored if :per_page is submitted | No | No | 

