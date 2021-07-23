## Search Categories

> `GET http://localhost:3001/api/v6/categories/search?catalogue_id=91eef228-5a8d-4eb5-9a44-22af1c6307d0&name=something`

> Example response

```json
{
  "request_id": "4867ff45-f7d9-4082-b81e-6bfec806d7a1",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "categories": [
    {
      "uuid": "d55010cb-5d05-4749-b6b4-f08070cc21bb",
      "colour": "#000000",
      "name": "test category"
    }
  ]
}
```

This endpoint retrieves Categories for a specific Catalogue and by a search term applied to the 'name' field. 


### HTTP Request

`GET http://localhost:3001/api/v6/categories/search`


### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
catalogue_id | nil | The uuid of a Catalogue | String | Yes
name | nil | A string to search categories by name | String | Yes