## Get A List Of Types

> `GET https://catalogue.smarteditors.co.uk/api/v6/types`

> Example response

```json
{
  "request_id": "2e843ad3-4f95-469b-b2ea-6819df107fdb",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "types": [
    {
      "uuid": "574fbbc9-fcea-4dd4-b1df-7e6f9c2ccdf4",
      "archived": false,
      "category_id": "d55010cb-5d05-4749-b6b4-f08070cc21bb",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "cubic_size": 3.0,
      "depreciation_rate": 1.0,
      "depreciation_term": 0,
      "icon_content_type": null,
      "icon_file_name": null,
      "icon_file_size": null,
      "icon_updated_at": null,
      "name": "chair",
      "slug": null
    },
    {
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
    }
  ]
}
```

This endpoint retrieves a list of Types for the current client or for a specified Category. 

### HTTP Request

`GET https://catalogue.smarteditors.co.uk/api/v6/types`


### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
category_id | nil | The uuid of a Category | String | No