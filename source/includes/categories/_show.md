## Get a Specific Category

> `GET http://localhost:3001/api/v6/categories/d55010cb-5d05-4749-b6b4-f08070cc21bb`

> Example response

```json
{
  "request_id": "ceebf6f5-2d5a-4bcd-8c36-fbbfadb81b81",
  "authority": {
    "email": "ian@eastenders.com"
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
  }
}
```

This endpoint retrieves a specific Category.

### HTTP Request

`GET http://localhost:3001/api/v6/categories/<ID>`
