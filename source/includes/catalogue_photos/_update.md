## Update An Item With A Photo

> `PUT https://catalogue.smarteditors.co.uk/api/v6/photos/73f5f971-c6d6-4495-b2bf-022380d27c23`

```ruby
example_params = {
  file: [String]
}
```

> Example response

```json
{
  "request_id": "5c5c5901-0886-421a-a0bf-242c7cf5f4ff",
  "authority": {
      "email": "ian@eastenders.com"
  },
  "item": {
    "uuid": "23e256c1-03a4-4b18-90b8-486505365e16",
    "archived": false,
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
    },
    "client_id": "bb4867d3-1f26-4a0c-a645-4d185c9e9498",
    "code": "123sssdsddscaxfbscdsbesfgd",
    "confirmed": false,
    "csr_confirmation": false,
    "cubic": 2.0,
    "cubic_size": 0.0,
    "depreciation_rate": 0.0,
    "depreciation_term": 0,
    "description": null,
    "display_status": "",
    "embedded_co2": null,
    "from_edi": false,
    "house_position": "",
    "locking_user_id": null,
    "locking_user_name": null,
    "material": null,
    "max_stock_level": -1,
    "min_stock_level": -1,
    "name": "Remove my NULL",
    "photo": "https://s3-eu-west-1.amazonaws.com/sassy-catalogue-development/items/photos/000/000/007/original/test.jpeg?1626955776",
    "photo_content_type": "image/jpeg",
    "photo_file_name": "test.jpeg",
    "photo_file_size": 7466,
    "photo_updated_at": "2021-07-22T12:09:36.003Z",
    "price_as_new": null,
    "rate": 1.0,
    "sale_or_donation": "",
    "sales_reference": "S000007",
    "sfg": null,
    "slug": null,
    "snd_max_price": null,
    "snd_min_price": null,
    "status": null,
    "status_locked": false,
    "status_locked_at": null,
    "status_unlocked_at": null,
    "supplier_id": null,
    "term": 0,
    "type": {
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
    },
    "used_for": null,
    "weight": null
  }
}
```

This endpoint attaches an image file to a specific Catalogue Item record.

### HTTP Request

`PUT https://catalogue.smarteditors.co.uk/api/v6/photos/<ItemID>`


### URL Parameters

Parameter | Description
--------- | -----------
ItemID | The uuid of the Item to add the image to


### Supported Media Types

multipart/form-data

### Params

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
file | nil | A file upload | String | Yes |