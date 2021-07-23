## Get All Catalogues

> `GET http://localhost:3001/api/v6/catalogues`

> Example response

```json
{
  "request_id": "754de387-fec0-4b25-af13-d959dcacf356",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "catalogues": [
    {
      "uuid": "c1ff6eb0-6adf-4834-86c3-f439640f3cbd",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "name": "caacs"
    },
    {
      "uuid": "91eef228-5a8d-4eb5-9a44-22af1c6307d0",
      "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
      "name": "dvzdv"
    }
  ]
}
```

This endpoint retrieves all Catalogues for the current client.

Catlogues are ????

### HTTP Request

`GET http://localhost:3001/api/v6/catalogues`
