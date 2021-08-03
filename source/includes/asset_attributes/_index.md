## Get All Asset Attributes

> `GET https://catalogue.smarteditors.co.uk/api/v6/attributes`

> Example response

```json
{
  "request_id": "4a4f24cc-2855-4878-aba3-c90d955abd8a",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "attributes": [
    {
      "uuid": "c4461f7f-0766-4432-9cd3-8954cf3f02b4",
      "field_name": "base_colour",
      "field_type": "colour",
      "field_values": "",
      "name": "base colour"
    },
    {
      "uuid": "201f0912-c111-4b2b-98e7-8fbfef6a976c",
      "field_name": "upholstery_colour",
      "field_type": "colour",
      "field_values": "",
      "name": "upholstery colour"
    }
  ]
}
```

This endpoint retrieves all Asset Attributes for the current client or for a Type.

### HTTP Request

`GET https://catalogue.smarteditors.co.uk/api/v6/attributes`


### Query Parameters

Parameter | Default | Description | Type | Required?
--------- | ------- | ----------- | ---- | --------
type_id | nil | The uuid of a Type | String | No