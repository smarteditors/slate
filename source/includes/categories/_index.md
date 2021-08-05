## Get All Categories

> `GET https://catalogue.smarteditors.co.uk/api/v6/categories`

> Example response

```json
{
  "request_id": "aa91941c-c20a-45cb-9d46-77f4e8e211d9",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "categories": [
    {
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
    }
  ]
}
```

This endpoint retrieves all Categories for the current client or for a specified Catalogue. 


### HTTP Request

`GET https://catalogue.smarteditors.co.uk/api/v6/categories`


### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
catalogue_id | nil | The uuid of a Catalogue | String | No