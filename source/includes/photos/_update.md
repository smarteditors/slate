## Update A Photo

> `PUT http://localhost:3000/api/v7/photos/73f5f971-c6d6-4495-b2bf-022380d27c23`

```ruby
example_params = {
  file: [String]
}
```

> Example response

```json
{
  "request_id": "25042121-a728-489a-bd84-9fdc1e30ada7",
  "authority": {
    "email": "ian@eastenders.com"
  },
  "photo": {
    "uuid": "ab0c490d-93aa-4ba0-beae-58d160ad0132",
    "height": null,
    "image": {
      "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/test.jpeg",
      "thumb": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/thumb_test.jpeg"
      },
      "large": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/large_test.jpeg"
      },
      "square": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/square_test.jpeg"
      },
      "portrait": {
        "url": "https://awesome-assets-bucket.s3.amazonaws.com/development/uploads/photo/image/28/portrait_test.jpeg"
      }
    },
    "image_file_name": null,
    "image_source_url": null,
    "image_tmp": null,
    "item_id": "56d844f6-ebdf-476e-932b-8b7ca565b77e",
    "width": null
  }
}
```

This endpoint attached a file to a specific Photo record.

### HTTP Request

`PUT http://localhost:3000/api/v7/photos/<ID>`


### URL Parameters

Parameter | Description
--------- | -----------
ID | The uuid of the Photo to update


### Supported Media Types

multipart/form-data

### Params

Parameter | Default | Description | Type | Required? | Options
--------- | ------- | ----------- | ---- | --------- | -------
file | nil | A file upload | String | Yes |