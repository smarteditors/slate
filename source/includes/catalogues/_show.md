## Get a Specific Catalogue

> `GET https://catalogue.smarteditors.co.uk/api/v6/catalogues/38f5d5a1-52e6-4091-b9cf-2d9bc34efc3f`

> Example response

```json
{
  "request_id": "4ec1e940-8bda-4d39-8dd1-5313fefcf72b",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "catalogue": {
    "uuid": "91eef228-5a8d-4eb5-9a44-22af1c6307d0",
    "catalogue_type": "ff_e",
    "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "name": "catalogue 1"
  }
}
```

This endpoint retrieves a specific catalogue.

### HTTP Request

`GET https://catalogue.smarteditors.co.uk/api/v6/catalogues/<ID>`
